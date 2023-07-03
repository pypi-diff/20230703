# Comparing `tmp/asposeslidescloud-23.4.0.tar.gz` & `tmp/asposeslidescloud-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-23.4.0.tar", last modified: Sun Apr 23 12:37:00 2023, max compression
+gzip compressed data, was "dist/asposeslidescloud-23.6.0.tar", last modified: Sun Jul  2 00:10:40 2023, max compression
```

## Comparing `asposeslidescloud-23.4.0.tar` & `asposeslidescloud-23.6.0.tar`

### file list

```diff
@@ -1,270 +1,273 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-04-23 12:36:30.000000 asposeslidescloud-23.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8064 2023-04-23 12:36:34.000000 asposeslidescloud-23.4.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    18067 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    28194 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      246 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1421835 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    17850 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    18977 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19140 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9725 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8034 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    25610 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4827 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)     9958 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5294 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6003 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5966 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    20135 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    11286 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14248 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7722 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    28850 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6348 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6404 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8656 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7749 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    17369 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    12213 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5424 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    12171 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)    15341 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5385 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7774 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7607 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15954 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    22416 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     7735 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_merge_options.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_split_type.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    17671 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14060 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2023-04-23 12:36:25.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10460 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15420 2023-04-23 12:36:26.000000 asposeslidescloud-23.4.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8452 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11248 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-23 12:37:00.000000 asposeslidescloud-23.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2023-04-23 12:36:41.000000 asposeslidescloud-23.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-02 00:10:20.000000 asposeslidescloud-23.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8330 2023-07-02 00:10:22.000000 asposeslidescloud-23.6.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    18249 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    28146 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      246 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1445375 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    18032 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    18977 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6280 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    19140 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4726 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9725 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8034 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    25610 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3772 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4827 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)     9958 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5294 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6003 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5966 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    20135 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    11286 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14248 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7722 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    28850 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6348 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6404 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8656 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7370 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6868 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7749 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    17369 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    12213 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3751 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5424 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    12171 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)    15341 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5385 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7774 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7607 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15954 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    17671 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_module.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_project.py
+-rw-rw-r--   0 root         (0) root         (0)     4613 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/vba_reference.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14060 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10460 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15494 2023-07-02 00:10:17.000000 asposeslidescloud-23.6.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8718 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11369 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-02 00:10:40.000000 asposeslidescloud-23.6.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2023-07-02 00:10:27.000000 asposeslidescloud-23.6.0/setup.py
```

### Comparing `asposeslidescloud-23.4.0/LICENSE` & `asposeslidescloud-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/PKG-INFO` & `asposeslidescloud-23.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 23.4.0
+Version: 23.6.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,18 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.6
+
+* Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
+
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
 * Added **UpdateTableCell** method to update table cells.
 * Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
 * Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
 * New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
