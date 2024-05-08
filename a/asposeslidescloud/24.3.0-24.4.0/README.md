# Comparing `tmp/asposeslidescloud-24.3.0.tar.gz` & `tmp/asposeslidescloud-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-24.3.0.tar", last modified: Wed Mar 27 23:58:14 2024, max compression
+gzip compressed data, was "dist/asposeslidescloud-24.4.0.tar", last modified: Tue May  7 17:32:42 2024, max compression
```

## Comparing `asposeslidescloud-24.3.0.tar` & `asposeslidescloud-24.4.0.tar`

### file list

```diff
@@ -1,282 +1,284 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2024-03-27 23:57:53.000000 asposeslidescloud-24.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7331 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6943 2024-03-27 23:57:56.000000 asposeslidescloud-24.3.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    18926 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27782 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      313 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1439127 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)    37269 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_async_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    18642 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    19086 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19249 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     4661 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/comment_author.py
--rw-rw-r--   0 root         (0) root         (0)     4362 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/comment_authors.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9834 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8034 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    31358 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3786 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5671 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)    10067 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5403 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6112 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8469 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/handout_layouting_options.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     8010 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    13883 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     6289 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)    11264 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_comments_layouting_options.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14357 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7722 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)    11732 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/operation.py
--rw-rw-r--   0 root         (0) root         (0)     5643 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/operation_progress.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    22614 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6410 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8662 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6977 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7858 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    18243 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    13365 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3765 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5587 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    13162 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)    36756 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_transition.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)     4908 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slides_layout_options.py
--rw-rw-r--   0 root         (0) root         (0)    15450 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5494 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7883 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7716 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    16063 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    22416 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     7735 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_merge_options.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_split_type.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    13912 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_module.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_project.py
--rw-rw-r--   0 root         (0) root         (0)     4613 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_reference.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15861 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10569 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15494 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7331 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11799 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2024-03-27 23:58:02.000000 asposeslidescloud-24.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-05-07 17:32:31.000000 asposeslidescloud-24.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7751 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7363 2024-05-07 17:32:32.000000 asposeslidescloud-24.4.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    19069 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27782 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      313 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1452457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)    37269 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_async_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    18785 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    19086 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6363 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    19249 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4726 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     4661 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/comment_author.py
+-rw-rw-r--   0 root         (0) root         (0)     4362 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/comment_authors.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9834 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8759 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    31358 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3786 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5671 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)    10067 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5403 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6112 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8469 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/handout_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     8010 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    13883 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     6289 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    14076 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/markdown_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3378 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_format.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    11264 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_comments_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14357 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7805 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)    11732 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/operation.py
+-rw-rw-r--   0 root         (0) root         (0)     5643 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/operation_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    22614 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6410 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8662 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7453 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6977 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7858 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    18243 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    13365 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3765 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5587 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    13162 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    36756 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_transition.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4908 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slides_layout_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15450 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5494 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7883 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7716 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    16063 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    13912 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_module.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_project.py
+-rw-rw-r--   0 root         (0) root         (0)     4613 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_reference.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15861 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10569 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15494 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7751 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11891 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2024-05-07 17:32:36.000000 asposeslidescloud-24.4.0/setup.py
```

### Comparing `asposeslidescloud-24.3.0/LICENSE` & `asposeslidescloud-24.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/PKG-INFO` & `asposeslidescloud-24.4.0/README`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: asposeslidescloud
-Version: 24.3.0
-Summary: Aspose.Slides Cloud SDK for Python
-Home-page: 
-Author: Victor Putrov
-Author-email: vistor.putrov@aspose.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -36,14 +23,19 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.4
+
+* Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
+* Added **Marker** property to **DataPoint** class.
+
 ## Enhancements in Version 24.3
 
 * Added Markdown (**Md**) to the list of allowed export formats.
 * Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
 * Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
 * Added **AnimateTextType** enum property to **Effect** class.
 * Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
```

