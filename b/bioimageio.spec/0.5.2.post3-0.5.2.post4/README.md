# Comparing `tmp/bioimageio.spec-0.5.2.post3.tar.gz` & `tmp/bioimageio.spec-0.5.2.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioimageio.spec-0.5.2.post3.tar", last modified: Tue Apr 30 14:07:24 2024, max compression
+gzip compressed data, was "bioimageio.spec-0.5.2.post4.tar", last modified: Wed May  8 13:56:51 2024, max compression
```

## Comparing `bioimageio.spec-0.5.2.post3.tar` & `bioimageio.spec-0.5.2.post4.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.333912 bioimageio.spec-0.5.2.post3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-30 14:07:24.333912 bioimageio.spec-0.5.2.post3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18438 2024-04-30 14:07:21.000000 bioimageio.spec-0.5.2.post3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.313912 bioimageio.spec-0.5.2.post3/bioimageio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.317912 bioimageio.spec-0.5.2.post3/bioimageio/spec/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-30 14:07:21.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_build_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_description.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.321912 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/_generated_spdx_license_literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/common_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/field_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/field_warning.py
--rw-r--r--   0 runner    (1001) docker     (127)    20589 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/io.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/io_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-30 14:07:21.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/packaging_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/root_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     4367 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-30 14:07:21.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validation_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validator_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/warning_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/_package.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.321912 bioimageio.spec-0.5.2.post3/bioimageio/spec/application/
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/application/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/application/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.321912 bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12926 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/v0_3.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.321912 bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/_v0_2_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/_v0_3_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/_v0_4_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41548 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)   101035 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/model/v0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/imjoy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/imjoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/pretty_validation_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/bioimageio/spec/static/
--rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/static/spdx_licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/static/tag_categories.json
--rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/bioimageio/spec/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.317912 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    19267 2024-04-30 14:07:24.000000 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-04-30 14:07:24.000000 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 14:07:24.000000 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-30 14:07:24.000000 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-30 14:07:24.000000 bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.313912 bioimageio.spec-0.5.2.post3/example_descriptions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.313912 bioimageio.spec-0.5.2.post3/example_descriptions/collections/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/example_descriptions/collections/unet2d_nuclei_broad_coll/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.313912 bioimageio.spec-0.5.2.post3/example_descriptions/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_diff_output_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_fixed_shape/
--rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-04-30 14:04:57.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_fixed_shape/unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_multi_tensor/
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.325912 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_nuclei_broad/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.329912 bioimageio.spec-0.5.2.post3/example_descriptions/models/upsample_test_model/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/example_descriptions/models/upsample_test_model/upsample_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.329912 bioimageio.spec-0.5.2.post3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/compare_yaml_syntax.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/generate_dtype_limits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/generate_json_schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/generate_spec_documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/generate_version_submodule_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/report_invalid_rdfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/scripts/update_spdx_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 14:07:24.333912 bioimageio.spec-0.5.2.post3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.329912 bioimageio.spec-0.5.2.post3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_bioimageio_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_description.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_example_specs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.329912 bioimageio.spec-0.5.2.post3/tests/test_generic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_generic/test_v0_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_generic/test_v0_3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.333912 bioimageio.spec-0.5.2.post3/tests/test_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_file_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_license_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_validated_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_internal/test_version_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 14:07:24.333912 bioimageio.spec-0.5.2.post3/tests/test_model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_model/test_v0_4.py
--rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_model/test_v0_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-30 14:04:58.000000 bioimageio.spec-0.5.2.post3/tests/test_specific_reexports_generics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.511952 bioimageio.spec-0.5.2.post4/bioimageio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.519952 bioimageio.spec-0.5.2.post4/bioimageio/spec/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_build_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_description.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10694 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_generated_spdx_license_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16162 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/common_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20517 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10274 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/packaging_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/root_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3694 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validation_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validator_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/warning_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1930 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9712 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11116 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12933 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_2_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15487 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14252 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.523953 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_3_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_4_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41555 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101042 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8530 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/pretty_validation_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   258617 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/spdx_licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/static/tag_categories.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/bioimageio/spec/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20231 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-08 13:56:51.000000 bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/collections/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.515952 bioimageio.spec-0.5.2.post4/example_descriptions/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    12778 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/
+-rw-r--r--   0 runner    (1001) docker     (127)    21841 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/example_descriptions/models/upsample_test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/example_descriptions/models/upsample_test_model/upsample_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.527953 bioimageio.spec-0.5.2.post4/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/compare_yaml_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_dtype_limits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_json_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17796 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_spec_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5903 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/generate_version_submodule_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12159 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/report_invalid_rdfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/scripts/update_spdx_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_bioimageio_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_example_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_generic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7086 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_file_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_license_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5362 2024-05-08 13:56:49.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_validated_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_internal/test_version_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 13:56:51.531952 bioimageio.spec-0.5.2.post4/tests/test_model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15505 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-05-08 13:54:33.000000 bioimageio.spec-0.5.2.post4/tests/test_specific_reexports_generics.py
```

### Comparing `bioimageio.spec-0.5.2.post3/LICENSE` & `bioimageio.spec-0.5.2.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/PKG-INFO` & `bioimageio.spec-0.5.2.post4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioimageio.spec
-Version: 0.5.2.post3
+Version: 0.5.2.post4
 Summary: Parser and validator library for bioimage.io specifications
 Home-page: https://github.com/bioimage-io/spec-bioimage-io
 Author: bioimage.io Team
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
 Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
 Platform: UNKNOWN