```

### Comparing `asposeslidescloud-23.4.0/README` & `asposeslidescloud-23.6.0/README`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.6
+
+* Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
+
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
 * Added **UpdateTableCell** method to update table cells.
 * Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
 * Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
 * New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/__init__.py` & `asposeslidescloud-23.6.0/asposeslidescloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,14 +268,17 @@
 from asposeslidescloud.models.text_items import TextItems
 from asposeslidescloud.models.theme import Theme
 from asposeslidescloud.models.three_d_format import ThreeDFormat
 from asposeslidescloud.models.tiff_export_options import TiffExportOptions
 from asposeslidescloud.models.tint_effect import TintEffect
 from asposeslidescloud.models.update_background import UpdateBackground
 from asposeslidescloud.models.update_shape import UpdateShape
+from asposeslidescloud.models.vba_module import VbaModule
+from asposeslidescloud.models.vba_project import VbaProject
+from asposeslidescloud.models.vba_reference import VbaReference
 from asposeslidescloud.models.video_export_options import VideoExportOptions
 from asposeslidescloud.models.video_frame import VideoFrame
 from asposeslidescloud.models.view_properties import ViewProperties
 from asposeslidescloud.models.workbook import Workbook
 from asposeslidescloud.models.xy_series import XYSeries
 from asposeslidescloud.models.xaml_export_options import XamlExportOptions
 from asposeslidescloud.models.xps_export_options import XpsExportOptions
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/api_client.py` & `asposeslidescloud-23.6.0/asposeslidescloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v23.4.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v23.6.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
@@ -129,20 +129,20 @@
         # perform request and return response
         response_data = self.__call_api_with_refresh(
             method, url, query_params, header_params, post_params, body, files, _preload_content, _request_timeout)
 
         self.last_response = response_data
 
         return_data = response_data
-        if _preload_content:
-            # deserialize response data
-            if response_type:
-                return_data = self.deserialize(response_data, response_type)
-            else:
-                return_data = None
+
+        # deserialize response data
+        if response_type:
+            return_data = self.deserialize(response_data, response_type)
+        else:
+            return_data = None
 
         if _return_http_data_only:
             return (return_data)
         else:
             return (return_data, response_data.status, response_data.getheaders())
 
     def __call_api_with_refresh(self, method, url, query_params, header_params, post_params, body, files, _preload_content, _request_timeout):
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-23.6.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-23.6.0/asposeslidescloud/apis/slides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def align_special_slide_shapes(self, name, slide_index, slide_type, alignment_type, align_to_slide = None, shapes = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Changes the placement of selected shapes on the master slide. Aligns shapes to the margins or the edge of the slide or aligns them relative to each other.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -314,15 +314,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def compress_embedded_fonts(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Compresses embedded fonts by removing unused characters.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -422,15 +422,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def compress_embedded_fonts_online(self, document, password = None, **kwargs):  # noqa: E501
         """Compresses embedded fonts by removing unused characters.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -523,15 +523,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def convert(self, document, format, password = None, storage = None, fonts_folder = None, slides = None, options = None, **kwargs):  # noqa: E501
         """Convert presentation from request content to format specified.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -650,15 +650,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def convert_and_save(self, document, format, out_path, password = None, storage = None, fonts_folder = None, slides = None, options = None, **kwargs):  # noqa: E501
         """Convert presentation from request content to format specified.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -784,15 +784,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def copy_file(self, src_path, dest_path, src_storage_name = None, dest_storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Copy file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -899,15 +899,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def copy_folder(self, src_path, dest_path, src_storage_name = None, dest_storage_name = None, **kwargs):  # noqa: E501
         """Copy folder  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1010,15 +1010,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def copy_layout_slide(self, name, clone_from, clone_from_position, clone_from_password = None, clone_from_storage = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Copy layoutSlide from source presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1140,15 +1140,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='LayoutSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def copy_master_slide(self, name, clone_from, clone_from_position, clone_from_password = None, clone_from_storage = None, apply_to_all = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Copy masterSlide from source presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1274,15 +1274,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='MasterSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def copy_slide(self, name, slide_to_copy, position = None, source = None, source_password = None, source_storage = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Copy a slide from the current or another presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1405,15 +1405,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_animation_effect(self, name, slide_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add an effect to slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1526,15 +1526,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_animation_interactive_sequence(self, name, slide_index, sequence, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1647,15 +1647,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_animation_interactive_sequence_effect(self, name, slide_index, sequence_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add an animation effect to a slide interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1774,15 +1774,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_chart_category(self, name, slide_index, shape_index, category, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add a new category to a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -1901,15 +1901,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_chart_data_point(self, name, slide_index, shape_index, series_index, data_point, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add a new data point to a chart series.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2034,15 +2034,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_chart_series(self, name, slide_index, shape_index, series, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add a new series to a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2161,15 +2161,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_comment(self, name, slide_index, dto, shape_index = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Adds the comment on the slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2286,15 +2286,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideComments',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_comment_online(self, document, slide_index, dto, shape_index = None, password = None, **kwargs):  # noqa: E501
         """Adds the comment on the slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2404,15 +2404,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_folder(self, path, storage_name = None, **kwargs):  # noqa: E501
         """Create the folder  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2504,15 +2504,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_image_watermark(self, name, image = None, picture_frame = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Adds an image watermark to each slide of the presentation.  Image can be provided as a part of the form or withing PictureFrame DTO for detailed customization. Both options are applicable simultaneously.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2620,15 +2620,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_image_watermark_online(self, document, image = None, picture_frame = None, password = None, **kwargs):  # noqa: E501
         """Adds an image watermark to each slide of the presentation.  Image can be provided as a part of the form or withing PictureFrame DTO for detailed customization. Both options are applicable simultaneously.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2729,15 +2729,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_notes_slide(self, name, slide_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add new notes slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2850,15 +2850,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_paragraph(self, name, slide_index, shape_index, dto, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Creates new paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -2985,15 +2985,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_portion(self, name, slide_index, shape_index, paragraph_index, dto, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Creates new portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3126,15 +3126,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_presentation(self, name, data = None, input_password = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create a presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3242,15 +3242,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_presentation_from_source(self, name, source_path = None, source_password = None, source_storage = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create a presentation from an existing source.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3362,15 +3362,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_presentation_from_template(self, name, template_path, data = None, template_password = None, template_storage = None, is_image_data_embedded = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create a presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3493,15 +3493,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_section(self, name, section_name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create a section starting at a specified slide index.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3615,15 +3615,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_shape(self, name, slide_index, dto = None, shape_to_clone = None, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Create new shape.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3745,15 +3745,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_slide(self, name, layout_alias = None, position = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3861,15 +3861,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_smart_art_node(self, name, slide_index, smart_art_index, sub_node = None, text = None, position = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add SmartArt node  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -3993,15 +3993,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SmartArt',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_animation_effect(self, name, slide_index, slide_type, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add an effect to special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4123,15 +4123,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_animation_interactive_sequence(self, name, slide_index, slide_type, sequence, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4253,15 +4253,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_animation_interactive_sequence_effect(self, name, slide_index, slide_type, sequence_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Add an animation effect to a special slide (master, layout, notes) interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4389,15 +4389,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_paragraph(self, name, slide_index, slide_type, shape_index, dto, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Creates new paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4533,15 +4533,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_portion(self, name, slide_index, slide_type, shape_index, paragraph_index, dto, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Creates new portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4683,15 +4683,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_special_slide_shape(self, name, slide_index, slide_type, dto = None, shape_to_clone = None, position = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Create new shape.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4822,15 +4822,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Creates table cell paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -4961,15 +4961,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Creates table cell portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5106,15 +5106,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_table_row(self, name, slide_index, shape_index, dto, position = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Inserts the table row in the specified position. If position is not specified, the row add to the end of the table.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5237,15 +5237,130 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TableRow',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def create_vba_module(self, name, module_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Append module to VBA project               # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, module_dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_dto VBA module DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.create_vba_module_with_http_info(name, module_dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.create_vba_module_with_http_info(name, module_dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def create_vba_module_with_http_info(self, name, module_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Append module to VBA project               # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.create_vba_module_with_http_info(name, module_dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_dto VBA module DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
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
+                    " to method create_vba_module" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `create_vba_module`")  # noqa: E501
+        # verify the required parameter 'module_dto' is set
+        if not module_dto:
+            raise ValueError("Missing the required parameter `module_dto` when calling `create_vba_module`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
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
+        if module_dto:
+            body_params = module_dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/vbaProject/modules', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='VbaModule',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_watermark(self, name, shape = None, font_height = None, text = None, font_name = None, font_color = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Adds a text watermark to each slide of the presentation. Text watermark can be setup via method arguments or withing Shape DTO for detailed customization. Both options are applicable simultaneously.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5365,15 +5480,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def create_watermark_online(self, document, shape = None, font_height = None, text = None, font_name = None, font_color = None, password = None, **kwargs):  # noqa: E501
         """Adds a text watermark to each slide of the presentation. Text watermark can be setup via method arguments or withing Shape DTO for detailed customization. Both options are applicable simultaneously.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5486,15 +5601,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove animation from a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5600,15 +5715,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation_effect(self, name, slide_index, effect_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an effect from slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5720,15 +5835,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation_interactive_sequence(self, name, slide_index, sequence_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an interactive sequence from slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5840,15 +5955,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation_interactive_sequence_effect(self, name, slide_index, sequence_index, effect_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an effect from slide animation interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -5966,15 +6081,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation_interactive_sequences(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Clear all interactive sequences from slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6080,15 +6195,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_animation_main_sequence(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Clear main sequence in slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6194,15 +6309,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_background(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove background from a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6308,15 +6423,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideBackground',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_chart_category(self, name, slide_index, shape_index, category_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete a category from a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6434,15 +6549,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_chart_data_point(self, name, slide_index, shape_index, series_index, point_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete a data point from a chart series.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6566,15 +6681,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_chart_series(self, name, slide_index, shape_index, series_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete a series from a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6692,15 +6807,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_comments(self, name, author = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes comments of the specified author from the presentation. If author value is not provided all comments will be removed.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6804,15 +6919,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_comments_online(self, document, author = None, password = None, **kwargs):  # noqa: E501
         """Removes comments of the specified author from the presentation. If author value is not provided all comments will be removed.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -6909,15 +7024,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_document_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Clean document properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7017,15 +7132,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_document_property(self, name, property_name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete document property.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7131,15 +7246,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_embedded_font(self, name, font_name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes specified embedded font and returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7245,15 +7360,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_embedded_font_online(self, document, font_name, password = None, **kwargs):  # noqa: E501
         """Removes specified embedded font and returns presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7352,15 +7467,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_file(self, path, storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Delete file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7456,15 +7571,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_folder(self, path, storage_name = None, recursive = None, **kwargs):  # noqa: E501
         """Delete folder  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7560,15 +7675,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_notes_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove notes slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7674,15 +7789,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_paragraph(self, name, slide_index, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7804,15 +7919,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_paragraphs(self, name, slide_index, shape_index, paragraphs = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of paragraphs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -7933,15 +8048,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8069,15 +8184,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_portions(self, name, slide_index, shape_index, paragraph_index, portions = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of portions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8204,15 +8319,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_protection(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Resets all presentation protection settings.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8312,15 +8427,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ProtectionProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_protection_online(self, document, password, **kwargs):  # noqa: E501
         """Resets all presentation protection settings.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8416,15 +8531,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_section(self, name, section_index, with_slides = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete a presentation section.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8534,15 +8649,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_sections(self, name, sections = None, with_slides = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete presentation sections.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8651,15 +8766,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_shape(self, name, slide_index, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a shape.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8775,15 +8890,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_shapes(self, name, slide_index, shapes = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of shapes.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -8898,15 +9013,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete a presentation slide by index.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9012,15 +9127,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_slide_comments(self, name, slide_index, author = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes comments of the specified author from the slide. If author value is not provided all comments will be removed.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9130,15 +9245,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideComments',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_slide_comments_online(self, document, slide_index, author = None, password = None, **kwargs):  # noqa: E501
         """Removes comments of the specified author from the slide. If author value is not provided all comments will be removed.                # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9241,15 +9356,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_slides(self, name, slides = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete presentation slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9354,15 +9469,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_smart_art_node(self, name, slide_index, smart_art_index, node_index, sub_node = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete SmartArt node  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9484,15 +9599,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SmartArt',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation(self, name, slide_index, slide_type, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove animation from a special slide (master, layout, notes).  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9607,15 +9722,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation_effect(self, name, slide_index, slide_type, effect_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an effect from special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9736,15 +9851,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation_interactive_sequence(self, name, slide_index, slide_type, sequence_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an interactive sequence from special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -9865,15 +9980,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation_interactive_sequence_effect(self, name, slide_index, slide_type, sequence_index, effect_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Remove an effect from special slide (master, layout, notes) animation interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10000,15 +10115,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation_interactive_sequences(self, name, slide_index, slide_type, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Clear all interactive sequences from special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10123,15 +10238,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_animation_main_sequence(self, name, slide_index, slide_type, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Clear main sequence in special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10246,15 +10361,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_paragraph(self, name, slide_index, slide_type, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10385,15 +10500,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_paragraphs(self, name, slide_index, slide_type, shape_index, paragraphs = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of paragraphs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10523,15 +10638,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_portion(self, name, slide_index, slide_type, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10668,15 +10783,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_portions(self, name, slide_index, slide_type, shape_index, paragraph_index, portions = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of portions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10812,15 +10927,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_shape(self, name, slide_index, slide_type, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a shape.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -10945,15 +11060,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_special_slide_shapes(self, name, slide_index, slide_type, shapes = None, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a range of shapes.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11077,15 +11192,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete cell paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11215,15 +11330,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Delete table ell portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11359,15 +11474,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_table_row(self, name, slide_index, shape_index, row_index, with_attached_rows = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Deletes the table row.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11489,15 +11604,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Table',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_unused_layout_slides(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes unused layout slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11597,15 +11712,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='LayoutSlides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_unused_layout_slides_online(self, document, password = None, **kwargs):  # noqa: E501
         """Removes unused layout slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11698,15 +11813,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_unused_master_slides(self, name, ignore_preserve_field = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes unused master slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11810,15 +11925,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='MasterSlides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_unused_master_slides_online(self, document, ignore_preserve_field = None, password = None, **kwargs):  # noqa: E501
         """Removes unused master slides.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -11915,15 +12030,129 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def delete_vba_module(self, name, module_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete module from VBA project.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, module_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaProject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.delete_vba_module_with_http_info(name, module_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_vba_module_with_http_info(name, module_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def delete_vba_module_with_http_info(self, name, module_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Delete module from VBA project.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.delete_vba_module_with_http_info(name, module_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaProject
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
+                    " to method delete_vba_module" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `delete_vba_module`")  # noqa: E501
+        # verify the required parameter 'module_index' is set
+        if not module_index:
+            raise ValueError("Missing the required parameter `module_index` when calling `delete_vba_module`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['moduleIndex'] = module_index  # noqa: E501
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
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/vbaProject/modules/{moduleIndex}', 'DELETE',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='VbaProject',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_watermark(self, name, shape_name = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Removes shapes with name \&quot;watermark\&quot; from the presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12027,15 +12256,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def delete_watermark_online(self, document, shape_name = None, password = None, **kwargs):  # noqa: E501
         """Removes shapes with name \&quot;watermark\&quot; from the presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12132,15 +12361,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_file(self, path, storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Download file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12236,15 +12465,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_image(self, name, index, format, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get image in specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12359,15 +12588,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_image_default_format(self, name, index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get image binary data.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12473,15 +12702,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_image_default_format_online(self, document, index, password = None, **kwargs):  # noqa: E501
         """Get image binary data.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12580,15 +12809,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_image_online(self, document, index, format, password = None, **kwargs):  # noqa: E501
         """Get image in specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12696,15 +12925,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_images(self, name, format, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get all presentation images in specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12813,15 +13042,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_images_default_format(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get all presentation images.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -12921,15 +13150,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_images_default_format_online(self, document, password = None, **kwargs):  # noqa: E501
         """Get all presentation images.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13022,15 +13251,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_images_online(self, document, format, password = None, **kwargs):  # noqa: E501
         """Get all presentation images in specified format.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13132,15 +13361,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_notes_slide(self, name, slide_index, format, width = None, height = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Convert notes slide to the specified image format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13267,15 +13496,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_notes_slide_online(self, document, slide_index, format, width = None, height = None, password = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Convert notes slide to the specified image format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13395,15 +13624,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_portion_as_math_ml(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Convert Mathematical Text to MathML Format  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13527,15 +13756,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_presentation(self, name, format, options = None, password = None, folder = None, storage = None, fonts_folder = None, slides = None, **kwargs):  # noqa: E501
         """Save a presentation to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13657,15 +13886,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_shape(self, name, slide_index, shape_index, format, options = None, scale_x = None, scale_y = None, bounds = None, password = None, folder = None, storage = None, fonts_folder = None, sub_shape = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13813,15 +14042,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_shape_from_dto(self, format, dto, **kwargs):  # noqa: E501
         """Creates the shape from the DTO and returns the result in the specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -13919,15 +14148,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_shape_online(self, document, slide_index, shape_index, format, scale_x = None, scale_y = None, bounds = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14068,15 +14297,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_slide(self, name, slide_index, format, options = None, width = None, height = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Save a slide to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14207,15 +14436,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_slide_online(self, document, slide_index, format, width = None, height = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Save a slide to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14343,15 +14572,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def download_special_slide_shape(self, name, slide_index, slide_type, shape_index, format, options = None, scale_x = None, scale_y = None, bounds = None, password = None, folder = None, storage = None, fonts_folder = None, sub_shape = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14508,15 +14737,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_animation(self, name, slide_index, shape_index = None, paragraph_index = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide animation effects.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14630,15 +14859,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_api_info(self, **kwargs):  # noqa: E501
         """Get API info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14720,15 +14949,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ApiInfo',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_background(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide background info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14834,15 +15063,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideBackground',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_color_scheme(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide theme color scheme info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -14948,15 +15177,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ColorScheme',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_disc_usage(self, storage_name = None, **kwargs):  # noqa: E501
         """Get disc usage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15042,15 +15271,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DiscUsage',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_document_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation document properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15150,15 +15379,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_document_property(self, name, property_name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation document property.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15264,15 +15493,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperty',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_file_versions(self, path, storage_name = None, **kwargs):  # noqa: E501
         """Get file versions  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15364,15 +15593,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FileVersions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_files_list(self, path, storage_name = None, **kwargs):  # noqa: E501
         """Get all files and folders within a folder  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15464,15 +15693,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FilesList',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_font_scheme(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide theme font scheme info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15578,15 +15807,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontScheme',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_fonts(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15686,15 +15915,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_fonts_online(self, document, password = None, **kwargs):  # noqa: E501
         """Returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15787,15 +16016,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_format_scheme(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide theme format scheme info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -15901,15 +16130,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FormatScheme',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_layout_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation layoutSlide info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16015,15 +16244,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='LayoutSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_layout_slides(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation layoutSlides info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16123,15 +16352,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='LayoutSlides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_master_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation masterSlide info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16237,15 +16466,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='MasterSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_master_slides(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation masterSlides info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16345,15 +16574,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='MasterSlides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_notes_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read notes slide info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16459,15 +16688,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_notes_slide_header_footer(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get header/footer info for the notes slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16573,15 +16802,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlideHeaderFooter',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_notes_slide_online(self, document, slide_index, password = None, **kwargs):  # noqa: E501
         """Read notes slide info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16680,15 +16909,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_paragraph(self, name, slide_index, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read shape paragraph info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16810,15 +17039,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_paragraph_effective(self, name, slide_index, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read effective paragraph info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -16940,15 +17169,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_paragraph_rectangle(self, name, slide_index, shape_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Return coordinates of rect that bounds paragraph. The rect includes all the lines of text in paragraph, including empty ones.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17066,15 +17295,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TextBounds',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_paragraphs(self, name, slide_index, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read shape paragraphs info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17190,15 +17419,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_placeholder(self, name, slide_index, placeholder_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide placeholder info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17310,15 +17539,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Placeholder',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_placeholders(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide placeholders info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17424,15 +17653,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Placeholders',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read paragraph portion info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17560,15 +17789,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_portion_effective(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read effective portion info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17696,15 +17925,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_portion_rectangle(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Return coordinates of rect that bounds paragraph. The rect includes all the lines of text in paragraph, including empty ones.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17828,15 +18057,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TextBounds',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_portions(self, name, slide_index, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read paragraph portions info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -17958,15 +18187,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_presentation(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18066,15 +18295,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_presentation_images(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation images info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18174,15 +18403,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Images',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_presentation_text_items(self, name, with_empty = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Extract presentation text items.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18286,15 +18515,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TextItems',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_protection_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation protection properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18394,15 +18623,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ProtectionProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_sections(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation sections info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18502,15 +18731,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_shape(self, name, slide_index, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read slide shape info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18626,15 +18855,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_shape_geometry_path(self, name, slide_index, shape_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns geometry path of the shape  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18746,15 +18975,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='GeometryPaths',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_shapes(self, name, slide_index, password = None, folder = None, storage = None, shape_type = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read slide shapes info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18871,15 +19100,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation slide info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -18985,15 +19214,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_comments(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation slide comments.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19099,15 +19328,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideComments',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_header_footer(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get footer info for the slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19213,15 +19442,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='HeaderFooter',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_images(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide images info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19327,15 +19556,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Images',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation slide properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19435,15 +19664,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_show_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation slide show properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19543,15 +19772,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideShowProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slide_text_items(self, name, slide_index, with_empty = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Extract slide text items.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19661,15 +19890,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TextItems',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_slides(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation slides info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19769,15 +19998,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_animation(self, name, slide_index, slide_type, shape_index = None, paragraph_index = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read special slide (master, layout, notes) animation effects.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -19900,15 +20129,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_paragraph(self, name, slide_index, slide_type, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read shape paragraph info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20039,15 +20268,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_paragraphs(self, name, slide_index, slide_type, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read special shape paragraphs info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20172,15 +20401,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_portion(self, name, slide_index, slide_type, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read paragraph portion info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20317,15 +20546,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_portions(self, name, slide_index, slide_type, shape_index, paragraph_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read paragraph portions info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20456,15 +20685,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_shape(self, name, slide_index, slide_type, shape_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read special slide shape info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20589,15 +20818,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_special_slide_shapes(self, name, slide_index, slide_type, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Read special slide shapes info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20716,15 +20945,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns paragraph info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20854,15 +21083,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_table_cell_paragraphs(self, name, slide_index, shape_index, row_index, cell_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns table cell paragraphs.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -20986,15 +21215,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraphs',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns table cell portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21130,15 +21359,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_table_cell_portions(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Returns table cell portions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21268,15 +21497,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portions',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_theme(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read slide theme info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21382,15 +21611,237 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Theme',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_vba_module(self, name, module_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Get VBA module info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, module_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_vba_module_with_http_info(name, module_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_vba_module_with_http_info(name, module_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_vba_module_with_http_info(self, name, module_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Get VBA module info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_vba_module_with_http_info(name, module_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
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
+                    " to method get_vba_module" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_vba_module`")  # noqa: E501
+        # verify the required parameter 'module_index' is set
+        if not module_index:
+            raise ValueError("Missing the required parameter `module_index` when calling `get_vba_module`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['moduleIndex'] = module_index  # noqa: E501
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
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/vbaProject/modules/{moduleIndex}', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='VbaModule',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def get_vba_project(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Get VBA project info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaProject
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.get_vba_project_with_http_info(name, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.get_vba_project_with_http_info(name, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def get_vba_project_with_http_info(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Get VBA project info.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.get_vba_project_with_http_info(name, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaProject
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
+                    " to method get_vba_project" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `get_vba_project`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
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
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/vbaProject', 'GET',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='VbaProject',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def get_view_properties(self, name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Read presentation view properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21490,15 +21941,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ViewProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def highlight_shape_regex(self, name, slide_index, shape_index, regex, color, whole_words_only = None, ignore_case = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Highlight all matches of sample in text frame text using specified color.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21632,15 +22083,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shape',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def highlight_shape_text(self, name, slide_index, shape_index, text, color, whole_words_only = None, ignore_case = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Highlight all matches of sample in text frame text using specified color.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21774,15 +22225,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shape',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def import_from_html(self, name, html = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create presentation document from html.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -21886,15 +22337,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def import_from_pdf(self, name, pdf, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create presentation document from pdf or append pdf to an existing presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22001,15 +22452,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def import_shapes_from_svg(self, name, slide_index, image = None, x = None, y = None, width = None, height = None, shapes = None, group = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Imports shapes from SVG file.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22144,15 +22595,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Shapes',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def merge(self, name, request, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Merge the presentation with other presentations specified in the request parameter.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22259,15 +22710,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def merge_and_save_online(self, out_path, files = None, request = None, storage = None, **kwargs):  # noqa: E501
         """Merges presentations or some of their slides specified in the request parameter. Result will be save in the storage.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22367,15 +22818,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def merge_online(self, files = None, request = None, storage = None, **kwargs):  # noqa: E501
         """Merges presentations or some of their slides specified in the request parameter. Returns result file in the response.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22468,15 +22919,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def merge_table_cells(self, name, slide_index, shape_index, table_cell_merge_options, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Merge table cells.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22595,15 +23046,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Table',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def move_file(self, src_path, dest_path, src_storage_name = None, dest_storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Move file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22710,15 +23161,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def move_folder(self, src_path, dest_path, src_storage_name = None, dest_storage_name = None, **kwargs):  # noqa: E501
         """Move folder  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22821,15 +23272,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def move_section(self, name, section_index, new_position, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Move presentation section to a specified position.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -22942,15 +23393,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def move_slide(self, name, slide_index, new_position, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Reorder presentation slide position.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23063,15 +23514,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def notes_slide_exists(self, name, slide_index, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Get info whether a notes slide exists.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23177,15 +23628,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='EntityExists',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def notes_slide_exists_online(self, document, slide_index, password = None, **kwargs):  # noqa: E501
         """Get info whether a notes slide exists.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23284,15 +23735,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='EntityExists',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def object_exists(self, path, storage_name = None, version_id = None, **kwargs):  # noqa: E501
         """Check if file or folder exists  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23388,15 +23839,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ObjectExist',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def ordered_merge(self, name, request, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Merge the presentation with other presentations or some of their slides specified in the request parameter.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23503,15 +23954,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def pipeline(self, pipeline, files = None, **kwargs):  # noqa: E501
         """Performs slides pipeline.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23603,15 +24054,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def reorder_slides(self, name, old_positions = None, new_positions = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Reorder presentation slides positions.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23721,15 +24172,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slides',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_font(self, name, source_font, target_font, embed = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Replaces specified font and returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23849,15 +24300,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_font_online(self, document, source_font, target_font, embed = None, password = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Replaces specified font and returns presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -23970,15 +24421,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_presentation_text(self, name, old_value, new_value, ignore_case = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Replace text with a new value.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24096,15 +24547,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentReplaceResult',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_presentation_text_online(self, document, old_value, new_value, ignore_case = None, password = None, **kwargs):  # noqa: E501
         """Replace text with a new value.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24215,15 +24666,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_slide_text(self, name, slide_index, old_value, new_value, ignore_case = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Replace text with a new value.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24347,15 +24798,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideReplaceResult',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def replace_slide_text_online(self, document, slide_index, old_value, new_value, ignore_case = None, password = None, **kwargs):  # noqa: E501
         """Replace slide text with a new value.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24472,15 +24923,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_portion_as_math_ml(self, name, slide_index, shape_index, paragraph_index, portion_index, out_path, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Convert Mathematical Text to MathML Format and saves result to the storage  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24611,15 +25062,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_presentation(self, name, format, out_path, options = None, password = None, folder = None, storage = None, fonts_folder = None, slides = None, **kwargs):  # noqa: E501
         """Save a presentation to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24748,15 +25199,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_shape(self, name, slide_index, shape_index, format, out_path, options = None, scale_x = None, scale_y = None, bounds = None, password = None, folder = None, storage = None, fonts_folder = None, sub_shape = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -24911,15 +25362,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_shape_online(self, document, slide_index, shape_index, format, out_path, scale_x = None, scale_y = None, bounds = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25067,15 +25518,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_slide(self, name, slide_index, format, out_path, options = None, width = None, height = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Save a slide to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25213,15 +25664,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_slide_online(self, document, slide_index, format, out_path, width = None, height = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Save a slide to a specified format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25356,15 +25807,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def save_special_slide_shape(self, name, slide_index, slide_type, shape_index, format, out_path, options = None, scale_x = None, scale_y = None, bounds = None, password = None, folder = None, storage = None, fonts_folder = None, sub_shape = None, **kwargs):  # noqa: E501
         """Render shape to specified picture format.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25528,15 +25979,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type=None,  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_animation(self, name, slide_index, animation, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set slide animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25649,15 +26100,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_background(self, name, slide_index, background, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set background for a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25770,15 +26221,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideBackground',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_background_color(self, name, slide_index, color, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set background color for a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -25891,15 +26342,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideBackground',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_chart_axis(self, name, slide_index, shape_index, axis_type, axis, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set chart axis.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26027,15 +26478,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Axis',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_chart_legend(self, name, slide_index, shape_index, legend, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set chart axis.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26154,15 +26605,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Legend',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_chart_series_group(self, name, slide_index, shape_index, series_group_index, series_group, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set a series group in a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26287,15 +26738,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_chart_wall(self, name, slide_index, shape_index, chart_wall_type, chart_wall, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set 3D chart wall.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26423,15 +26874,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ChartWall',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_document_properties(self, name, properties, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set document properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26538,15 +26989,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_document_property(self, name, property_name, _property, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set document property.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26659,15 +27110,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='DocumentProperty',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_embedded_font(self, name, font_name, only_used = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Embeds specified font and returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26781,15 +27232,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_embedded_font_from_request(self, font, name, only_used = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Embeds font from request and returns presentation fonts info.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -26900,15 +27351,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FontsData',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_embedded_font_from_request_online(self, document, font, only_used = None, password = None, **kwargs):  # noqa: E501
         """Embeds font from request and returns presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27012,15 +27463,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_embedded_font_online(self, document, font_name, only_used = None, password = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Embeds specified font and returns presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27127,15 +27578,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_notes_slide_header_footer(self, name, slide_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set header/footer the notes slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27248,15 +27699,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlideHeaderFooter',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_presentation_header_footer(self, name, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set footers for all slides in a presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27363,15 +27814,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Document',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_protection(self, name, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Updates presentation protection properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27478,15 +27929,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ProtectionProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_protection_online(self, document, dto, password = None, **kwargs):  # noqa: E501
         """Sets presentation protection options.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27586,15 +28037,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_sections(self, name, sections, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Replace existing presentation sections with the ones provided in the sections DTO.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27701,15 +28152,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_shape_geometry_path(self, name, slide_index, shape_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Sets geometry path to the shape  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27828,15 +28279,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_slide_header_footer(self, name, slide_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set footer the slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -27949,15 +28400,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='HeaderFooter',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_slide_properties(self, name, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update presentation slide properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28064,15 +28515,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_slide_show_properties(self, name, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update presentation slide show properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28179,15 +28630,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideShowProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_special_slide_animation(self, name, slide_index, slide_type, animation, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Set special slide (master, layout, notes) animation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28309,15 +28760,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def set_view_properties(self, name, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update presentation view properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28424,15 +28875,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ViewProperties',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def split(self, name, options = None, format = None, width = None, height = None, _from = None, to = None, dest_folder = None, password = None, folder = None, storage = None, fonts_folder = None, **kwargs):  # noqa: E501
         """Splitting presentations. Create one image per slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28567,15 +29018,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SplitDocumentResult',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def split_and_save_online(self, document, format, dest_folder = None, width = None, height = None, _from = None, to = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Splits PowerPoint presentation slides from the specified range into separate files and exports them in the specified file format. If the range is not provided all slides will be processed.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28709,15 +29160,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SplitDocumentResult',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def split_online(self, document, format, width = None, height = None, _from = None, to = None, password = None, storage = None, fonts_folder = None, options = None, **kwargs):  # noqa: E501
         """Splits PowerPoint presentation slides from the specified range into separate files and exports them in the specified file format. If the range is not provided all slides will be processed.   # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28847,15 +29298,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='file',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def split_table_cell(self, name, slide_index, shape_index, row_index, cell_index, split_type, value, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Split table cell.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -28994,15 +29445,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Table',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def storage_exists(self, storage_name, **kwargs):  # noqa: E501
         """Check if storage exists  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29090,15 +29541,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='StorageExist',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_animation_effect(self, name, slide_index, effect_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Modify an animation effect for a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29217,15 +29668,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_animation_interactive_sequence_effect(self, name, slide_index, sequence_index, effect_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Modify an animation effect for a slide interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29350,15 +29801,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_chart_category(self, name, slide_index, shape_index, category_index, category, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update a chart category.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29483,15 +29934,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_chart_data_point(self, name, slide_index, shape_index, series_index, point_index, data_point, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update a data point in a chart series.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29622,15 +30073,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_chart_series(self, name, slide_index, shape_index, series_index, series, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update a series in a chart.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29755,15 +30206,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Chart',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_layout_slide(self, name, slide_index, slide_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update a layoutSlide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29876,15 +30327,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='LayoutSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_notes_slide(self, name, slide_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update notes slide properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -29997,15 +30448,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='NotesSlide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_paragraph(self, name, slide_index, shape_index, paragraph_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update paragraph properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30134,15 +30585,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update portion properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30277,15 +30728,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_section(self, name, section_index, section_name, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update section name.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30398,15 +30849,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Sections',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_shape(self, name, slide_index, shape_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update shape properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30529,15 +30980,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_slide(self, name, slide_index, slide_dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update a slide.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30650,15 +31101,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Slide',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_special_slide_animation_effect(self, name, slide_index, slide_type, effect_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Modify an animation effect for a special slide (master, layout, notes).  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30786,15 +31237,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_special_slide_animation_interactive_sequence_effect(self, name, slide_index, slide_type, sequence_index, effect_index, effect, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Modify an animation effect for a special slide (master, layout, notes) interactive sequence.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -30928,15 +31379,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='SlideAnimation',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_special_slide_paragraph(self, name, slide_index, slide_type, shape_index, paragraph_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update paragraph properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31074,15 +31525,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_special_slide_portion(self, name, slide_index, slide_type, shape_index, paragraph_index, portion_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update portion properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31226,15 +31677,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_special_slide_shape(self, name, slide_index, slide_type, shape_index, dto, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Update shape properties.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31366,15 +31817,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='ShapeBase',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_table_cell(self, name, slide_index, shape_index, row_index, cell_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update the table cell.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31505,15 +31956,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TableCell',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_table_cell_paragraph(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Updates table cell paragraph.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31650,15 +32101,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Paragraph',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_table_cell_portion(self, name, slide_index, shape_index, row_index, cell_index, paragraph_index, portion_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Updates table cell portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31801,15 +32252,15 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='Portion',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def update_table_row(self, name, slide_index, shape_index, row_index, dto, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Update the table row.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -31934,15 +32385,133 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='TableRow',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def update_vba_module(self, name, module_index, module_dto = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update VBA module.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, module_index, module_dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param module_dto VBA module DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def update_vba_module_with_http_info(self, name, module_index, module_dto = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+        """Update VBA module.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.update_vba_module_with_http_info(name, module_index, module_dto, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param module_index The index of the macros module to remove.
+        :param module_dto VBA module DTO.
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Document storage.
+        :return: VbaModule
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
+                    " to method update_vba_module" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `update_vba_module`")  # noqa: E501
+        # verify the required parameter 'module_index' is set
+        if not module_index:
+            raise ValueError("Missing the required parameter `module_index` when calling `update_vba_module`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['moduleIndex'] = module_index  # noqa: E501
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
+        if module_dto:
+            body_params = module_dto
+
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/vbaProject/modules/{moduleIndex}', 'PUT',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=param_files,
+            response_type='VbaModule',  # noqa: E501
+            auth_settings=auth_settings,
+            is_async=params.get('is_async'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
     def upload_file(self, path, file, storage_name = None, **kwargs):  # noqa: E501
         """Upload file  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
@@ -32041,10 +32610,10 @@
             body=body_params,
             post_params=form_params,
             files=param_files,
             response_type='FilesUploadResult',  # noqa: E501
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
-            _preload_content=params.get('_preload_content', True),
+            _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/configuration.py` & `asposeslidescloud-23.6.0/asposeslidescloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 23.4.0".\
+               "SDK Package Version: 23.6.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/error_message.py` & `asposeslidescloud-23.6.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,17 @@
 from asposeslidescloud.models.text_items import TextItems
 from asposeslidescloud.models.theme import Theme
 from asposeslidescloud.models.three_d_format import ThreeDFormat
 from asposeslidescloud.models.tiff_export_options import TiffExportOptions
 from asposeslidescloud.models.tint_effect import TintEffect
 from asposeslidescloud.models.update_background import UpdateBackground
 from asposeslidescloud.models.update_shape import UpdateShape
+from asposeslidescloud.models.vba_module import VbaModule
+from asposeslidescloud.models.vba_project import VbaProject
+from asposeslidescloud.models.vba_reference import VbaReference
 from asposeslidescloud.models.video_export_options import VideoExportOptions
 from asposeslidescloud.models.video_frame import VideoFrame
 from asposeslidescloud.models.view_properties import ViewProperties
 from asposeslidescloud.models.workbook import Workbook
 from asposeslidescloud.models.xy_series import XYSeries
 from asposeslidescloud.models.xaml_export_options import XamlExportOptions
 from asposeslidescloud.models.xps_export_options import XpsExportOptions
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/audio_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_title.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/connector.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/document.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/error.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/geometry_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/graphical_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/html5_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/html_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/image.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/images.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/input.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/path_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/pdf_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/pdf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/picture_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/portions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/save.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/save.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/save_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/section.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/series.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_base.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_merge_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_merge_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table_cell_split_type.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table_cell_split_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/task.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/text_items.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/tiff_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/tiff_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/video_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-23.6.0/asposeslidescloud/models/zoom_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-23.6.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud/rest.py` & `asposeslidescloud-23.6.0/asposeslidescloud/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,18 @@
 
 class ApiException(Exception):
 
     def __init__(self, status=None, reason=None, http_resp=None):
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
-            self.body = http_resp.data
+            try:
+                self.body = http_resp.data
+            except:
+                self.body = None
             self.headers = http_resp.getheaders()
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-23.6.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 23.4.0
+Version: 23.6.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,18 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 23.6
+
+* Added methods ho handle VBA methods: **GetVbaProject**, **GetVbaModule**, **CreateVbaModule**, **UpdateVbaModule** and **DeleteVbaModule**. Added model classes related to VBA: **VbaProject**,  **VbaModule** and  **VbaReference**.
+
 ## Enhancements in Version 23.4
 
 * Added **CreateTableRow**, **UpdateTableRow** and **DeleteTableRow** methods to add, update and delete table rows.
 * Added **UpdateTableCell** method to update table cells.
 * Added  **MergeTableCells** and **SplitTableCell** methods to merge &amp; split table cells.
 * Added methods to get, add, modify and delete paragraphs & portions within table cells: **GetTableCellParagraph**, **GetTableCellParagraphs**, **GetTableCellPortion**, **GetTableCellPortions**, **CreateTableCellParagraph**, **CreateTableCellPortion**, **UpdateTableCellPortion**, **UpdateTableCellParagraph**, **DeleteTableCellParagraph**,  **DeleteTableCellPortion**.
 * New **TextFrameFormat** property in **TableCell** class allows to specify text format for table cells.
```

### Comparing `asposeslidescloud-23.4.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-23.6.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,17 @@
 asposeslidescloud/models/text_items.py
 asposeslidescloud/models/theme.py
 asposeslidescloud/models/three_d_format.py
 asposeslidescloud/models/tiff_export_options.py
 asposeslidescloud/models/tint_effect.py
 asposeslidescloud/models/update_background.py
 asposeslidescloud/models/update_shape.py
+asposeslidescloud/models/vba_module.py
+asposeslidescloud/models/vba_project.py
+asposeslidescloud/models/vba_reference.py
 asposeslidescloud/models/video_export_options.py
 asposeslidescloud/models/video_frame.py
 asposeslidescloud/models/view_properties.py
 asposeslidescloud/models/workbook.py
 asposeslidescloud/models/xaml_export_options.py
 asposeslidescloud/models/xps_export_options.py
 asposeslidescloud/models/xy_series.py
```

### Comparing `asposeslidescloud-23.4.0/setup.py` & `asposeslidescloud-23.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="23.4.0",
+    version="23.6.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