### Comparing `asposeslidescloud-24.3.0/README` & `asposeslidescloud-24.4.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: asposeslidescloud
+Version: 24.4.0
+Summary: Aspose.Slides Cloud SDK for Python
+Home-page: 
+Author: Victor Putrov
+Author-email: vistor.putrov@aspose.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -23,14 +36,19 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.4
+
+* Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
+* Added **Marker** property to **DataPoint** class.
+
 ## Enhancements in Version 24.3
 
 * Added Markdown (**Md**) to the list of allowed export formats.
 * Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
 * Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
 * Added **AnimateTextType** enum property to **Effect** class.
 * Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/__init__.py` & `asposeslidescloud-24.4.0/asposeslidescloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,17 +152,19 @@
 from asposeslidescloud.models.legend import Legend
 from asposeslidescloud.models.light_rig import LightRig
 from asposeslidescloud.models.limit_element import LimitElement
 from asposeslidescloud.models.line_format import LineFormat
 from asposeslidescloud.models.line_to_path_segment import LineToPathSegment
 from asposeslidescloud.models.literals import Literals
 from asposeslidescloud.models.luminance_effect import LuminanceEffect
+from asposeslidescloud.models.markdown_export_options import MarkdownExportOptions
 from asposeslidescloud.models.master_slide import MasterSlide
 from asposeslidescloud.models.master_slides import MasterSlides
 from asposeslidescloud.models.math_element import MathElement
+from asposeslidescloud.models.math_format import MathFormat
 from asposeslidescloud.models.math_paragraph import MathParagraph
 from asposeslidescloud.models.matrix_element import MatrixElement
 from asposeslidescloud.models.merge import Merge
 from asposeslidescloud.models.merging_source import MergingSource
 from asposeslidescloud.models.move_to_path_segment import MoveToPathSegment
 from asposeslidescloud.models.nary_operator_element import NaryOperatorElement
 from asposeslidescloud.models.no_fill import NoFill
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/api_client.py` & `asposeslidescloud-24.4.0/asposeslidescloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v24.3.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v24.4.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-24.4.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7795,15 +7795,15 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def delete_picture_cropped_areas(self, name, slide_index, shape_index, password, folder, storage = None, **kwargs):  # noqa: E501
+    def delete_picture_cropped_areas(self, name, slide_index, shape_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Deletes cropped areas of a pictire.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, shape_index, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
@@ -7821,15 +7821,15 @@
         kwargs['_return_http_data_only'] = True
         if kwargs.get('is_async'):
             return self.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, **kwargs)  # noqa: E501
         else:
             (data) = self.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, **kwargs)  # noqa: E501
             return data
 