@@ -21,17 +21,19 @@
 
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains specifications defined by the bioimage.io community. These specifications are used for defining fields in YAML 1.2 files which should be named `rdf.yaml`. Such a rdf.yaml --- along with files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g. image analysis software like ilastik).
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
 
-bioimage.io-compatible resources must fulfill the following rules:
+[These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
 Please also note that the best way to check whether your `rdf.yaml` file is bioimage.io-compliant is to call `bioimageio.core.validate` from the [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package.
 The [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package also provides the bioimageio command line interface (CLI) with the `validate` command:
@@ -62,40 +64,56 @@
 | latest | [bioimageio_schema_latest.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_latest.json) |
 | 0.5 | [bioimageio_schema_v0-5.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_v0-5.json) |
 
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
-We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md).
+We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
+and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
+
 
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`, we recommend to install `bioimageio.core` instead:
+bioimageio.spec can be installed with either `conda` or `pip`. 
+We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
 
 ```console
 pip install -U bioimageio.core
 ```
 
+Still, for a lighter package or just testing, you can install the `bioimageio.spec` package solely:
+
+```console
+conda install -c conda-forge bioimageio.spec
+```
+
+or
+
+```console
+pip install -U bioimageio.spec
+```
+
+
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -106,14 +124,20 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post4
+
+* resolve backup DOIs
+* fix resolving relative file paths given as strings
+* allow to bypass download and hashing of known files
+
 #### bioimageio.spec 0.5.2post3
 
 * avoid full download when validating urls
 
 #### bioimageio.spec 0.5.2post2
 
 * resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
```

### Comparing `bioimageio.spec-0.5.2.post3/README.md` & `bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,39 @@
+Metadata-Version: 2.1
+Name: bioimageio.spec
+Version: 0.5.2.post4
+Summary: Parser and validator library for bioimage.io specifications
+Home-page: https://github.com/bioimage-io/spec-bioimage-io
+Author: bioimage.io Team
+License: UNKNOWN
+Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
+Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains specifications defined by the bioimage.io community. These specifications are used for defining fields in YAML 1.2 files which should be named `rdf.yaml`. Such a rdf.yaml --- along with files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g. image analysis software like ilastik).
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
 
-bioimage.io-compatible resources must fulfill the following rules:
+[These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
 Please also note that the best way to check whether your `rdf.yaml` file is bioimage.io-compliant is to call `bioimageio.core.validate` from the [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package.
 The [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package also provides the bioimageio command line interface (CLI) with the `validate` command:
@@ -41,40 +64,56 @@
 | latest | [bioimageio_schema_latest.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_latest.json) |
 | 0.5 | [bioimageio_schema_v0-5.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_v0-5.json) |
 
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
-We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md).
+We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
+and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
+
 
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`, we recommend to install `bioimageio.core` instead:
+bioimageio.spec can be installed with either `conda` or `pip`. 
+We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
 
 ```console
 pip install -U bioimageio.core
 ```
 
+Still, for a lighter package or just testing, you can install the `bioimageio.spec` package solely:
+
+```console
+conda install -c conda-forge bioimageio.spec
+```
+
+or
+
+```console
+pip install -U bioimageio.spec
+```
+
+
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -85,14 +124,20 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post4
+
+* resolve backup DOIs
+* fix resolving relative file paths given as strings
+* allow to bypass download and hashing of known files
+
 #### bioimageio.spec 0.5.2post3
 
 * avoid full download when validating urls
 
 #### bioimageio.spec 0.5.2post2
 
 * resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
@@ -433,7 +478,9 @@
   * Change `authors` and `packaged_by` fields from List[str] to List[Author] with Author consisting of a dictionary `{name: '<Full name>', affiliation: '<Affiliation>', orcid: 'optional orcid id'}`;
   * Add a mandatory `type` field to comply with the generic description. Only valid value is 'model' for model description;
   * Only allow `license` identifier from the [SPDX license list](https://spdx.org/licenses/);
 
 * Non-breaking changes
   * Add optional `version` field (default 0.1.0) to keep track of model changes;
   * Allow the values in the `attachments` list to be any values besides URI;
+
+
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_build_description.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_build_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_description.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/_generated_spdx_license_literals.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_generated_spdx_license_literals.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/_settings.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/_settings.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/common_nodes.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/common_nodes.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/constants.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/docs_utils.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/docs_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/field_validation.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_validation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/field_warning.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/field_warning.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from pydantic_core.core_schema import (
     NoInfoValidatorFunction,
     ValidationInfo,
     WithInfoValidatorFunction,
 )
 from typing_extensions import Annotated, LiteralString
 
-from .._internal.validation_context import validation_context_var
-from .._internal.warning_levels import WARNING, WarningSeverity
+from .validation_context import validation_context_var
+from .warning_levels import WARNING, WarningSeverity
 
 if TYPE_CHECKING:
     from pydantic.functional_validators import _V2Validator  # type: ignore
 
 if sys.version_info < (3, 10):
     SLOTS: Dict[str, Any] = {}
 else:
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/io.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import hashlib
 import sys
 import warnings
 from abc import abstractmethod
 from dataclasses import dataclass
 from datetime import date as _date
 from datetime import datetime as _datetime
+from functools import lru_cache
 from pathlib import Path, PurePath
 from typing import (
     Any,
-    ClassVar,
     Dict,
     Generic,
     Iterable,
     List,
     Optional,
     Sequence,
     Tuple,
@@ -34,65 +34,51 @@
     Field,
     FilePath,
     GetCoreSchemaHandler,
     PlainSerializer,
     PrivateAttr,
     RootModel,
     SerializationInfo,
-    StringConstraints,
     TypeAdapter,
     model_validator,
 )
 from pydantic_core import core_schema
 from typing_extensions import (
     Annotated,
     LiteralString,
     NotRequired,
     Self,
     Unpack,
     assert_never,
 )
 from typing_extensions import TypeAliasType as _TypeAliasType
 
-from .._internal._settings import settings
-from .._internal.io_basics import (
+from ._settings import settings
+from .io_basics import (
     ALL_BIOIMAGEIO_YAML_NAMES,
     ALTERNATIVE_BIOIMAGEIO_YAML_NAMES,
     BIOIMAGEIO_YAML,
     AbsoluteDirectory,
     AbsoluteFilePath,
     FileName,
+    Sha256,
 )
-from .._internal.node import Node
-from .._internal.packaging_context import packaging_context_var
-from .._internal.root_url import RootHttpUrl
-from .._internal.url import HttpUrl
-from .._internal.validated_string import ValidatedString
-from .._internal.validation_context import ValidationContext, validation_context_var
+from .node import Node
+from .packaging_context import packaging_context_var
+from .root_url import RootHttpUrl
+from .url import HttpUrl
+from .validation_context import validation_context_var
 from .validator_annotations import AfterValidator
 
 if sys.version_info < (3, 10):
     SLOTS: Dict[str, bool] = {}
 else:
     SLOTS = {"slots": True}
 
 
-class Sha256(ValidatedString):
-    """SHA-256 hash value"""
-
-    root_model: ClassVar[Type[RootModel[Any]]] = RootModel[
-        Annotated[
-            str,
-            StringConstraints(
-                strip_whitespace=True, to_lower=True, min_length=64, max_length=64
-            ),
-        ]
-    ]
-
-
 AbsolutePathT = TypeVar(
     "AbsolutePathT", bound=Union[HttpUrl, AbsoluteDirectory, AbsoluteFilePath]
 )
 
 
 class RelativePathBase(RootModel[PurePath], Generic[AbsolutePathT], frozen=True):
     _absolute: AbsolutePathT = PrivateAttr()
@@ -184,15 +170,16 @@
 ):
     def get_absolute(
         self, root: "RootHttpUrl | Path | AnyUrl"
     ) -> "AbsoluteFilePath | AbsoluteDirectory | HttpUrl":
         absolute = self._get_absolute_impl(root)
         if (
             isinstance(absolute, Path)
-            and validation_context_var.get().perform_io_checks
+            and (context := validation_context_var.get()).perform_io_checks
+            and str(self.root) not in context.known_files
             and not absolute.exists()
         ):
             raise ValueError(f"{absolute} does not exist")
 
         return absolute
 
 
@@ -205,15 +192,16 @@
 
     def get_absolute(
         self, root: "RootHttpUrl | Path | AnyUrl"
     ) -> "AbsoluteFilePath | HttpUrl":
         absolute = self._get_absolute_impl(root)
         if (
             isinstance(absolute, Path)
-            and validation_context_var.get().perform_io_checks
+            and (context := validation_context_var.get()).perform_io_checks
+            and str(self.root) not in context.known_files
             and not absolute.is_file()
         ):
             raise ValueError(f"{absolute} does not point to an existing file")
 
         return absolute
 
 
@@ -231,15 +219,15 @@
         ):
             raise ValueError(f"{absolute} does not point to an existing directory")
 
         return absolute
 
 
 FileSource = Annotated[
-    Union[FilePath, RelativeFilePath, HttpUrl, pydantic.HttpUrl],
+    Union[FilePath, HttpUrl, RelativeFilePath, pydantic.HttpUrl],
     Field(union_mode="left_to_right"),
 ]
 PermissiveFileSource = Union[FileSource, str]
 
 V_suffix = TypeVar("V_suffix", bound=FileSource)
 path_or_url_adapter = TypeAdapter(Union[FilePath, DirectoryPath, HttpUrl])
 
@@ -523,15 +511,15 @@
 def interprete_file_source(file_source: PermissiveFileSource) -> StrictFileSource:
     if isinstance(file_source, (HttpUrl, Path)):
         return file_source
 
     if isinstance(file_source, pydantic.AnyUrl):
         file_source = str(file_source)
 
-    with ValidationContext(perform_io_checks=False):
+    with validation_context_var.get().replace(perform_io_checks=False):
         strict = _strict_file_source_adapter.validate_python(file_source)
 
     return strict
 
 
 def _get_known_hash(hash_kwargs: HashKwargs):
     if "sha256" in hash_kwargs and hash_kwargs["sha256"] is not None:
@@ -613,17 +601,21 @@
     """SHA256 checksum of the source file"""
 
     @model_validator(mode="after")
     def validate_sha256(self) -> Self:
         context = validation_context_var.get()
         if not context.perform_io_checks:
             return self
+        elif (src_str := str(self.source)) in context.known_files:
+            actual_sha = context.known_files[src_str]
+        else:
+            local_source = download(self.source, sha256=self.sha256).path
+            actual_sha = get_sha256(local_source)
+            context.known_files[str(self.source)] = actual_sha
 
-        local_source = download(self.source, sha256=self.sha256).path
-        actual_sha = get_sha256(local_source)
         if self.sha256 is None:
             self.sha256 = actual_sha
         elif self.sha256 != actual_sha:
             raise ValueError(
                 f"Sha256 mismatch for {self.source}. Expected {self.sha256}, got "
                 + f"{actual_sha}. Update expected `sha256` or point to the matching "
                 + "file."
@@ -652,14 +644,15 @@
             and url.path.endswith("/content")
         ):
             return url.path.split("/")[-2]
         else:
             return url.path.split("/")[-1]
 
 
+@lru_cache
 def get_sha256(path: Path) -> Sha256:
     """from https://stackoverflow.com/a/44873382"""
     h = hashlib.sha256()
     b = bytearray(128 * 1024)
     mv = memoryview(b)
     with open(path, "rb", buffering=0) as f:
         for n in iter(lambda: f.readinto(mv), 0):
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/io_utils.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/io_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,20 +28,19 @@
 from ._settings import settings
 from .io import (
     BIOIMAGEIO_YAML,
     BioimageioYamlContent,
     FileDescr,
     HashKwargs,
     OpenedBioimageioYaml,
-    Sha256,
     YamlValue,
     download,
     find_bioimageio_yaml_file_name,
 )
-from .io_basics import FileName
+from .io_basics import FileName, Sha256
 from .types import FileSource, PermissiveFileSource
 
 yaml = YAML(typ="safe")
 
 
 def read_yaml(file: Union[FilePath, TextIO]) -> YamlValue:
     if isinstance(file, Path):
@@ -196,14 +195,19 @@
                 else Sha256(entry["entry_sha256"])
             ),
             version=str(entry["version_number"]),
         )
         # set version specific entry
         ret[c_entry.id + "/" + str(entry["version_number"])] = c_entry
 
+        # set doi entry
+        doi = entry.get("doi")
+        if doi is not None:
+            ret[doi] = c_entry
+
         # update 'latest version' entry
         if c_entry.id not in ret:
             update = True
         else:
             old_v = ret[c_entry.id].version
             v = c_entry.version
 
@@ -212,14 +216,18 @@
                     v.replace("staged/", "")
                 ) > int(old_v.replace("staged/", ""))
             else:
                 update = not v.startswith("staged") and int(v) > int(old_v)
 
         if update:
             ret[c_entry.id] = c_entry
+            # set concept doi entry
+            concept_doi = entry.get("concept_doi")
+            if concept_doi is not None:
+                ret[concept_doi] = c_entry
 
     return ret
 
 
 @lru_cache
 def get_collection() -> Mapping[str, _CollectionEntry]:
     try:
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/license_id.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/node.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/packaging_context.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/packaging_context.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/root_url.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/root_url.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/types.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from typing_extensions import Annotated, Literal
 
 from .constants import DOI_REGEX, SI_UNIT_REGEX
 from .io import FileSource as FileSource
 from .io import ImportantFileSource as ImportantFileSource
 from .io import PermissiveFileSource as PermissiveFileSource
 from .io import RelativeFilePath as RelativeFilePath
-from .io import Sha256 as Sha256
 from .io_basics import AbsoluteDirectory as AbsoluteDirectory
 from .io_basics import AbsoluteFilePath as AbsoluteFilePath
 from .io_basics import FileName as FileName
+from .io_basics import Sha256 as Sha256
 from .license_id import DeprecatedLicenseId as DeprecatedLicenseId
 from .license_id import LicenseId as LicenseId
 from .url import HttpUrl as HttpUrl
 from .validated_string import ValidatedString
 from .validator_annotations import AfterValidator, BeforeValidator
 from .version_type import Version as Version
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/url.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/url.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from .field_warning import issue_warning
 from .root_url import RootHttpUrl
 from .validation_context import validation_context_var
 
 
 def _validate_url(url: Union[str, pydantic.HttpUrl]) -> pydantic.AnyUrl:
     url = str(url)
-    if not validation_context_var.get().perform_io_checks:
+    context = validation_context_var.get()
+    if not context.perform_io_checks or url in context.known_files:
         return pydantic.AnyUrl(url)
 
     val_url = url
 
     if url.startswith("https://colab.research.google.com/github/"):
         # get requests for colab returns 200 even if the source notebook does not exists.
         # We therefore validate the url to the notebbok instead (for github notebooks)
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/utils.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validated_string.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validation_context.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validation_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from contextvars import ContextVar, Token
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 from urllib.parse import urlsplit, urlunsplit
 
 from pydantic import DirectoryPath
 
 from ._settings import settings
-from .io_basics import AbsoluteDirectory, FileName
+from .io_basics import AbsoluteDirectory, FileName, Sha256
 from .root_url import RootHttpUrl
 from .warning_levels import WarningLevel
 
 
 @dataclass(frozen=True)
 class ValidationContext:
     _context_tokens: "List[Token[ValidationContext]]" = field(
@@ -34,34 +34,39 @@
 
     perform_io_checks: bool = settings.perform_io_checks
     """wether or not to perform validation that requires file io,
     e.g. downloading a remote files.
 
     Existence of local absolute file paths is still being checked."""
 
+    known_files: Dict[str, Sha256] = field(default_factory=dict)
+    """allows to bypass download and hashing of referenced files"""
+
     def replace(
         self,
         root: Optional[Union[RootHttpUrl, DirectoryPath]] = None,
         warning_level: Optional[WarningLevel] = None,
         log_warnings: Optional[bool] = None,
         file_name: Optional[str] = None,
         perform_io_checks: Optional[bool] = None,
+        known_files: Optional[Dict[str, Sha256]] = None,
     ) -> "ValidationContext":
         return ValidationContext(
             root=self.root if root is None else root,
             warning_level=(
                 self.warning_level if warning_level is None else warning_level
             ),
             log_warnings=self.log_warnings if log_warnings is None else log_warnings,
             file_name=self.file_name if file_name is None else file_name,
             perform_io_checks=(
                 self.perform_io_checks
                 if perform_io_checks is None
                 else perform_io_checks
             ),
+            known_files=self.known_files if known_files is None else known_files,
         )
 
     def __enter__(self):
         self._context_tokens.append(validation_context_var.set(self))
         return self
 
     def __exit__(self, type, value, traceback):  # type: ignore
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/validator_annotations.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/validator_annotations.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/version_type.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/version_type.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_internal/warning_levels.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_internal/warning_levels.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_io.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_io.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/_package.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/application/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/application/v0_2.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/application/v0_3.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/application/v0_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Literal, Optional
 
 from pydantic import Field
 from typing_extensions import Annotated
 
 from .._internal.common_nodes import Node
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.types import ImportantFileSource
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import Doi as Doi
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/v0_2.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/collection/v0_3.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/collection/v0_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from pydantic import PrivateAttr, model_validator
 from typing_extensions import Self
 
 from .._build_description import build_description_impl, get_rd_class_impl
 from .._internal.common_nodes import InvalidDescr, Node
 from .._internal.field_warning import issue_warning
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io import YamlValue
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.io_utils import open_bioimageio_yaml
 from .._internal.types import FileSource, NotEmpty
 from .._internal.url import HttpUrl as HttpUrl
 from .._internal.validation_context import (
     validation_context_var,
 )
 from .._internal.warning_levels import ALERT
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/common.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from pydantic import ValidationError as ValidationError
 
 from ._internal.common_nodes import InvalidDescr as InvalidDescr
 from ._internal.io import BioimageioYamlContent as BioimageioYamlContent
 from ._internal.io import BioimageioYamlSource as BioimageioYamlSource
 from ._internal.io import FileDescr as FileDescr
-from ._internal.io import Sha256 as Sha256
 from ._internal.io import YamlValue as YamlValue
 from ._internal.io_basics import AbsoluteDirectory as AbsoluteDirectory
 from ._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
 from ._internal.io_basics import FileName as FileName
+from ._internal.io_basics import Sha256 as Sha256
 from ._internal.root_url import RootHttpUrl as RootHttpUrl
 from ._internal.types import FileSource as FileSource
 from ._internal.types import PermissiveFileSource as PermissiveFileSource
 from ._internal.types import RelativeFilePath as RelativeFilePath
 from ._internal.url import HttpUrl as HttpUrl
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/v0_2.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/dataset/v0_3.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/dataset/v0_3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import TYPE_CHECKING, Any, Dict, Literal, Optional, cast
 
 from pydantic import model_validator
 
 from .._internal.common_nodes import InvalidDescr, Node
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import (
     DocumentationSource,
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/_v0_2_converter.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_2_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/v0_2.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/generic/v0_3.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/generic/v0_3.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
     BioimageioYamlContent,
     V_suffix,
     YamlValue,
     include_in_package_serializer,
     validate_suffix,
 )
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io_basics import AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.license_id import LicenseId
 from .._internal.types import (
     DeprecatedLicenseId,
     ImportantFileSource,
     NotEmpty,
 )
 from .._internal.types import RelativeFilePath as RelativeFilePath
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/model/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/model/_v0_3_converter.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_3_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/model/_v0_4_converter.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/_v0_4_converter.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/model/v0_4.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_4.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 from .._internal.io import (
     BioimageioYamlContent,
     WithSuffix,
     download,
     include_in_package_serializer,
 )
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.packaging_context import packaging_context_var
 from .._internal.types import Datetime as Datetime
 from .._internal.types import Identifier as Identifier
 from .._internal.types import ImportantFileSource, LowerCaseIdentifier
 from .._internal.types import LicenseId as LicenseId
 from .._internal.types import NotEmpty as NotEmpty
 from .._internal.url import HttpUrl as HttpUrl
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/model/v0_5.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/model/v0_5.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,17 +55,17 @@
     Node,
     NodeWithExplicitlySetFields,
 )
 from .._internal.constants import DTYPE_LIMITS
 from .._internal.field_warning import issue_warning, warn
 from .._internal.io import BioimageioYamlContent as BioimageioYamlContent
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io import WithSuffix, YamlValue, download
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.io_utils import load_array
 from .._internal.types import Datetime as Datetime
 from .._internal.types import DeprecatedLicenseId as DeprecatedLicenseId
 from .._internal.types import Identifier as Identifier
 from .._internal.types import (
     ImportantFileSource,
     LowerCaseIdentifier,
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/__init__.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/v0_2.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/notebook/v0_3.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/notebook/v0_3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Literal, Optional
 
 from .._internal.common_nodes import Node
 from .._internal.io import FileDescr as FileDescr
-from .._internal.io import Sha256 as Sha256
 from .._internal.io_basics import AbsoluteFilePath as AbsoluteFilePath
+from .._internal.io_basics import Sha256 as Sha256
 from .._internal.url import HttpUrl as HttpUrl
 from ..generic.v0_3 import VALID_COVER_IMAGE_EXTENSIONS as VALID_COVER_IMAGE_EXTENSIONS
 from ..generic.v0_3 import Author as Author
 from ..generic.v0_3 import BadgeDescr as BadgeDescr
 from ..generic.v0_3 import CiteEntry as CiteEntry
 from ..generic.v0_3 import Doi as Doi
 from ..generic.v0_3 import GenericDescrBase
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/partner_utils/imjoy/_plugin_parser.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/pretty_validation_errors.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/pretty_validation_errors.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/static/spdx_licenses.json` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/static/spdx_licenses.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/static/tag_categories.json` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/static/tag_categories.json`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio/spec/summary.py` & `bioimageio.spec-0.5.2.post4/bioimageio/spec/summary.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/PKG-INFO` & `bioimageio.spec-0.5.2.post4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-Metadata-Version: 2.1
-Name: bioimageio.spec
-Version: 0.5.2.post3
-Summary: Parser and validator library for bioimage.io specifications
-Home-page: https://github.com/bioimage-io/spec-bioimage-io
-Author: bioimage.io Team
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/bioimage-io/spec-bioimage-io/issues
-Project-URL: Source, https://github.com/bioimage-io/spec-bioimage-io
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 ![License](https://img.shields.io/github/license/bioimage-io/spec-bioimage-io.svg)
 ![PyPI](https://img.shields.io/pypi/v/bioimageio-spec.svg?style=popout)
 ![conda-version](https://anaconda.org/conda-forge/bioimageio.spec/badges/version.svg)
 
 # Specifications for bioimage.io
 
-This repository contains specifications defined by the bioimage.io community. These specifications are used for defining fields in YAML 1.2 files which should be named `rdf.yaml`. Such a rdf.yaml --- along with files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g. image analysis software like ilastik).
+This repository contains the specifications of the standard format defined by the bioimage.io community for the content (i.e., models, datasets and applications) in the [bioimage.io website](https://bioimage.io). 
+Each item in the content is always described using a YAML 1.2 file named `rdf.yaml` or `bioimageio.yaml`. 
+This `rdf.yaml` \ `bioimageio.yaml`--- along with the files referenced in it --- can be downloaded from or uploaded to the [bioimage.io website](https://bioimage.io) and may be produced or consumed by bioimage.io-compatible consumers (e.g., image analysis software like ilastik). 
 
-bioimage.io-compatible resources must fulfill the following rules:
+[These](https://github.com/bioimage-io/spec-bioimage-io?tab=readme-ov-file#format-version-overview) are the rules and format that bioimage.io-compatible resources must fulfill.
 
 Note that the Python package PyYAML does not support YAML 1.2 .
 We therefore use and recommend [ruyaml](https://ruyaml.readthedocs.io/en/latest/).
 For differences see <https://ruamelyaml.readthedocs.io/en/latest/pyyaml>.
 
 Please also note that the best way to check whether your `rdf.yaml` file is bioimage.io-compliant is to call `bioimageio.core.validate` from the [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package.
 The [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python) Python package also provides the bioimageio command line interface (CLI) with the `validate` command:
@@ -62,40 +43,56 @@
 | latest | [bioimageio_schema_latest.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_latest.json) |
 | 0.5 | [bioimageio_schema_v0-5.json](https://github.com/bioimage-io/spec-bioimage-io/blob/gh-pages/bioimageio_schema_v0-5.json) |
 
 These are primarily intended for syntax highlighting and form generation.
 
 ## Examples
 
-We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md).
+We provide some [examples for using rdf.yaml files to describe models, applications, notebooks and datasets](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example_descriptions/examples.md),
+and an [example notebook to programmatically access the models, applications, notebooks and datasets descriptions](https://github.com/bioimage-io/spec-bioimage-io/blob/main/example/load_model_and_create_your_own.ipynb).
+
 
 ## 💁 Recommendations
 
 * Due to the limitations of storage services such as Zenodo, which does not support subfolders, it is recommended to place other files in the same directory level of the `rdf.yaml` file and try to avoid using subdirectories.
 * Use the [bioimageio.core Python package](https://github.com/bioimage-io/core-bioimage-io-python) to validate your `rdf.yaml` file.
 * bioimageio.spec keeps evolving. Try to use and upgrade to the most current format version!
 
 ## ⌨ bioimageio command-line interface (CLI)
 
 The bioimageio CLI has moved entirely to [bioimageio.core](https://github.com/bioimage-io/core-bioimage-io-python).
 
 ## 🖥 Installation
 
-bioimageio.spec can be installed with either `conda` or `pip`, we recommend to install `bioimageio.core` instead:
+bioimageio.spec can be installed with either `conda` or `pip`. 
+We recommend installing `bioimageio.core` instead to get access to the Python programmatic features available in the BioImage.IO community:
 
 ```console
 conda install -c conda-forge bioimageio.core
 ```
 
 or
 
 ```console
 pip install -U bioimageio.core
 ```
 
+Still, for a lighter package or just testing, you can install the `bioimageio.spec` package solely:
+
+```console
+conda install -c conda-forge bioimageio.spec
+```
+
+or
+
+```console
+pip install -U bioimageio.spec
+```
+
+
 ## 🏞 Environment variables
 
 TODO: link to settings in dev docs
 
 ## 🤝 How to contribute
 
 ## ♥ Contributors
@@ -106,14 +103,20 @@
 
 Made with [contrib.rocks](https://contrib.rocks).
 
 ## Δ Changelog
 
 ### bioimageio.spec Python package
 
+#### bioimageio.spec 0.5.2post4
+
+* resolve backup DOIs
+* fix resolving relative file paths given as strings
+* allow to bypass download and hashing of known files
+
 #### bioimageio.spec 0.5.2post3
 
 * avoid full download when validating urls
 
 #### bioimageio.spec 0.5.2post2
 
 * resolve version (un)specific collection IDs, e.g. `load_description('affable-shark')`, `load_description('affable-shark/1')`
@@ -454,9 +457,7 @@
   * Change `authors` and `packaged_by` fields from List[str] to List[Author] with Author consisting of a dictionary `{name: '<Full name>', affiliation: '<Affiliation>', orcid: 'optional orcid id'}`;
   * Add a mandatory `type` field to comply with the generic description. Only valid value is 'model' for model description;
   * Only allow `license` identifier from the [SPDX license list](https://spdx.org/licenses/);
 
 * Non-breaking changes
   * Add optional `version` field (default 0.1.0) to keep track of model changes;
   * Allow the values in the `attachments` list to be any values besides URI;
-
-
```

### Comparing `bioimageio.spec-0.5.2.post3/bioimageio.spec.egg-info/SOURCES.txt` & `bioimageio.spec-0.5.2.post4/bioimageio.spec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/collections/unet2d_nuclei_broad_coll/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_diff_output_shape/resize_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_fixed_shape/unet.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_fixed_shape/unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_multi_tensor/multi_tensor_unet.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_nuclei_broad/unet2d.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py` & `bioimageio.spec-0.5.2.post4/example_descriptions/models/unet2d_nuclei_broad/unet2d_expand_output_shape.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/pyproject.toml` & `bioimageio.spec-0.5.2.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/compare_yaml_syntax.py` & `bioimageio.spec-0.5.2.post4/scripts/compare_yaml_syntax.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/generate_json_schemas.py` & `bioimageio.spec-0.5.2.post4/scripts/generate_json_schemas.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/generate_spec_documentation.py` & `bioimageio.spec-0.5.2.post4/scripts/generate_spec_documentation.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/generate_version_submodule_imports.py` & `bioimageio.spec-0.5.2.post4/scripts/generate_version_submodule_imports.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/report_invalid_rdfs.py` & `bioimageio.spec-0.5.2.post4/scripts/report_invalid_rdfs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/scripts/update_spdx_licenses.py` & `bioimageio.spec-0.5.2.post4/scripts/update_spdx_licenses.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/setup.py` & `bioimageio.spec-0.5.2.post4/setup.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_bioimageio_collection.py` & `bioimageio.spec-0.5.2.post4/tests/test_bioimageio_collection.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_description.py` & `bioimageio.spec-0.5.2.post4/tests/test_description.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_example_specs.py` & `bioimageio.spec-0.5.2.post4/tests/test_example_specs.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_generic/test_v0_2.py` & `bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_2.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_generic/test_v0_3.py` & `bioimageio.spec-0.5.2.post4/tests/test_generic/test_v0_3.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_constants.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_constants.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_file_source.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_file_source.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_license_id.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_license_id.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_node.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_node.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_types.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from pathlib import Path
 
 import pytest
 from dateutil.parser import isoparse
 from pydantic import PlainSerializer, TypeAdapter
 from typing_extensions import Annotated
 
+import bioimageio.spec._internal.io_basics
 from bioimageio.spec._internal import types
 from bioimageio.spec._internal.io import RelativeFilePath
 from bioimageio.spec._internal.types import Datetime, SiUnit
 from tests.utils import check_type
 
 TYPE_ARGS = {
     types.Datetime: (2024, 2, 14),
@@ -26,15 +27,15 @@
     types.RelativeFilePath: Path(__file__).relative_to(Path().absolute()),
     types.SiUnit: "kg",
     types.AbsoluteDirectory: str(Path(__file__).absolute().parent),
     types.AbsoluteFilePath: str(Path(__file__).absolute()),
     types.FileName: "lala.py",
     types.Version: "1.0",
     types.HttpUrl: "http://example.com",
-    types.Sha256: "0" * 64,
+    bioimageio.spec._internal.io_basics.Sha256: "0" * 64,
 }
 
 IGNORE_TYPES_MEMBERS = {
     "AfterValidator",
     "annotated_types",
     "Annotated",
     "annotations",
```

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_utils.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_validate.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_validate.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_internal/test_validated_string.py` & `bioimageio.spec-0.5.2.post4/tests/test_internal/test_validated_string.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_io.py` & `bioimageio.spec-0.5.2.post4/tests/test_io.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 
 
 @pytest.mark.parametrize(
     "rid",
     [
         "invigorating-lab-coat",
         "invigorating-lab-coat/1",
-        "invigorating-lab-coat/staged/1",
+        "10.5281/zenodo.11092896",  # backup doi of version 1
+        "10.5281/zenodo.11092895",  # concept doi of backup
     ],
 )
 def test_load_by_id(rid: str):
     from bioimageio.spec import InvalidDescr, load_description
 
     model = load_description(rid)
     assert not isinstance(model, InvalidDescr)
-    assert model.id == rid.split("/")[0]
+    assert model.id == "invigorating-lab-coat"
```

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_model/test_v0_4.py` & `bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_4.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_model/test_v0_5.py` & `bioimageio.spec-0.5.2.post4/tests/test_model/test_v0_5.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_package.py` & `bioimageio.spec-0.5.2.post4/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `bioimageio.spec-0.5.2.post3/tests/test_specific_reexports_generics.py` & `bioimageio.spec-0.5.2.post4/tests/test_specific_reexports_generics.py`

 * *Files identical despite different names*