-    def delete_picture_cropped_areas_with_http_info(self, name, slide_index, shape_index, password, folder, storage = None, **kwargs):  # noqa: E501
+    def delete_picture_cropped_areas_with_http_info(self, name, slide_index, shape_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Deletes cropped areas of a pictire.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
@@ -7865,20 +7865,14 @@
             raise ValueError("Missing the required parameter `name` when calling `delete_picture_cropped_areas`")  # noqa: E501
         # verify the required parameter 'slide_index' is set
         if not slide_index:
             raise ValueError("Missing the required parameter `slide_index` when calling `delete_picture_cropped_areas`")  # noqa: E501
         # verify the required parameter 'shape_index' is set
         if not shape_index:
             raise ValueError("Missing the required parameter `shape_index` when calling `delete_picture_cropped_areas`")  # noqa: E501
-        # verify the required parameter 'password' is set
-        if not password:
-            raise ValueError("Missing the required parameter `password` when calling `delete_picture_cropped_areas`")  # noqa: E501
-        # verify the required parameter 'folder' is set
-        if not folder:
-            raise ValueError("Missing the required parameter `folder` when calling `delete_picture_cropped_areas`")  # noqa: E501
 
         collection_formats = {}
 
         path_params = {}
         path_params['name'] = name  # noqa: E501
         path_params['slideIndex'] = slide_index  # noqa: E501
         path_params['shapeIndex'] = shape_index  # noqa: E501
@@ -7896,15 +7890,15 @@
         form_params = []
         param_files = {}
 
         body_params = None
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
-            ['multipart/form-data'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['JWT']  # noqa: E501
 
         return self.api_client.call_api(
             '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/pictureCroppedAreas', 'DELETE',
             path_params,
@@ -13051,14 +13045,151 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def download_math_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, format, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Convert Mathematical Text to MathML Format  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, paragraph_index, portion_index, format, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param format Format.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: file
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.download_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.download_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def download_math_portion_with_http_info(self, name, slide_index, shape_index, paragraph_index, portion_index, format, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Convert Mathematical Text to MathML Format  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.download_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param format Format.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: file
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method download_math_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `download_math_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `download_math_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `download_math_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `download_math_portion`")  # noqa: E501
+        # verify the required parameter 'portion_index' is set
+        if not portion_index:
+            raise ValueError("Missing the required parameter `portion_index` when calling `download_math_portion`")  # noqa: E501
+        # verify the required parameter 'format' is set
+        if not format:
+            raise ValueError("Missing the required parameter `format` when calling `download_math_portion`")  # noqa: E501
+        # verify the value of parameter 'format' is valid
+        if not format.upper() in MathFormat.__dict__:
+            raise ValueError("Invalid value for parameter `format` when calling `download_math_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+        path_params['portionIndex'] = portion_index  # noqa: E501
+        path_params['format'] = format  # noqa: E501
+
+        query_params = []
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/paragraphs/{paragraphIndex}/portions/{portionIndex}/{format}', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='file',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def download_notes_slide(self, name, slide_index, format, width = None, height = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Convert notes slide to the specified image format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, format, width, height, password, folder, storage, fonts_folder, is_async=True)
         >>> result = thread.get()
@@ -24899,14 +25030,158 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def save_math_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Convert Mathematical Text to MathML Format and saves result to the storage  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param format Format.
+        :param out_path Path to save result.
+        :param password Document password.
+        :param folder Presentation folder.
+        :param storage Presentation storage.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.save_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.save_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def save_math_portion_with_http_info(self, name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Convert Mathematical Text to MathML Format and saves result to the storage  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.save_math_portion_with_http_info(name, slide_index, shape_index, paragraph_index, portion_index, format, out_path, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index.
+        :param paragraph_index Paragraph index.
+        :param portion_index Portion index.
+        :param format Format.
+        :param out_path Path to save result.
+        :param password Document password.
+        :param folder Presentation folder.
+        :param storage Presentation storage.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = []  # noqa: E501
+        all_params.append('is_async')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method save_math_portion" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'paragraph_index' is set
+        if not paragraph_index:
+            raise ValueError("Missing the required parameter `paragraph_index` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'portion_index' is set
+        if not portion_index:
+            raise ValueError("Missing the required parameter `portion_index` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'format' is set
+        if not format:
+            raise ValueError("Missing the required parameter `format` when calling `save_math_portion`")  # noqa: E501
+        # verify the value of parameter 'format' is valid
+        if not format.upper() in MathFormat.__dict__:
+            raise ValueError("Invalid value for parameter `format` when calling `save_math_portion`")  # noqa: E501
+        # verify the required parameter 'out_path' is set
+        if not out_path:
+            raise ValueError("Missing the required parameter `out_path` when calling `save_math_portion`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
+        path_params['paragraphIndex'] = paragraph_index  # noqa: E501
+        path_params['portionIndex'] = portion_index  # noqa: E501
+        path_params['format'] = format  # noqa: E501
+
+        query_params = []
+        if out_path:
+            query_params.append(('outPath', out_path))  # noqa: E501
+        if folder:
+            query_params.append(('folder', folder))  # noqa: E501
+        if storage:
+            query_params.append(('storage', storage))  # noqa: E501
+
+        header_params = {}
+        if password:
+            header_params['password'] = password  # noqa: E501
+
+        form_params = []
+        param_files = {}
+
+        body_params = None
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/paragraphs/{paragraphIndex}/portions/{portionIndex}/{format}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type=None,  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
     def save_portion_as_math_ml(self, name, slide_index, shape_index, paragraph_index, portion_index, out_path, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Convert Mathematical Text to MathML Format and saves result to the storage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, shape_index, paragraph_index, portion_index, out_path, password, folder, storage, is_async=True)
         >>> result = thread.get()
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_async_api.py` & `asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_async_api.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/configuration.py` & `asposeslidescloud-24.4.0/asposeslidescloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 24.3.0".\
+               "SDK Package Version: 24.4.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/error_message.py` & `asposeslidescloud-24.4.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,17 +144,19 @@
 from asposeslidescloud.models.legend import Legend
 from asposeslidescloud.models.light_rig import LightRig
 from asposeslidescloud.models.limit_element import LimitElement
 from asposeslidescloud.models.line_format import LineFormat
 from asposeslidescloud.models.line_to_path_segment import LineToPathSegment
 from asposeslidescloud.models.literals import Literals
 from asposeslidescloud.models.luminance_effect import LuminanceEffect
+from asposeslidescloud.models.markdown_export_options import MarkdownExportOptions
 from asposeslidescloud.models.master_slide import MasterSlide
 from asposeslidescloud.models.master_slides import MasterSlides
 from asposeslidescloud.models.math_element import MathElement
+from asposeslidescloud.models.math_format import MathFormat
 from asposeslidescloud.models.math_paragraph import MathParagraph
 from asposeslidescloud.models.matrix_element import MatrixElement
 from asposeslidescloud.models.merge import Merge
 from asposeslidescloud.models.merging_source import MergingSource
 from asposeslidescloud.models.move_to_path_segment import MoveToPathSegment
 from asposeslidescloud.models.nary_operator_element import NaryOperatorElement
 from asposeslidescloud.models.no_fill import NoFill
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/audio_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,44 +43,46 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
+        'marker': 'SeriesMarker',
         'type': 'str',
         'x_value': 'float',
         'y_value': 'float',
         'x_value_formula': 'str',
         'y_value_formula': 'str',
         'bubble_size': 'float',
         'bubble_size_formula': 'str'
     }
 
     attribute_map = {
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
+        'marker': 'marker',
         'type': 'type',
         'x_value': 'xValue',
         'y_value': 'yValue',
         'x_value_formula': 'xValueFormula',
         'y_value_formula': 'yValueFormula',
         'bubble_size': 'bubbleSize',
         'bubble_size_formula': 'bubbleSizeFormula'
     }
 
     type_determiners = {
         'type': 'Bubble',
     }
 
-    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, type='Bubble', x_value=None, y_value=None, x_value_formula=None, y_value_formula=None, bubble_size=None, bubble_size_formula=None):  # noqa: E501
+    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, marker=None, type='Bubble', x_value=None, y_value=None, x_value_formula=None, y_value_formula=None, bubble_size=None, bubble_size_formula=None):  # noqa: E501
         """BubbleChartDataPoint - a model defined in Swagger"""  # noqa: E501
-        super(BubbleChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, type, x_value, y_value, x_value_formula, y_value_formula)
+        super(BubbleChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, marker, type, x_value, y_value, x_value_formula, y_value_formula)
 
         self._bubble_size = None
         self._bubble_size_formula = None
         self.type = 'Bubble'
 
         if bubble_size is not None:
             self.bubble_size = bubble_size
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_title.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/comment_author.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/comment_author.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/comment_authors.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/comment_authors.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/connector.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/data_point.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,45 +42,50 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
+        'marker': 'SeriesMarker',
         'type': 'str'
     }
 
     attribute_map = {
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
+        'marker': 'marker',
         'type': 'type'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, type=None):  # noqa: E501
+    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, marker=None, type=None):  # noqa: E501
         """DataPoint - a model defined in Swagger"""  # noqa: E501
 
         self._fill_format = None
         self._effect_format = None
         self._three_d_format = None
         self._line_format = None
+        self._marker = None
         self._type = None
 
         if fill_format is not None:
             self.fill_format = fill_format
         if effect_format is not None:
             self.effect_format = effect_format
         if three_d_format is not None:
             self.three_d_format = three_d_format
         if line_format is not None:
             self.line_format = line_format
+        if marker is not None:
+            self.marker = marker
         if type is not None:
             self.type = type
 
     @property
     def fill_format(self):
         """Gets the fill_format of this DataPoint.  # noqa: E501
 
@@ -165,14 +170,36 @@
 
         :param line_format: The line_format of this DataPoint.  # noqa: E501
         :type: LineFormat
         """
         self._line_format = line_format
 
     @property
+    def marker(self):
+        """Gets the marker of this DataPoint.  # noqa: E501
+
+        Gets or sets the marker.  # noqa: E501
+
+        :return: The marker of this DataPoint.  # noqa: E501
+        :rtype: SeriesMarker
+        """
+        return self._marker
+
+    @marker.setter
+    def marker(self, marker):
+        """Sets the marker of this DataPoint.
+
+        Gets or sets the marker.  # noqa: E501
+
+        :param marker: The marker of this DataPoint.  # noqa: E501
+        :type: SeriesMarker
+        """
+        self._marker = marker
+
+    @property
     def type(self):
         """Gets the type of this DataPoint.  # noqa: E501
 
 
         :return: The type of this DataPoint.  # noqa: E501
         :rtype: str
         """
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/document.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/error.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/graphical_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/handout_layouting_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/handout_layouting_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/html5_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/html_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/image.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/images.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/input.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_comments_layouting_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_comments_layouting_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,40 +43,42 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
+        'marker': 'SeriesMarker',
         'type': 'str',
         'value': 'float',
         'value_formula': 'str',
         'set_as_total': 'bool',
         'invert_if_negative': 'bool'
     }
 
     attribute_map = {
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
+        'marker': 'marker',
         'type': 'type',
         'value': 'value',
         'value_formula': 'valueFormula',
         'set_as_total': 'setAsTotal',
         'invert_if_negative': 'invertIfNegative'
     }
 
     type_determiners = {
         'type': 'OneValue',
     }
 
-    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, type='OneValue', value=None, value_formula=None, set_as_total=None, invert_if_negative=None):  # noqa: E501
+    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, marker=None, type='OneValue', value=None, value_formula=None, set_as_total=None, invert_if_negative=None):  # noqa: E501
         """OneValueChartDataPoint - a model defined in Swagger"""  # noqa: E501
-        super(OneValueChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, type)
+        super(OneValueChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, marker, type)
 
         self._value = None
         self._value_formula = None
         self._set_as_total = None
         self._invert_if_negative = None
         self.type = 'OneValue'
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/operation.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/operation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/operation_progress.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/operation_progress.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/path_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/pdf_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/pdf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/picture_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/portions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/save.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/save.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/save_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,40 +43,42 @@
                             and the value is json key in definition.
     """
     swagger_types = {
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
+        'marker': 'SeriesMarker',
         'type': 'str',
         'x_value': 'float',
         'y_value': 'float',
         'x_value_formula': 'str',
         'y_value_formula': 'str'
     }
 
     attribute_map = {
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
+        'marker': 'marker',
         'type': 'type',
         'x_value': 'xValue',
         'y_value': 'yValue',
         'x_value_formula': 'xValueFormula',
         'y_value_formula': 'yValueFormula'
     }
 
     type_determiners = {
         'type': 'Scatter',
     }
 
-    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, type='Scatter', x_value=None, y_value=None, x_value_formula=None, y_value_formula=None):  # noqa: E501
+    def __init__(self, fill_format=None, effect_format=None, three_d_format=None, line_format=None, marker=None, type='Scatter', x_value=None, y_value=None, x_value_formula=None, y_value_formula=None):  # noqa: E501
         """ScatterChartDataPoint - a model defined in Swagger"""  # noqa: E501
-        super(ScatterChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, type)
+        super(ScatterChartDataPoint, self).__init__(fill_format, effect_format, three_d_format, line_format, marker, type)
 
         self._x_value = None
         self._y_value = None
         self._x_value_formula = None
         self._y_value_formula = None
         self.type = 'Scatter'
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/section.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/series.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_base.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_transition.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_transition.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/slides_layout_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/slides_layout_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_merge_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_merge_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_split_type.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_split_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/task.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/text_items.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/tiff_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/tiff_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_module.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_module.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_project.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_project.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_reference.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_reference.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/video_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-24.4.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud/rest.py` & `asposeslidescloud-24.4.0/asposeslidescloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-24.4.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 24.3.0
+Version: 24.4.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,19 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.4
+
+* Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
+* Added **Marker** property to **DataPoint** class.
+
 ## Enhancements in Version 24.3
 
 * Added Markdown (**Md**) to the list of allowed export formats.
 * Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
 * Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
 * Added **AnimateTextType** enum property to **Effect** class.
 * Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
```

### Comparing `asposeslidescloud-24.3.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-24.4.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,19 @@
 asposeslidescloud/models/legend.py
 asposeslidescloud/models/light_rig.py
 asposeslidescloud/models/limit_element.py
 asposeslidescloud/models/line_format.py
 asposeslidescloud/models/line_to_path_segment.py
 asposeslidescloud/models/literals.py
 asposeslidescloud/models/luminance_effect.py
+asposeslidescloud/models/markdown_export_options.py
 asposeslidescloud/models/master_slide.py
 asposeslidescloud/models/master_slides.py
 asposeslidescloud/models/math_element.py
+asposeslidescloud/models/math_format.py
 asposeslidescloud/models/math_paragraph.py
 asposeslidescloud/models/matrix_element.py
 asposeslidescloud/models/merge.py
 asposeslidescloud/models/merging_source.py
 asposeslidescloud/models/move_to_path_segment.py
 asposeslidescloud/models/nary_operator_element.py
 asposeslidescloud/models/no_fill.py
```

### Comparing `asposeslidescloud-24.3.0/setup.py` & `asposeslidescloud-24.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="24.3.0",
+    version="24.4.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

