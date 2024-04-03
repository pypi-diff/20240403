# Comparing `tmp/asposeslidescloud-24.2.0.tar.gz` & `tmp/asposeslidescloud-24.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-24.2.0.tar", last modified: Fri Feb 23 12:49:15 2024, max compression
+gzip compressed data, was "dist/asposeslidescloud-24.3.0.tar", last modified: Wed Mar 27 23:58:14 2024, max compression
```

## Comparing `asposeslidescloud-24.2.0.tar` & `asposeslidescloud-24.3.0.tar`

### file list

```diff
@@ -1,279 +1,282 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:49:15.000000 asposeslidescloud-24.2.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2024-02-23 12:48:43.000000 asposeslidescloud-24.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6500 2024-02-23 12:49:15.000000 asposeslidescloud-24.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6112 2024-02-23 12:48:47.000000 asposeslidescloud-24.2.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    18660 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27782 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      313 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1433577 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)    37269 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/apis/slides_async_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:49:15.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    18376 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    18977 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6280 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19140 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     4661 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/comment_author.py
--rw-rw-r--   0 root         (0) root         (0)     4362 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/comment_authors.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9725 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8034 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    29539 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3772 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5671 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)     9958 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5294 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6003 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5966 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    20135 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    11286 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14248 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7722 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)    11732 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/operation.py
--rw-rw-r--   0 root         (0) root         (0)     5643 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/operation_progress.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    28850 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6348 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6404 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8656 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7370 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6868 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7749 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    17369 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    13365 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3751 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5587 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    12171 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)    36756 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slide_show_transition.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)    15341 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5385 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7774 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7607 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15954 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    22416 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     7735 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell_merge_options.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell_split_type.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    17671 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/vba_module.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/vba_project.py
--rw-rw-r--   0 root         (0) root         (0)     4613 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/vba_reference.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15752 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10460 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15494 2024-02-23 12:48:38.000000 asposeslidescloud-24.2.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6500 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11634 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-02-23 12:49:14.000000 asposeslidescloud-24.2.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-23 12:49:15.000000 asposeslidescloud-24.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2024-02-23 12:48:56.000000 asposeslidescloud-24.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-03-27 23:57:53.000000 asposeslidescloud-24.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7331 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6943 2024-03-27 23:57:56.000000 asposeslidescloud-24.3.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    18926 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27782 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      313 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1439127 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)    37269 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_async_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    18642 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    19086 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6280 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    19249 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     4726 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     4661 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/comment_author.py
+-rw-rw-r--   0 root         (0) root         (0)     4362 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/comment_authors.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9834 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8034 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    31358 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3786 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5671 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)    10067 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5403 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6112 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8469 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/handout_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     8010 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    13883 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     6289 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    11264 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_comments_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14357 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7722 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)    11732 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/operation.py
+-rw-rw-r--   0 root         (0) root         (0)     5643 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/operation_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    22614 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6410 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8662 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7370 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6977 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7858 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    18243 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    13365 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3765 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5587 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    13162 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    36756 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_transition.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4908 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/slides_layout_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15450 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5494 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7883 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7716 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    16063 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    13912 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_module.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_project.py
+-rw-rw-r--   0 root         (0) root         (0)     4613 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/vba_reference.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15861 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10569 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15494 2024-03-27 23:57:48.000000 asposeslidescloud-24.3.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7331 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11799 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-27 23:58:14.000000 asposeslidescloud-24.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2024-03-27 23:58:02.000000 asposeslidescloud-24.3.0/setup.py
```

### Comparing `asposeslidescloud-24.2.0/LICENSE` & `asposeslidescloud-24.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/PKG-INFO` & `asposeslidescloud-24.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 24.2.0
+Version: 24.3.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,27 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.3
+
+* Added Markdown (**Md**) to the list of allowed export formats.
+* Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
+* Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
+* Added **AnimateTextType** enum property to **Effect** class.
+* Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
+* Added **BwConversionMode** property to **TiffExportOptions** class.
+* Added **EmbedImages** boolean property to **Html5ExportOptions** class.
+* Added **ShowMediaControls** boolean property to **SlideShowProperties** class.
+* Added **IsDecorative** boolean property to **ShapeBase** class.
+
+
 ## Enhancements in Version 24.2
 
 * Added **GetCommentAuthors** method to get list of comment authors.
 
 ## Enhancements in Version 24.1
 
 * Added **GetAvailableFonts** method to get list of installed system & custom fonts.
```

### Comparing `asposeslidescloud-24.2.0/README` & `asposeslidescloud-24.3.0/README`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,27 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.3
+
+* Added Markdown (**Md**) to the list of allowed export formats.
+* Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
+* Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
+* Added **AnimateTextType** enum property to **Effect** class.
+* Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
+* Added **BwConversionMode** property to **TiffExportOptions** class.
+* Added **EmbedImages** boolean property to **Html5ExportOptions** class.
+* Added **ShowMediaControls** boolean property to **SlideShowProperties** class.
+* Added **IsDecorative** boolean property to **ShapeBase** class.
+
+
 ## Enhancements in Version 24.2
 
 * Added **GetCommentAuthors** method to get list of comment authors.
 
 ## Enhancements in Version 24.1
 
 * Added **GetAvailableFonts** method to get list of installed system & custom fonts.
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/__init__.py` & `asposeslidescloud-24.3.0/asposeslidescloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 from asposeslidescloud.models.glow_effect import GlowEffect
 from asposeslidescloud.models.gradient_fill import GradientFill
 from asposeslidescloud.models.gradient_fill_stop import GradientFillStop
 from asposeslidescloud.models.graphical_object import GraphicalObject
 from asposeslidescloud.models.gray_scale_effect import GrayScaleEffect
 from asposeslidescloud.models.group_shape import GroupShape
 from asposeslidescloud.models.grouping_character_element import GroupingCharacterElement
+from asposeslidescloud.models.handout_layouting_options import HandoutLayoutingOptions
 from asposeslidescloud.models.header_footer import HeaderFooter
 from asposeslidescloud.models.hsl_effect import HslEffect
 from asposeslidescloud.models.html5_export_options import Html5ExportOptions
 from asposeslidescloud.models.html_export_options import HtmlExportOptions
 from asposeslidescloud.models.hyperlink import Hyperlink
 from asposeslidescloud.models.i_shape_export_options import IShapeExportOptions
 from asposeslidescloud.models.image import Image
@@ -162,14 +163,15 @@
 from asposeslidescloud.models.matrix_element import MatrixElement
 from asposeslidescloud.models.merge import Merge
 from asposeslidescloud.models.merging_source import MergingSource
 from asposeslidescloud.models.move_to_path_segment import MoveToPathSegment
 from asposeslidescloud.models.nary_operator_element import NaryOperatorElement
 from asposeslidescloud.models.no_fill import NoFill
 from asposeslidescloud.models.normal_view_restored_properties import NormalViewRestoredProperties
+from asposeslidescloud.models.notes_comments_layouting_options import NotesCommentsLayoutingOptions
 from asposeslidescloud.models.notes_slide import NotesSlide
 from asposeslidescloud.models.notes_slide_export_format import NotesSlideExportFormat
 from asposeslidescloud.models.notes_slide_header_footer import NotesSlideHeaderFooter
 from asposeslidescloud.models.object_exist import ObjectExist
 from asposeslidescloud.models.ole_object_frame import OleObjectFrame
 from asposeslidescloud.models.one_value_chart_data_point import OneValueChartDataPoint
 from asposeslidescloud.models.one_value_series import OneValueSeries
@@ -241,14 +243,15 @@
 from asposeslidescloud.models.slide_export_format import SlideExportFormat
 from asposeslidescloud.models.slide_modern_comment import SlideModernComment
 from asposeslidescloud.models.slide_properties import SlideProperties
 from asposeslidescloud.models.slide_replace_result import SlideReplaceResult
 from asposeslidescloud.models.slide_show_properties import SlideShowProperties
 from asposeslidescloud.models.slide_show_transition import SlideShowTransition
 from asposeslidescloud.models.slides import Slides
+from asposeslidescloud.models.slides_layout_options import SlidesLayoutOptions
 from asposeslidescloud.models.smart_art import SmartArt
 from asposeslidescloud.models.smart_art_node import SmartArtNode
 from asposeslidescloud.models.smart_art_shape import SmartArtShape
 from asposeslidescloud.models.soft_edge_effect import SoftEdgeEffect
 from asposeslidescloud.models.solid_fill import SolidFill
 from asposeslidescloud.models.special_slide_type import SpecialSlideType
 from asposeslidescloud.models.split_document_result import SplitDocumentResult
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/api_client.py` & `asposeslidescloud-24.3.0/asposeslidescloud/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v24.2.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v24.3.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-24.3.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -7795,14 +7795,136 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
+    def delete_picture_cropped_areas(self, name, slide_index, shape_index, password, folder, storage = None, **kwargs):  # noqa: E501
+        """Deletes cropped areas of a pictire.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.(name, slide_index, shape_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index (must refer to a picture frame).
+        :param password Document password.
+        :param folder Document folder.
+        :param storage Presentation storage.
+        :return: None
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('is_async'):
+            return self.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, **kwargs)  # noqa: E501
+        else:
+            (data) = self.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, **kwargs)  # noqa: E501
+            return data
+
+    def delete_picture_cropped_areas_with_http_info(self, name, slide_index, shape_index, password, folder, storage = None, **kwargs):  # noqa: E501
+        """Deletes cropped areas of a pictire.  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass is_async=True
+        >>> thread = api.delete_picture_cropped_areas_with_http_info(name, slide_index, shape_index, password, folder, storage, is_async=True)
+        >>> result = thread.get()
+
+        :param is_async bool
+        :param name Document name.
+        :param slide_index Slide index.
+        :param shape_index Shape index (must refer to a picture frame).
+        :param password Document password.
+        :param folder Document folder.
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
+                    " to method delete_picture_cropped_areas" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'name' is set
+        if not name:
+            raise ValueError("Missing the required parameter `name` when calling `delete_picture_cropped_areas`")  # noqa: E501
+        # verify the required parameter 'slide_index' is set
+        if not slide_index:
+            raise ValueError("Missing the required parameter `slide_index` when calling `delete_picture_cropped_areas`")  # noqa: E501
+        # verify the required parameter 'shape_index' is set
+        if not shape_index:
+            raise ValueError("Missing the required parameter `shape_index` when calling `delete_picture_cropped_areas`")  # noqa: E501
+        # verify the required parameter 'password' is set
+        if not password:
+            raise ValueError("Missing the required parameter `password` when calling `delete_picture_cropped_areas`")  # noqa: E501
+        # verify the required parameter 'folder' is set
+        if not folder:
+            raise ValueError("Missing the required parameter `folder` when calling `delete_picture_cropped_areas`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+        path_params['name'] = name  # noqa: E501
+        path_params['slideIndex'] = slide_index  # noqa: E501
+        path_params['shapeIndex'] = shape_index  # noqa: E501
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
+            ['multipart/form-data'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['JWT']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/slides/{name}/slides/{slideIndex}/shapes/{shapeIndex}/pictureCroppedAreas', 'DELETE',
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
     def delete_portion(self, name, slide_index, shape_index, paragraph_index, portion_index, password = None, folder = None, storage = None, sub_shape = None, **kwargs):  # noqa: E501
         """Remove a portion.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
         >>> thread = api.(name, slide_index, shape_index, paragraph_index, portion_index, password, folder, storage, sub_shape, is_async=True)
         >>> result = thread.get()
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/apis/slides_async_api.py` & `asposeslidescloud-24.3.0/asposeslidescloud/apis/slides_async_api.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/configuration.py` & `asposeslidescloud-24.3.0/asposeslidescloud/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 24.2.0".\
+               "SDK Package Version: 24.3.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/error_message.py` & `asposeslidescloud-24.3.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 from asposeslidescloud.models.glow_effect import GlowEffect
 from asposeslidescloud.models.gradient_fill import GradientFill
 from asposeslidescloud.models.gradient_fill_stop import GradientFillStop
 from asposeslidescloud.models.graphical_object import GraphicalObject
 from asposeslidescloud.models.gray_scale_effect import GrayScaleEffect
 from asposeslidescloud.models.group_shape import GroupShape
 from asposeslidescloud.models.grouping_character_element import GroupingCharacterElement
+from asposeslidescloud.models.handout_layouting_options import HandoutLayoutingOptions
 from asposeslidescloud.models.header_footer import HeaderFooter
 from asposeslidescloud.models.hsl_effect import HslEffect
 from asposeslidescloud.models.html5_export_options import Html5ExportOptions
 from asposeslidescloud.models.html_export_options import HtmlExportOptions
 from asposeslidescloud.models.hyperlink import Hyperlink
 from asposeslidescloud.models.i_shape_export_options import IShapeExportOptions
 from asposeslidescloud.models.image import Image
@@ -154,14 +155,15 @@
 from asposeslidescloud.models.matrix_element import MatrixElement
 from asposeslidescloud.models.merge import Merge
 from asposeslidescloud.models.merging_source import MergingSource
 from asposeslidescloud.models.move_to_path_segment import MoveToPathSegment
 from asposeslidescloud.models.nary_operator_element import NaryOperatorElement
 from asposeslidescloud.models.no_fill import NoFill
 from asposeslidescloud.models.normal_view_restored_properties import NormalViewRestoredProperties
+from asposeslidescloud.models.notes_comments_layouting_options import NotesCommentsLayoutingOptions
 from asposeslidescloud.models.notes_slide import NotesSlide
 from asposeslidescloud.models.notes_slide_export_format import NotesSlideExportFormat
 from asposeslidescloud.models.notes_slide_header_footer import NotesSlideHeaderFooter
 from asposeslidescloud.models.object_exist import ObjectExist
 from asposeslidescloud.models.ole_object_frame import OleObjectFrame
 from asposeslidescloud.models.one_value_chart_data_point import OneValueChartDataPoint
 from asposeslidescloud.models.one_value_series import OneValueSeries
@@ -233,14 +235,15 @@
 from asposeslidescloud.models.slide_export_format import SlideExportFormat
 from asposeslidescloud.models.slide_modern_comment import SlideModernComment
 from asposeslidescloud.models.slide_properties import SlideProperties
 from asposeslidescloud.models.slide_replace_result import SlideReplaceResult
 from asposeslidescloud.models.slide_show_properties import SlideShowProperties
 from asposeslidescloud.models.slide_show_transition import SlideShowTransition
 from asposeslidescloud.models.slides import Slides
+from asposeslidescloud.models.slides_layout_options import SlidesLayoutOptions
 from asposeslidescloud.models.smart_art import SmartArt
 from asposeslidescloud.models.smart_art_node import SmartArtNode
 from asposeslidescloud.models.smart_art_shape import SmartArtShape
 from asposeslidescloud.models.soft_edge_effect import SoftEdgeEffect
 from asposeslidescloud.models.solid_fill import SolidFill
 from asposeslidescloud.models.special_slide_type import SpecialSlideType
 from asposeslidescloud.models.split_document_result import SplitDocumentResult
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/audio_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -82,14 +83,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -112,17 +114,17 @@
         'picture_fill_format': 'pictureFillFormat'
     }
 
     type_determiners = {
         'type': 'AudioFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='AudioFrame', shape_type=None, audio_cd_end_track=None, audio_cd_end_track_time=None, audio_cd_start_track=None, audio_cd_start_track_time=None, embedded=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, volume=None, base64_data=None, play_across_slides=None, rewind_audio=None, picture_fill_format=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='AudioFrame', shape_type=None, audio_cd_end_track=None, audio_cd_end_track_time=None, audio_cd_start_track=None, audio_cd_start_track_time=None, embedded=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, volume=None, base64_data=None, play_across_slides=None, rewind_audio=None, picture_fill_format=None):  # noqa: E501
         """AudioFrame - a model defined in Swagger"""  # noqa: E501
-        super(AudioFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(AudioFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._audio_cd_end_track = None
         self._audio_cd_end_track_time = None
         self._audio_cd_start_track = None
         self._audio_cd_start_track_time = None
         self._embedded = None
         self._hide_at_showing = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/axis.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -82,14 +83,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -112,17 +114,17 @@
         'series_groups': 'seriesGroups'
     }
 
     type_determiners = {
         'type': 'Chart',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Chart', chart_type=None, show_data_labels_over_maximum=None, series=None, categories=None, data_source_for_categories=None, title=None, back_wall=None, side_wall=None, floor=None, legend=None, axes=None, plot_area=None, has_rounded_corners=None, series_groups=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Chart', chart_type=None, show_data_labels_over_maximum=None, series=None, categories=None, data_source_for_categories=None, title=None, back_wall=None, side_wall=None, floor=None, legend=None, axes=None, plot_area=None, has_rounded_corners=None, series_groups=None):  # noqa: E501
         """Chart - a model defined in Swagger"""  # noqa: E501
-        super(Chart, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(Chart, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._chart_type = None
         self._show_data_labels_over_maximum = None
         self._series = None
         self._categories = None
         self._data_source_for_categories = None
         self._title = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_title.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/comment_author.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/comment_author.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/comment_authors.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/comment_authors.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -73,14 +74,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -94,17 +96,17 @@
         'end_shape_connected_to_index': 'endShapeConnectedToIndex'
     }
 
     type_determiners = {
         'type': 'Connector',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Connector', shape_type=None, start_shape_connected_to=None, start_shape_connected_to_index=None, end_shape_connected_to=None, end_shape_connected_to_index=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Connector', shape_type=None, start_shape_connected_to=None, start_shape_connected_to_index=None, end_shape_connected_to=None, end_shape_connected_to_index=None):  # noqa: E501
         """Connector - a model defined in Swagger"""  # noqa: E501
-        super(Connector, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(Connector, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._start_shape_connected_to = None
         self._start_shape_connected_to_index = None
         self._end_shape_connected_to = None
         self._end_shape_connected_to_index = None
         self.type = 'Connector'
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/document.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/effect.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,15 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'type': 'str',
         'subtype': 'str',
         'preset_class_type': 'str',
+        'animate_text_type': 'str',
         'shape_index': 'int',
         'paragraph_index': 'int',
         'trigger_type': 'str',
         'accelerate': 'float',
         'auto_reverse': 'bool',
         'decelerate': 'float',
         'duration': 'float',
@@ -65,14 +66,15 @@
         'after_animation_color': 'str'
     }
 
     attribute_map = {
         'type': 'type',
         'subtype': 'subtype',
         'preset_class_type': 'presetClassType',
+        'animate_text_type': 'animateTextType',
         'shape_index': 'shapeIndex',
         'paragraph_index': 'paragraphIndex',
         'trigger_type': 'triggerType',
         'accelerate': 'accelerate',
         'auto_reverse': 'autoReverse',
         'decelerate': 'decelerate',
         'duration': 'duration',
@@ -88,20 +90,21 @@
         'after_animation_type': 'afterAnimationType',
         'after_animation_color': 'afterAnimationColor'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, type=None, subtype=None, preset_class_type=None, shape_index=None, paragraph_index=None, trigger_type=None, accelerate=None, auto_reverse=None, decelerate=None, duration=None, repeat_count=None, repeat_duration=None, restart=None, speed=None, trigger_delay_time=None, repeat_until_end_slide=None, repeat_until_next_click=None, stop_previous_sound=None, rewind=None, after_animation_type=None, after_animation_color=None):  # noqa: E501
+    def __init__(self, type=None, subtype=None, preset_class_type=None, animate_text_type=None, shape_index=None, paragraph_index=None, trigger_type=None, accelerate=None, auto_reverse=None, decelerate=None, duration=None, repeat_count=None, repeat_duration=None, restart=None, speed=None, trigger_delay_time=None, repeat_until_end_slide=None, repeat_until_next_click=None, stop_previous_sound=None, rewind=None, after_animation_type=None, after_animation_color=None):  # noqa: E501
         """Effect - a model defined in Swagger"""  # noqa: E501
 
         self._type = None
         self._subtype = None
         self._preset_class_type = None
+        self._animate_text_type = None
         self._shape_index = None
         self._paragraph_index = None
         self._trigger_type = None
         self._accelerate = None
         self._auto_reverse = None
         self._decelerate = None
         self._duration = None
@@ -119,14 +122,16 @@
 
         if type is not None:
             self.type = type
         if subtype is not None:
             self.subtype = subtype
         if preset_class_type is not None:
             self.preset_class_type = preset_class_type
+        if animate_text_type is not None:
+            self.animate_text_type = animate_text_type
         self.shape_index = shape_index
         if paragraph_index is not None:
             self.paragraph_index = paragraph_index
         if trigger_type is not None:
             self.trigger_type = trigger_type
         if accelerate is not None:
             self.accelerate = accelerate
@@ -270,14 +275,52 @@
                 raise ValueError(
                     "Invalid value for `preset_class_type` ({0}), must be one of {1}"  # noqa: E501
                     .format(preset_class_type, allowed_values)
                 )
         self._preset_class_type = preset_class_type
 
     @property
+    def animate_text_type(self):
+        """Gets the animate_text_type of this Effect.  # noqa: E501
+
+        Preset class type.  # noqa: E501
+
+        :return: The animate_text_type of this Effect.  # noqa: E501
+        :rtype: str
+        """
+        return self._animate_text_type
+
+    @animate_text_type.setter
+    def animate_text_type(self, animate_text_type):
+        """Sets the animate_text_type of this Effect.
+
+        Preset class type.  # noqa: E501
+
+        :param animate_text_type: The animate_text_type of this Effect.  # noqa: E501
+        :type: str
+        """
+        if animate_text_type is not None:
+            allowed_values = ["AllAtOnce", "ByWord", "ByLetter"]  # noqa: E501
+            if animate_text_type.isdigit():
+                int_animate_text_type = int(animate_text_type)
+                if int_animate_text_type < 0 or int_animate_text_type >= len(allowed_values):
+                    raise ValueError(
+                        "Invalid value for `animate_text_type` ({0}), must be one of {1}"  # noqa: E501
+                        .format(animate_text_type, allowed_values)
+                    )
+                self._animate_text_type = allowed_values[int_animate_text_type]
+                return
+            if animate_text_type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `animate_text_type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(animate_text_type, allowed_values)
+                )
+        self._animate_text_type = animate_text_type
+
+    @property
     def shape_index(self):
         """Gets the shape_index of this Effect.  # noqa: E501
 
         Shape index.  # noqa: E501
 
         :return: The shape_index of this Effect.  # noqa: E501
         :rtype: int
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/error.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/export_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     JPEG = "Jpeg"
     PNG = "Png"
     GIF = "Gif"
     BMP = "Bmp"
     FODP = "Fodp"
     XAML = "Xaml"
     MPEG4 = "Mpeg4"
+    MD = "Md"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/geometry_shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -69,14 +70,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -85,17 +87,17 @@
         'type': 'type',
         'shape_type': 'shapeType'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type=None, shape_type=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type=None, shape_type=None):  # noqa: E501
         """GeometryShape - a model defined in Swagger"""  # noqa: E501
-        super(GeometryShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(GeometryShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._shape_type = None
 
         self.shape_type = shape_type
 
     @property
     def shape_type(self):
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/graphical_object.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -68,14 +69,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -84,17 +86,17 @@
         'type': 'type'
     }
 
     type_determiners = {
         'type': 'GraphicalObject',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='GraphicalObject'):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='GraphicalObject'):  # noqa: E501
         """GraphicalObject - a model defined in Swagger"""  # noqa: E501
-        super(GraphicalObject, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(GraphicalObject, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
         self.type = 'GraphicalObject'
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/group_shape.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -69,14 +70,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -86,17 +88,17 @@
         'shapes': 'shapes'
     }
 
     type_determiners = {
         'type': 'GroupShape',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='GroupShape', shapes=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='GroupShape', shapes=None):  # noqa: E501
         """GroupShape - a model defined in Swagger"""  # noqa: E501
-        super(GroupShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(GroupShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._shapes = None
         self.type = 'GroupShape'
 
         if shapes is not None:
             self.shapes = shapes
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/html5_export_options.py`

 * *Files 20% similar despite different names*

```diff
@@ -44,42 +44,52 @@
     """
     swagger_types = {
         'default_regular_font': 'str',
         'font_fallback_rules': 'list[FontFallbackRule]',
         'font_subst_rules': 'list[FontSubstRule]',
         'format': 'str',
         'animate_transitions': 'bool',
-        'animate_shapes': 'bool'
+        'animate_shapes': 'bool',
+        'embed_images': 'bool',
+        'notes_comments_layouting': 'NotesCommentsLayoutingOptions'
     }
 
     attribute_map = {
         'default_regular_font': 'defaultRegularFont',
         'font_fallback_rules': 'fontFallbackRules',
         'font_subst_rules': 'fontSubstRules',
         'format': 'format',
         'animate_transitions': 'animateTransitions',
-        'animate_shapes': 'animateShapes'
+        'animate_shapes': 'animateShapes',
+        'embed_images': 'embedImages',
+        'notes_comments_layouting': 'notesCommentsLayouting'
     }
 
     type_determiners = {
         'format': 'html5',
     }
 
-    def __init__(self, default_regular_font=None, font_fallback_rules=None, font_subst_rules=None, format='html5', animate_transitions=None, animate_shapes=None):  # noqa: E501
+    def __init__(self, default_regular_font=None, font_fallback_rules=None, font_subst_rules=None, format='html5', animate_transitions=None, animate_shapes=None, embed_images=None, notes_comments_layouting=None):  # noqa: E501
         """Html5ExportOptions - a model defined in Swagger"""  # noqa: E501
         super(Html5ExportOptions, self).__init__(default_regular_font, font_fallback_rules, font_subst_rules, format)
 
         self._animate_transitions = None
         self._animate_shapes = None
+        self._embed_images = None
+        self._notes_comments_layouting = None
         self.format = 'html5'
 
         if animate_transitions is not None:
             self.animate_transitions = animate_transitions
         if animate_shapes is not None:
             self.animate_shapes = animate_shapes
+        if embed_images is not None:
+            self.embed_images = embed_images
+        if notes_comments_layouting is not None:
+            self.notes_comments_layouting = notes_comments_layouting
 
     @property
     def animate_transitions(self):
         """Gets the animate_transitions of this Html5ExportOptions.  # noqa: E501
 
         Gets or sets transitions animation option.  # noqa: E501
 
@@ -117,14 +127,58 @@
         Gets or sets shapes animation option.  # noqa: E501
 
         :param animate_shapes: The animate_shapes of this Html5ExportOptions.  # noqa: E501
         :type: bool
         """
         self._animate_shapes = animate_shapes
 
+    @property
+    def embed_images(self):
+        """Gets the embed_images of this Html5ExportOptions.  # noqa: E501
+
+        Gets or sets embed images option.  # noqa: E501
+
+        :return: The embed_images of this Html5ExportOptions.  # noqa: E501
+        :rtype: bool
+        """
+        return self._embed_images
+
+    @embed_images.setter
+    def embed_images(self, embed_images):
+        """Sets the embed_images of this Html5ExportOptions.
+
+        Gets or sets embed images option.  # noqa: E501
+
+        :param embed_images: The embed_images of this Html5ExportOptions.  # noqa: E501
+        :type: bool
+        """
+        self._embed_images = embed_images
+
+    @property
+    def notes_comments_layouting(self):
+        """Gets the notes_comments_layouting of this Html5ExportOptions.  # noqa: E501
+
+        Slides layouting options  # noqa: E501
+
+        :return: The notes_comments_layouting of this Html5ExportOptions.  # noqa: E501
+        :rtype: NotesCommentsLayoutingOptions
+        """
+        return self._notes_comments_layouting
+
+    @notes_comments_layouting.setter
+    def notes_comments_layouting(self, notes_comments_layouting):
+        """Sets the notes_comments_layouting of this Html5ExportOptions.
+
+        Slides layouting options  # noqa: E501
+
+        :param notes_comments_layouting: The notes_comments_layouting of this Html5ExportOptions.  # noqa: E501
+        :type: NotesCommentsLayoutingOptions
+        """
+        self._notes_comments_layouting = notes_comments_layouting
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_base.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,422 +26,516 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from asposeslidescloud.models.export_options import ExportOptions
+from asposeslidescloud.models.resource_base import ResourceBase
 
-class HtmlExportOptions(ExportOptions):
+class ShapeBase(ResourceBase):
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'default_regular_font': 'str',
-        'font_fallback_rules': 'list[FontFallbackRule]',
-        'font_subst_rules': 'list[FontSubstRule]',
-        'format': 'str',
-        'save_as_zip': 'bool',
-        'sub_directory_name': 'str',
-        'show_hidden_slides': 'bool',
-        'svg_responsive_layout': 'bool',
-        'jpeg_quality': 'int',
-        'pictures_compression': 'str',
-        'delete_pictures_cropped_areas': 'bool',
-        'notes_position': 'str',
-        'comments_position': 'str',
-        'comments_area_width': 'int',
-        'comments_area_color': 'str',
-        'show_comments_by_no_author': 'bool'
+        'self_uri': 'ResourceUri',
+        'alternate_links': 'list[ResourceUri]',
+        'name': 'str',
+        'width': 'float',
+        'height': 'float',
+        'alternative_text': 'str',
+        'alternative_text_title': 'str',
+        'hidden': 'bool',
+        'is_decorative': 'bool',
+        'x': 'float',
+        'y': 'float',
+        'z_order_position': 'int',
+        'fill_format': 'FillFormat',
+        'effect_format': 'EffectFormat',
+        'three_d_format': 'ThreeDFormat',
+        'line_format': 'LineFormat',
+        'hyperlink_click': 'Hyperlink',
+        'hyperlink_mouse_over': 'Hyperlink',
+        'type': 'str'
     }
 
     attribute_map = {
-        'default_regular_font': 'defaultRegularFont',
-        'font_fallback_rules': 'fontFallbackRules',
-        'font_subst_rules': 'fontSubstRules',
-        'format': 'format',
-        'save_as_zip': 'saveAsZip',
-        'sub_directory_name': 'subDirectoryName',
-        'show_hidden_slides': 'showHiddenSlides',
-        'svg_responsive_layout': 'svgResponsiveLayout',
-        'jpeg_quality': 'jpegQuality',
-        'pictures_compression': 'picturesCompression',
-        'delete_pictures_cropped_areas': 'deletePicturesCroppedAreas',
-        'notes_position': 'notesPosition',
-        'comments_position': 'commentsPosition',
-        'comments_area_width': 'commentsAreaWidth',
-        'comments_area_color': 'commentsAreaColor',
-        'show_comments_by_no_author': 'showCommentsByNoAuthor'
+        'self_uri': 'selfUri',
+        'alternate_links': 'alternateLinks',
+        'name': 'name',
+        'width': 'width',
+        'height': 'height',
+        'alternative_text': 'alternativeText',
+        'alternative_text_title': 'alternativeTextTitle',
+        'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
+        'x': 'x',
+        'y': 'y',
+        'z_order_position': 'zOrderPosition',
+        'fill_format': 'fillFormat',
+        'effect_format': 'effectFormat',
+        'three_d_format': 'threeDFormat',
+        'line_format': 'lineFormat',
+        'hyperlink_click': 'hyperlinkClick',
+        'hyperlink_mouse_over': 'hyperlinkMouseOver',
+        'type': 'type'
     }
 
     type_determiners = {
-        'format': 'html',
     }
 
-    def __init__(self, default_regular_font=None, font_fallback_rules=None, font_subst_rules=None, format='html', save_as_zip=None, sub_directory_name=None, show_hidden_slides=None, svg_responsive_layout=None, jpeg_quality=None, pictures_compression=None, delete_pictures_cropped_areas=None, notes_position=None, comments_position=None, comments_area_width=None, comments_area_color=None, show_comments_by_no_author=None):  # noqa: E501
-        """HtmlExportOptions - a model defined in Swagger"""  # noqa: E501
-        super(HtmlExportOptions, self).__init__(default_regular_font, font_fallback_rules, font_subst_rules, format)
-
-        self._save_as_zip = None
-        self._sub_directory_name = None
-        self._show_hidden_slides = None
-        self._svg_responsive_layout = None
-        self._jpeg_quality = None
-        self._pictures_compression = None
-        self._delete_pictures_cropped_areas = None
-        self._notes_position = None
-        self._comments_position = None
-        self._comments_area_width = None
-        self._comments_area_color = None
-        self._show_comments_by_no_author = None
-        self.format = 'html'
-
-        if save_as_zip is not None:
-            self.save_as_zip = save_as_zip
-        if sub_directory_name is not None:
-            self.sub_directory_name = sub_directory_name
-        if show_hidden_slides is not None:
-            self.show_hidden_slides = show_hidden_slides
-        if svg_responsive_layout is not None:
-            self.svg_responsive_layout = svg_responsive_layout
-        if jpeg_quality is not None:
-            self.jpeg_quality = jpeg_quality
-        if pictures_compression is not None:
-            self.pictures_compression = pictures_compression
-        if delete_pictures_cropped_areas is not None:
-            self.delete_pictures_cropped_areas = delete_pictures_cropped_areas
-        if notes_position is not None:
-            self.notes_position = notes_position
-        if comments_position is not None:
-            self.comments_position = comments_position
-        if comments_area_width is not None:
-            self.comments_area_width = comments_area_width
-        if comments_area_color is not None:
-            self.comments_area_color = comments_area_color
-        if show_comments_by_no_author is not None:
-            self.show_comments_by_no_author = show_comments_by_no_author
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type=None):  # noqa: E501
+        """ShapeBase - a model defined in Swagger"""  # noqa: E501
+        super(ShapeBase, self).__init__(self_uri, alternate_links)
+
+        self._name = None
+        self._width = None
+        self._height = None
+        self._alternative_text = None
+        self._alternative_text_title = None
+        self._hidden = None
+        self._is_decorative = None
+        self._x = None
+        self._y = None
+        self._z_order_position = None
+        self._fill_format = None
+        self._effect_format = None
+        self._three_d_format = None
+        self._line_format = None
+        self._hyperlink_click = None
+        self._hyperlink_mouse_over = None
+        self._type = None
+
+        if name is not None:
+            self.name = name
+        if width is not None:
+            self.width = width
+        if height is not None:
+            self.height = height
+        if alternative_text is not None:
+            self.alternative_text = alternative_text
+        if alternative_text_title is not None:
+            self.alternative_text_title = alternative_text_title
+        if hidden is not None:
+            self.hidden = hidden
+        if is_decorative is not None:
+            self.is_decorative = is_decorative
+        if x is not None:
+            self.x = x
+        if y is not None:
+            self.y = y
+        self.z_order_position = z_order_position
+        if fill_format is not None:
+            self.fill_format = fill_format
+        if effect_format is not None:
+            self.effect_format = effect_format
+        if three_d_format is not None:
+            self.three_d_format = three_d_format
+        if line_format is not None:
+            self.line_format = line_format
+        if hyperlink_click is not None:
+            self.hyperlink_click = hyperlink_click
+        if hyperlink_mouse_over is not None:
+            self.hyperlink_mouse_over = hyperlink_mouse_over
+        if type is not None:
+            self.type = type
 
     @property
-    def save_as_zip(self):
-        """Gets the save_as_zip of this HtmlExportOptions.  # noqa: E501
+    def name(self):
+        """Gets the name of this ShapeBase.  # noqa: E501
 
-        Get or sets flag for save presentation as zip file  # noqa: E501
+        Gets or sets the name.  # noqa: E501
 
-        :return: The save_as_zip of this HtmlExportOptions.  # noqa: E501
-        :rtype: bool
+        :return: The name of this ShapeBase.  # noqa: E501
+        :rtype: str
         """
-        return self._save_as_zip
+        return self._name
 
-    @save_as_zip.setter
-    def save_as_zip(self, save_as_zip):
-        """Sets the save_as_zip of this HtmlExportOptions.
+    @name.setter
+    def name(self, name):
+        """Sets the name of this ShapeBase.
 
-        Get or sets flag for save presentation as zip file  # noqa: E501
+        Gets or sets the name.  # noqa: E501
 
-        :param save_as_zip: The save_as_zip of this HtmlExportOptions.  # noqa: E501
-        :type: bool
+        :param name: The name of this ShapeBase.  # noqa: E501
+        :type: str
+        """
+        self._name = name
+
+    @property
+    def width(self):
+        """Gets the width of this ShapeBase.  # noqa: E501
+
+        Gets or sets the width.  # noqa: E501
+
+        :return: The width of this ShapeBase.  # noqa: E501
+        :rtype: float
+        """
+        return self._width
+
+    @width.setter
+    def width(self, width):
+        """Sets the width of this ShapeBase.
+
+        Gets or sets the width.  # noqa: E501
+
+        :param width: The width of this ShapeBase.  # noqa: E501
+        :type: float
+        """
+        self._width = width
+
+    @property
+    def height(self):
+        """Gets the height of this ShapeBase.  # noqa: E501
+
+        Gets or sets the height.  # noqa: E501
+
+        :return: The height of this ShapeBase.  # noqa: E501
+        :rtype: float
+        """
+        return self._height
+
+    @height.setter
+    def height(self, height):
+        """Sets the height of this ShapeBase.
+
+        Gets or sets the height.  # noqa: E501
+
+        :param height: The height of this ShapeBase.  # noqa: E501
+        :type: float
         """
-        self._save_as_zip = save_as_zip
+        self._height = height
 
     @property
-    def sub_directory_name(self):
-        """Gets the sub_directory_name of this HtmlExportOptions.  # noqa: E501
+    def alternative_text(self):
+        """Gets the alternative_text of this ShapeBase.  # noqa: E501
 
-        Get or set name of subdirectory in zip-file for store external files  # noqa: E501
+        Gets or sets the alternative text.  # noqa: E501
 
-        :return: The sub_directory_name of this HtmlExportOptions.  # noqa: E501
+        :return: The alternative_text of this ShapeBase.  # noqa: E501
         :rtype: str
         """
-        return self._sub_directory_name
+        return self._alternative_text
 
-    @sub_directory_name.setter
-    def sub_directory_name(self, sub_directory_name):
-        """Sets the sub_directory_name of this HtmlExportOptions.
+    @alternative_text.setter
+    def alternative_text(self, alternative_text):
+        """Sets the alternative_text of this ShapeBase.
 
-        Get or set name of subdirectory in zip-file for store external files  # noqa: E501
+        Gets or sets the alternative text.  # noqa: E501
 
-        :param sub_directory_name: The sub_directory_name of this HtmlExportOptions.  # noqa: E501
+        :param alternative_text: The alternative_text of this ShapeBase.  # noqa: E501
         :type: str
         """
-        self._sub_directory_name = sub_directory_name
+        self._alternative_text = alternative_text
 
     @property
-    def show_hidden_slides(self):
-        """Gets the show_hidden_slides of this HtmlExportOptions.  # noqa: E501
+    def alternative_text_title(self):
+        """Gets the alternative_text_title of this ShapeBase.  # noqa: E501
 
-        Specifies whether the generated document should include hidden slides or not. Default is false.   # noqa: E501
+        The title of alternative text associated with the shape.  # noqa: E501
 
-        :return: The show_hidden_slides of this HtmlExportOptions.  # noqa: E501
+        :return: The alternative_text_title of this ShapeBase.  # noqa: E501
+        :rtype: str
+        """
+        return self._alternative_text_title
+
+    @alternative_text_title.setter
+    def alternative_text_title(self, alternative_text_title):
+        """Sets the alternative_text_title of this ShapeBase.
+
+        The title of alternative text associated with the shape.  # noqa: E501
+
+        :param alternative_text_title: The alternative_text_title of this ShapeBase.  # noqa: E501
+        :type: str
+        """
+        self._alternative_text_title = alternative_text_title
+
+    @property
+    def hidden(self):
+        """Gets the hidden of this ShapeBase.  # noqa: E501
+
+        Gets or sets a value indicating whether this ShapeBase is hidden.  # noqa: E501
+
+        :return: The hidden of this ShapeBase.  # noqa: E501
         :rtype: bool
         """
-        return self._show_hidden_slides
+        return self._hidden
 
-    @show_hidden_slides.setter
-    def show_hidden_slides(self, show_hidden_slides):
-        """Sets the show_hidden_slides of this HtmlExportOptions.
+    @hidden.setter
+    def hidden(self, hidden):
+        """Sets the hidden of this ShapeBase.
 
-        Specifies whether the generated document should include hidden slides or not. Default is false.   # noqa: E501
+        Gets or sets a value indicating whether this ShapeBase is hidden.  # noqa: E501
 
-        :param show_hidden_slides: The show_hidden_slides of this HtmlExportOptions.  # noqa: E501
+        :param hidden: The hidden of this ShapeBase.  # noqa: E501
         :type: bool
         """
-        self._show_hidden_slides = show_hidden_slides
+        self._hidden = hidden
 
     @property
-    def svg_responsive_layout(self):
-        """Gets the svg_responsive_layout of this HtmlExportOptions.  # noqa: E501
+    def is_decorative(self):
+        """Gets the is_decorative of this ShapeBase.  # noqa: E501
 
-        True to make layout responsive by excluding width and height attributes from svg container.  # noqa: E501
+        Gets or sets 'Mark as decorative' option.  # noqa: E501
 
-        :return: The svg_responsive_layout of this HtmlExportOptions.  # noqa: E501
+        :return: The is_decorative of this ShapeBase.  # noqa: E501
         :rtype: bool
         """
-        return self._svg_responsive_layout
+        return self._is_decorative
 
-    @svg_responsive_layout.setter
-    def svg_responsive_layout(self, svg_responsive_layout):
-        """Sets the svg_responsive_layout of this HtmlExportOptions.
+    @is_decorative.setter
+    def is_decorative(self, is_decorative):
+        """Sets the is_decorative of this ShapeBase.
 
-        True to make layout responsive by excluding width and height attributes from svg container.  # noqa: E501
+        Gets or sets 'Mark as decorative' option.  # noqa: E501
 
-        :param svg_responsive_layout: The svg_responsive_layout of this HtmlExportOptions.  # noqa: E501
+        :param is_decorative: The is_decorative of this ShapeBase.  # noqa: E501
         :type: bool
         """
-        self._svg_responsive_layout = svg_responsive_layout
+        self._is_decorative = is_decorative
 
     @property
-    def jpeg_quality(self):
-        """Gets the jpeg_quality of this HtmlExportOptions.  # noqa: E501
+    def x(self):
+        """Gets the x of this ShapeBase.  # noqa: E501
 
-        Returns or sets a value determining the quality of the JPEG images inside PDF document.  # noqa: E501
+        Gets or sets the X  # noqa: E501
+
+        :return: The x of this ShapeBase.  # noqa: E501
+        :rtype: float
+        """
+        return self._x
+
+    @x.setter
+    def x(self, x):
+        """Sets the x of this ShapeBase.
+
+        Gets or sets the X  # noqa: E501
+
+        :param x: The x of this ShapeBase.  # noqa: E501
+        :type: float
+        """
+        self._x = x
+
+    @property
+    def y(self):
+        """Gets the y of this ShapeBase.  # noqa: E501
+
+        Gets or sets the Y.  # noqa: E501
+
+        :return: The y of this ShapeBase.  # noqa: E501
+        :rtype: float
+        """
+        return self._y
 
-        :return: The jpeg_quality of this HtmlExportOptions.  # noqa: E501
+    @y.setter
+    def y(self, y):
+        """Sets the y of this ShapeBase.
+
+        Gets or sets the Y.  # noqa: E501
+
+        :param y: The y of this ShapeBase.  # noqa: E501
+        :type: float
+        """
+        self._y = y
+
+    @property
+    def z_order_position(self):
+        """Gets the z_order_position of this ShapeBase.  # noqa: E501
+
+        Gets z-order position of shape  # noqa: E501
+
+        :return: The z_order_position of this ShapeBase.  # noqa: E501
         :rtype: int
         """
-        return self._jpeg_quality
+        return self._z_order_position
 
-    @jpeg_quality.setter
-    def jpeg_quality(self, jpeg_quality):
-        """Sets the jpeg_quality of this HtmlExportOptions.
+    @z_order_position.setter
+    def z_order_position(self, z_order_position):
+        """Sets the z_order_position of this ShapeBase.
 
-        Returns or sets a value determining the quality of the JPEG images inside PDF document.  # noqa: E501
+        Gets z-order position of shape  # noqa: E501
 
-        :param jpeg_quality: The jpeg_quality of this HtmlExportOptions.  # noqa: E501
+        :param z_order_position: The z_order_position of this ShapeBase.  # noqa: E501
         :type: int
         """
-        self._jpeg_quality = jpeg_quality
+        self._z_order_position = z_order_position
 
     @property
-    def pictures_compression(self):
-        """Gets the pictures_compression of this HtmlExportOptions.  # noqa: E501
+    def fill_format(self):
+        """Gets the fill_format of this ShapeBase.  # noqa: E501
 
-        Represents the pictures compression level  # noqa: E501
+        Gets or sets the fill format.  # noqa: E501
 
-        :return: The pictures_compression of this HtmlExportOptions.  # noqa: E501
-        :rtype: str
+        :return: The fill_format of this ShapeBase.  # noqa: E501
+        :rtype: FillFormat
         """
-        return self._pictures_compression
+        return self._fill_format
 
-    @pictures_compression.setter
-    def pictures_compression(self, pictures_compression):
-        """Sets the pictures_compression of this HtmlExportOptions.
+    @fill_format.setter
+    def fill_format(self, fill_format):
+        """Sets the fill_format of this ShapeBase.
 
-        Represents the pictures compression level  # noqa: E501
+        Gets or sets the fill format.  # noqa: E501
 
-        :param pictures_compression: The pictures_compression of this HtmlExportOptions.  # noqa: E501
-        :type: str
+        :param fill_format: The fill_format of this ShapeBase.  # noqa: E501
+        :type: FillFormat
         """
-        if pictures_compression is not None:
-            allowed_values = ["Dpi330", "Dpi220", "Dpi150", "Dpi96", "Dpi72", "DocumentResolution"]  # noqa: E501
-            if pictures_compression.isdigit():
-                int_pictures_compression = int(pictures_compression)
-                if int_pictures_compression < 0 or int_pictures_compression >= len(allowed_values):
-                    raise ValueError(
-                        "Invalid value for `pictures_compression` ({0}), must be one of {1}"  # noqa: E501
-                        .format(pictures_compression, allowed_values)
-                    )
-                self._pictures_compression = allowed_values[int_pictures_compression]
-                return
-            if pictures_compression not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `pictures_compression` ({0}), must be one of {1}"  # noqa: E501
-                    .format(pictures_compression, allowed_values)
-                )
-        self._pictures_compression = pictures_compression
+        self._fill_format = fill_format
 
     @property
-    def delete_pictures_cropped_areas(self):
-        """Gets the delete_pictures_cropped_areas of this HtmlExportOptions.  # noqa: E501
+    def effect_format(self):
+        """Gets the effect_format of this ShapeBase.  # noqa: E501
 
-        A boolean flag indicates if the cropped parts remain as part of the document. If true the cropped  parts will removed, if false they will be serialized in the document (which can possible lead to a  larger file)  # noqa: E501
+        Gets or sets the effect format.  # noqa: E501
 
-        :return: The delete_pictures_cropped_areas of this HtmlExportOptions.  # noqa: E501
-        :rtype: bool
+        :return: The effect_format of this ShapeBase.  # noqa: E501
+        :rtype: EffectFormat
         """
-        return self._delete_pictures_cropped_areas
+        return self._effect_format
 
-    @delete_pictures_cropped_areas.setter
-    def delete_pictures_cropped_areas(self, delete_pictures_cropped_areas):
-        """Sets the delete_pictures_cropped_areas of this HtmlExportOptions.
+    @effect_format.setter
+    def effect_format(self, effect_format):
+        """Sets the effect_format of this ShapeBase.
 
-        A boolean flag indicates if the cropped parts remain as part of the document. If true the cropped  parts will removed, if false they will be serialized in the document (which can possible lead to a  larger file)  # noqa: E501
+        Gets or sets the effect format.  # noqa: E501
 
-        :param delete_pictures_cropped_areas: The delete_pictures_cropped_areas of this HtmlExportOptions.  # noqa: E501
-        :type: bool
+        :param effect_format: The effect_format of this ShapeBase.  # noqa: E501
+        :type: EffectFormat
         """
-        self._delete_pictures_cropped_areas = delete_pictures_cropped_areas
+        self._effect_format = effect_format
 
     @property
-    def notes_position(self):
-        """Gets the notes_position of this HtmlExportOptions.  # noqa: E501
+    def three_d_format(self):
+        """Gets the three_d_format of this ShapeBase.  # noqa: E501
 
-        Gets or sets the position of the notes on the page.  # noqa: E501
+        Gets or sets the 3D format  # noqa: E501
 
-        :return: The notes_position of this HtmlExportOptions.  # noqa: E501
-        :rtype: str
+        :return: The three_d_format of this ShapeBase.  # noqa: E501
+        :rtype: ThreeDFormat
         """
-        return self._notes_position
+        return self._three_d_format
 
-    @notes_position.setter
-    def notes_position(self, notes_position):
-        """Sets the notes_position of this HtmlExportOptions.
+    @three_d_format.setter
+    def three_d_format(self, three_d_format):
+        """Sets the three_d_format of this ShapeBase.
 
-        Gets or sets the position of the notes on the page.  # noqa: E501
+        Gets or sets the 3D format  # noqa: E501
 
-        :param notes_position: The notes_position of this HtmlExportOptions.  # noqa: E501
-        :type: str
+        :param three_d_format: The three_d_format of this ShapeBase.  # noqa: E501
+        :type: ThreeDFormat
         """
-        if notes_position is not None:
-            allowed_values = ["None", "BottomFull", "BottomTruncated"]  # noqa: E501
-            if notes_position.isdigit():
-                int_notes_position = int(notes_position)
-                if int_notes_position < 0 or int_notes_position >= len(allowed_values):
-                    raise ValueError(
-                        "Invalid value for `notes_position` ({0}), must be one of {1}"  # noqa: E501
-                        .format(notes_position, allowed_values)
-                    )
-                self._notes_position = allowed_values[int_notes_position]
-                return
-            if notes_position not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `notes_position` ({0}), must be one of {1}"  # noqa: E501
-                    .format(notes_position, allowed_values)
-                )
-        self._notes_position = notes_position
+        self._three_d_format = three_d_format
 
     @property
-    def comments_position(self):
-        """Gets the comments_position of this HtmlExportOptions.  # noqa: E501
+    def line_format(self):
+        """Gets the line_format of this ShapeBase.  # noqa: E501
 
-        Gets or sets the position of the comments on the page.  # noqa: E501
+        Gets or sets the line format.  # noqa: E501
 
-        :return: The comments_position of this HtmlExportOptions.  # noqa: E501
-        :rtype: str
+        :return: The line_format of this ShapeBase.  # noqa: E501
+        :rtype: LineFormat
         """
-        return self._comments_position
+        return self._line_format
 
-    @comments_position.setter
-    def comments_position(self, comments_position):
-        """Sets the comments_position of this HtmlExportOptions.
+    @line_format.setter
+    def line_format(self, line_format):
+        """Sets the line_format of this ShapeBase.
 
-        Gets or sets the position of the comments on the page.  # noqa: E501
+        Gets or sets the line format.  # noqa: E501
 
-        :param comments_position: The comments_position of this HtmlExportOptions.  # noqa: E501
-        :type: str
+        :param line_format: The line_format of this ShapeBase.  # noqa: E501
+        :type: LineFormat
         """
-        if comments_position is not None:
-            allowed_values = ["None", "Bottom", "Right"]  # noqa: E501
-            if comments_position.isdigit():
-                int_comments_position = int(comments_position)
-                if int_comments_position < 0 or int_comments_position >= len(allowed_values):
-                    raise ValueError(
-                        "Invalid value for `comments_position` ({0}), must be one of {1}"  # noqa: E501
-                        .format(comments_position, allowed_values)
-                    )
-                self._comments_position = allowed_values[int_comments_position]
-                return
-            if comments_position not in allowed_values:
-                raise ValueError(
-                    "Invalid value for `comments_position` ({0}), must be one of {1}"  # noqa: E501
-                    .format(comments_position, allowed_values)
-                )
-        self._comments_position = comments_position
+        self._line_format = line_format
 
     @property
-    def comments_area_width(self):
-        """Gets the comments_area_width of this HtmlExportOptions.  # noqa: E501
+    def hyperlink_click(self):
+        """Gets the hyperlink_click of this ShapeBase.  # noqa: E501
 
-        Gets or sets the width of the comment output area in pixels (Applies only if comments are displayed on the right).  # noqa: E501
+        Hyperlink defined for mouse click.  # noqa: E501
 
-        :return: The comments_area_width of this HtmlExportOptions.  # noqa: E501
-        :rtype: int
+        :return: The hyperlink_click of this ShapeBase.  # noqa: E501
+        :rtype: Hyperlink
         """
-        return self._comments_area_width
+        return self._hyperlink_click
 
-    @comments_area_width.setter
-    def comments_area_width(self, comments_area_width):
-        """Sets the comments_area_width of this HtmlExportOptions.
+    @hyperlink_click.setter
+    def hyperlink_click(self, hyperlink_click):
+        """Sets the hyperlink_click of this ShapeBase.
 
-        Gets or sets the width of the comment output area in pixels (Applies only if comments are displayed on the right).  # noqa: E501
+        Hyperlink defined for mouse click.  # noqa: E501
 
-        :param comments_area_width: The comments_area_width of this HtmlExportOptions.  # noqa: E501
-        :type: int
+        :param hyperlink_click: The hyperlink_click of this ShapeBase.  # noqa: E501
+        :type: Hyperlink
         """
-        self._comments_area_width = comments_area_width
+        self._hyperlink_click = hyperlink_click
 
     @property
-    def comments_area_color(self):
-        """Gets the comments_area_color of this HtmlExportOptions.  # noqa: E501
+    def hyperlink_mouse_over(self):
+        """Gets the hyperlink_mouse_over of this ShapeBase.  # noqa: E501
 
-        Gets or sets the color of comments area (Applies only if comments are displayed on the right).  # noqa: E501
+        Hyperlink defined for mouse over.  # noqa: E501
 
-        :return: The comments_area_color of this HtmlExportOptions.  # noqa: E501
-        :rtype: str
+        :return: The hyperlink_mouse_over of this ShapeBase.  # noqa: E501
+        :rtype: Hyperlink
         """
-        return self._comments_area_color
+        return self._hyperlink_mouse_over
 
-    @comments_area_color.setter
-    def comments_area_color(self, comments_area_color):
-        """Sets the comments_area_color of this HtmlExportOptions.
+    @hyperlink_mouse_over.setter
+    def hyperlink_mouse_over(self, hyperlink_mouse_over):
+        """Sets the hyperlink_mouse_over of this ShapeBase.
 
-        Gets or sets the color of comments area (Applies only if comments are displayed on the right).  # noqa: E501
+        Hyperlink defined for mouse over.  # noqa: E501
 
-        :param comments_area_color: The comments_area_color of this HtmlExportOptions.  # noqa: E501
-        :type: str
+        :param hyperlink_mouse_over: The hyperlink_mouse_over of this ShapeBase.  # noqa: E501
+        :type: Hyperlink
         """
-        self._comments_area_color = comments_area_color
+        self._hyperlink_mouse_over = hyperlink_mouse_over
 
     @property
-    def show_comments_by_no_author(self):
-        """Gets the show_comments_by_no_author of this HtmlExportOptions.  # noqa: E501
+    def type(self):
+        """Gets the type of this ShapeBase.  # noqa: E501
 
-        True if comments that have no author are displayed. (Applies only if comments are displayed).  # noqa: E501
 
-        :return: The show_comments_by_no_author of this HtmlExportOptions.  # noqa: E501
-        :rtype: bool
+        :return: The type of this ShapeBase.  # noqa: E501
+        :rtype: str
         """
-        return self._show_comments_by_no_author
+        return self._type
 
-    @show_comments_by_no_author.setter
-    def show_comments_by_no_author(self, show_comments_by_no_author):
-        """Sets the show_comments_by_no_author of this HtmlExportOptions.
+    @type.setter
+    def type(self, type):
+        """Sets the type of this ShapeBase.
 
-        True if comments that have no author are displayed. (Applies only if comments are displayed).  # noqa: E501
 
-        :param show_comments_by_no_author: The show_comments_by_no_author of this HtmlExportOptions.  # noqa: E501
-        :type: bool
+        :param type: The type of this ShapeBase.  # noqa: E501
+        :type: str
         """
-        self._show_comments_by_no_author = show_comments_by_no_author
+        if type is not None:
+            allowed_values = ["Shape", "Chart", "Table", "PictureFrame", "VideoFrame", "AudioFrame", "SmartArt", "OleObjectFrame", "GroupShape", "GraphicalObject", "Connector", "SmartArtShape", "ZoomFrame", "SectionZoomFrame", "SummaryZoomFrame", "SummaryZoomSection"]  # noqa: E501
+            if type.isdigit():
+                int_type = int(type)
+                if int_type < 0 or int_type >= len(allowed_values):
+                    raise ValueError(
+                        "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                        .format(type, allowed_values)
+                    )
+                self._type = allowed_values[int_type]
+                return
+            if type not in allowed_values:
+                raise ValueError(
+                    "Invalid value for `type` ({0}), must be one of {1}"  # noqa: E501
+                    .format(type, allowed_values)
+                )
+        self._type = type
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -469,15 +563,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, HtmlExportOptions):
+        if not isinstance(other, ShapeBase):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/image.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_comments_layouting_options.py`

 * *Files 18% similar despite different names*

```diff
@@ -26,98 +26,88 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from asposeslidescloud.models.image_export_options_base import ImageExportOptionsBase
+from asposeslidescloud.models.slides_layout_options import SlidesLayoutOptions
 
-class ImageExportOptions(ImageExportOptionsBase):
+class NotesCommentsLayoutingOptions(SlidesLayoutOptions):
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'default_regular_font': 'str',
-        'font_fallback_rules': 'list[FontFallbackRule]',
-        'font_subst_rules': 'list[FontSubstRule]',
-        'format': 'str',
-        'height': 'int',
-        'width': 'int',
+        'layout_type': 'str',
         'notes_position': 'str',
         'comments_position': 'str',
         'comments_area_width': 'int',
         'comments_area_color': 'str',
-        'show_hidden_slides': 'bool'
+        'show_comments_by_no_author': 'bool'
     }
 
     attribute_map = {
-        'default_regular_font': 'defaultRegularFont',
-        'font_fallback_rules': 'fontFallbackRules',
-        'font_subst_rules': 'fontSubstRules',
-        'format': 'format',
-        'height': 'height',
-        'width': 'width',
+        'layout_type': 'layoutType',
         'notes_position': 'notesPosition',
         'comments_position': 'commentsPosition',
         'comments_area_width': 'commentsAreaWidth',
         'comments_area_color': 'commentsAreaColor',
-        'show_hidden_slides': 'showHiddenSlides'
+        'show_comments_by_no_author': 'showCommentsByNoAuthor'
     }
 
     type_determiners = {
-        'format': 'image',
+        'layoutType': 'NotesComments',
     }
 
-    def __init__(self, default_regular_font=None, font_fallback_rules=None, font_subst_rules=None, format='image', height=None, width=None, notes_position=None, comments_position=None, comments_area_width=None, comments_area_color=None, show_hidden_slides=None):  # noqa: E501
-        """ImageExportOptions - a model defined in Swagger"""  # noqa: E501
-        super(ImageExportOptions, self).__init__(default_regular_font, font_fallback_rules, font_subst_rules, format, height, width)
+    def __init__(self, layout_type='NotesComments', notes_position=None, comments_position=None, comments_area_width=None, comments_area_color=None, show_comments_by_no_author=None):  # noqa: E501
+        """NotesCommentsLayoutingOptions - a model defined in Swagger"""  # noqa: E501
+        super(NotesCommentsLayoutingOptions, self).__init__(layout_type)
 
         self._notes_position = None
         self._comments_position = None
         self._comments_area_width = None
         self._comments_area_color = None
-        self._show_hidden_slides = None
-        self.format = 'image'
+        self._show_comments_by_no_author = None
+        self.layout_type = 'NotesComments'
 
         if notes_position is not None:
             self.notes_position = notes_position
         if comments_position is not None:
             self.comments_position = comments_position
         if comments_area_width is not None:
             self.comments_area_width = comments_area_width
         if comments_area_color is not None:
             self.comments_area_color = comments_area_color
-        if show_hidden_slides is not None:
-            self.show_hidden_slides = show_hidden_slides
+        if show_comments_by_no_author is not None:
+            self.show_comments_by_no_author = show_comments_by_no_author
 
     @property
     def notes_position(self):
-        """Gets the notes_position of this ImageExportOptions.  # noqa: E501
+        """Gets the notes_position of this NotesCommentsLayoutingOptions.  # noqa: E501
 
         Gets or sets the position of the notes on the page.  # noqa: E501
 
-        :return: The notes_position of this ImageExportOptions.  # noqa: E501
+        :return: The notes_position of this NotesCommentsLayoutingOptions.  # noqa: E501
         :rtype: str
         """
         return self._notes_position
 
     @notes_position.setter
     def notes_position(self, notes_position):
-        """Sets the notes_position of this ImageExportOptions.
+        """Sets the notes_position of this NotesCommentsLayoutingOptions.
 
         Gets or sets the position of the notes on the page.  # noqa: E501
 
-        :param notes_position: The notes_position of this ImageExportOptions.  # noqa: E501
+        :param notes_position: The notes_position of this NotesCommentsLayoutingOptions.  # noqa: E501
         :type: str
         """
         if notes_position is not None:
             allowed_values = ["None", "BottomFull", "BottomTruncated"]  # noqa: E501
             if notes_position.isdigit():
                 int_notes_position = int(notes_position)
                 if int_notes_position < 0 or int_notes_position >= len(allowed_values):
@@ -132,30 +122,30 @@
                     "Invalid value for `notes_position` ({0}), must be one of {1}"  # noqa: E501
                     .format(notes_position, allowed_values)
                 )
         self._notes_position = notes_position
 
     @property
     def comments_position(self):
-        """Gets the comments_position of this ImageExportOptions.  # noqa: E501
+        """Gets the comments_position of this NotesCommentsLayoutingOptions.  # noqa: E501
 
         Gets or sets the position of the comments on the page.  # noqa: E501
 
-        :return: The comments_position of this ImageExportOptions.  # noqa: E501
+        :return: The comments_position of this NotesCommentsLayoutingOptions.  # noqa: E501
         :rtype: str
         """
         return self._comments_position
 
     @comments_position.setter
     def comments_position(self, comments_position):
-        """Sets the comments_position of this ImageExportOptions.
+        """Sets the comments_position of this NotesCommentsLayoutingOptions.
 
         Gets or sets the position of the comments on the page.  # noqa: E501
 
-        :param comments_position: The comments_position of this ImageExportOptions.  # noqa: E501
+        :param comments_position: The comments_position of this NotesCommentsLayoutingOptions.  # noqa: E501
         :type: str
         """
         if comments_position is not None:
             allowed_values = ["None", "Bottom", "Right"]  # noqa: E501
             if comments_position.isdigit():
                 int_comments_position = int(comments_position)
                 if int_comments_position < 0 or int_comments_position >= len(allowed_values):
@@ -170,77 +160,77 @@
                     "Invalid value for `comments_position` ({0}), must be one of {1}"  # noqa: E501
                     .format(comments_position, allowed_values)
                 )
         self._comments_position = comments_position
 
     @property
     def comments_area_width(self):
-        """Gets the comments_area_width of this ImageExportOptions.  # noqa: E501
+        """Gets the comments_area_width of this NotesCommentsLayoutingOptions.  # noqa: E501
 
         Gets or sets the width of the comment output area in pixels (Applies only if comments are displayed on the right).  # noqa: E501
 
-        :return: The comments_area_width of this ImageExportOptions.  # noqa: E501
+        :return: The comments_area_width of this NotesCommentsLayoutingOptions.  # noqa: E501
         :rtype: int
         """
         return self._comments_area_width
 
     @comments_area_width.setter
     def comments_area_width(self, comments_area_width):
-        """Sets the comments_area_width of this ImageExportOptions.
+        """Sets the comments_area_width of this NotesCommentsLayoutingOptions.
 
         Gets or sets the width of the comment output area in pixels (Applies only if comments are displayed on the right).  # noqa: E501
 
-        :param comments_area_width: The comments_area_width of this ImageExportOptions.  # noqa: E501
+        :param comments_area_width: The comments_area_width of this NotesCommentsLayoutingOptions.  # noqa: E501
         :type: int
         """
         self._comments_area_width = comments_area_width
 
     @property
     def comments_area_color(self):
-        """Gets the comments_area_color of this ImageExportOptions.  # noqa: E501
+        """Gets the comments_area_color of this NotesCommentsLayoutingOptions.  # noqa: E501
 
         Gets or sets the color of comments area (Applies only if comments are displayed on the right).  # noqa: E501
 
-        :return: The comments_area_color of this ImageExportOptions.  # noqa: E501
+        :return: The comments_area_color of this NotesCommentsLayoutingOptions.  # noqa: E501
         :rtype: str
         """
         return self._comments_area_color
 
     @comments_area_color.setter
     def comments_area_color(self, comments_area_color):
-        """Sets the comments_area_color of this ImageExportOptions.
+        """Sets the comments_area_color of this NotesCommentsLayoutingOptions.
 
         Gets or sets the color of comments area (Applies only if comments are displayed on the right).  # noqa: E501
 
-        :param comments_area_color: The comments_area_color of this ImageExportOptions.  # noqa: E501
+        :param comments_area_color: The comments_area_color of this NotesCommentsLayoutingOptions.  # noqa: E501
         :type: str
         """
         self._comments_area_color = comments_area_color
 
     @property
-    def show_hidden_slides(self):
-        """Gets the show_hidden_slides of this ImageExportOptions.  # noqa: E501
+    def show_comments_by_no_author(self):
+        """Gets the show_comments_by_no_author of this NotesCommentsLayoutingOptions.  # noqa: E501
 
-        Show hidden slides. If true, hidden are exported.  # noqa: E501
+        True if comments that have no author are displayed. (Applies only if comments are displayed).  # noqa: E501
 
-        :return: The show_hidden_slides of this ImageExportOptions.  # noqa: E501
+        :return: The show_comments_by_no_author of this NotesCommentsLayoutingOptions.  # noqa: E501
         :rtype: bool
         """
-        return self._show_hidden_slides
+        return self._show_comments_by_no_author
 
-    @show_hidden_slides.setter
-    def show_hidden_slides(self, show_hidden_slides):
-        """Sets the show_hidden_slides of this ImageExportOptions.
+    @show_comments_by_no_author.setter
+    def show_comments_by_no_author(self, show_comments_by_no_author):
+        """Sets the show_comments_by_no_author of this NotesCommentsLayoutingOptions.
 
-        Show hidden slides. If true, hidden are exported.  # noqa: E501
+        True if comments that have no author are displayed. (Applies only if comments are displayed).  # noqa: E501
 
-        :param show_hidden_slides: The show_hidden_slides of this ImageExportOptions.  # noqa: E501
+        :param show_comments_by_no_author: The show_comments_by_no_author of this NotesCommentsLayoutingOptions.  # noqa: E501
         :type: bool
         """
-        self._show_hidden_slides = show_hidden_slides
+        self._show_comments_by_no_author = show_comments_by_no_author
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -268,15 +258,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ImageExportOptions):
+        if not isinstance(other, NotesCommentsLayoutingOptions):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/images.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/input.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -77,14 +78,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -102,17 +104,17 @@
         'update_automatic': 'updateAutomatic'
     }
 
     type_determiners = {
         'type': 'OleObjectFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='OleObjectFrame', is_object_icon=None, substitute_picture_title=None, substitute_picture_format=None, object_name=None, embedded_file_base64_data=None, embedded_file_extension=None, object_prog_id=None, link_path=None, update_automatic=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='OleObjectFrame', is_object_icon=None, substitute_picture_title=None, substitute_picture_format=None, object_name=None, embedded_file_base64_data=None, embedded_file_extension=None, object_prog_id=None, link_path=None, update_automatic=None):  # noqa: E501
         """OleObjectFrame - a model defined in Swagger"""  # noqa: E501
-        super(OleObjectFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(OleObjectFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._is_object_icon = None
         self._substitute_picture_title = None
         self._substitute_picture_format = None
         self._object_name = None
         self._embedded_file_base64_data = None
         self._embedded_file_extension = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/operation.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/operation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/operation_progress.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/operation_progress.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/path_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/picture_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -70,14 +71,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -88,17 +90,17 @@
         'picture_fill_format': 'pictureFillFormat'
     }
 
     type_determiners = {
         'type': 'PictureFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='PictureFrame', shape_type=None, picture_fill_format=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='PictureFrame', shape_type=None, picture_fill_format=None):  # noqa: E501
         """PictureFrame - a model defined in Swagger"""  # noqa: E501
-        super(PictureFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(PictureFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._picture_fill_format = None
         self.type = 'PictureFrame'
 
         if picture_fill_format is not None:
             self.picture_fill_format = picture_fill_format
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/portions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/save.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
         Format.  # noqa: E501
 
         :param format: The format of this Save.  # noqa: E501
         :type: str
         """
         if format is not None:
-            allowed_values = ["Pdf", "Xps", "Tiff", "Pptx", "Odp", "Otp", "Ppt", "Pps", "Ppsx", "Pptm", "Ppsm", "Pot", "Potx", "Potm", "Html", "Html5", "Swf", "Svg", "Jpeg", "Png", "Gif", "Bmp", "Fodp", "Xaml", "Mpeg4"]  # noqa: E501
+            allowed_values = ["Pdf", "Xps", "Tiff", "Pptx", "Odp", "Otp", "Ppt", "Pps", "Ppsx", "Pptm", "Ppsm", "Pot", "Potx", "Potm", "Html", "Html5", "Swf", "Svg", "Jpeg", "Png", "Gif", "Bmp", "Fodp", "Xaml", "Mpeg4", "Md"]  # noqa: E501
             if format.isdigit():
                 int_format = int(format)
                 if int_format < 0 or int_format >= len(allowed_values):
                     raise ValueError(
                         "Invalid value for `format` ({0}), must be one of {1}"  # noqa: E501
                         .format(format, allowed_values)
                     )
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/save_slide.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,15 +128,15 @@
 
         Save format.  # noqa: E501
 
         :param format: The format of this SaveSlide.  # noqa: E501
         :type: str
         """
         if format is not None:
-            allowed_values = ["Jpeg", "Png", "Gif", "Bmp", "Tiff", "Html", "Pdf", "Xps", "Pptx", "Odp", "Otp", "Ppt", "Pps", "Ppsx", "Pptm", "Ppsm", "Potx", "Pot", "Potm", "Svg", "Fodp", "Xaml", "Html5"]  # noqa: E501
+            allowed_values = ["Jpeg", "Png", "Gif", "Bmp", "Tiff", "Html", "Pdf", "Xps", "Pptx", "Odp", "Otp", "Ppt", "Pps", "Ppsx", "Pptm", "Ppsm", "Potx", "Pot", "Potm", "Svg", "Fodp", "Xaml", "Html5", "Md"]  # noqa: E501
             if format.isdigit():
                 int_format = int(format)
                 if int_format < 0 or int_format >= len(allowed_values):
                     raise ValueError(
                         "Invalid value for `format` ({0}), must be one of {1}"  # noqa: E501
                         .format(format, allowed_values)
                     )
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/section.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -74,14 +75,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -96,17 +98,17 @@
         'target_section_index': 'targetSectionIndex'
     }
 
     type_determiners = {
         'type': 'SectionZoomFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SectionZoomFrame', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_section_index=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SectionZoomFrame', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_section_index=None):  # noqa: E501
         """SectionZoomFrame - a model defined in Swagger"""  # noqa: E501
-        super(SectionZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration)
+        super(SectionZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration)
 
         self._target_section_index = None
         self.type = 'SectionZoomFrame'
 
         if target_section_index is not None:
             self.target_section_index = target_section_index
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/series.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -72,14 +73,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -92,17 +94,17 @@
         'text_frame_format': 'textFrameFormat'
     }
 
     type_determiners = {
         'type': 'Shape',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Shape', shape_type=None, text=None, paragraphs=None, text_frame_format=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Shape', shape_type=None, text=None, paragraphs=None, text_frame_format=None):  # noqa: E501
         """Shape - a model defined in Swagger"""  # noqa: E501
-        super(Shape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(Shape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._text = None
         self._paragraphs = None
         self._text_frame_format = None
         self.type = 'Shape'
 
         if text is not None:
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_export_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     POTX = "Potx"
     POT = "Pot"
     POTM = "Potm"
     SVG = "Svg"
     FODP = "Fodp"
     XAML = "Xaml"
     HTML5 = "Html5"
+    MD = "Md"
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,46 +47,49 @@
         'alternate_links': 'list[ResourceUri]',
         'loop': 'bool',
         'start_slide': 'int',
         'end_slide': 'int',
         'pen_color': 'str',
         'show_animation': 'bool',
         'show_narration': 'bool',
+        'show_media_controls': 'bool',
         'use_timings': 'bool',
         'slide_show_type': 'str',
         'show_scrollbar': 'bool'
     }
 
     attribute_map = {
         'self_uri': 'selfUri',
         'alternate_links': 'alternateLinks',
         'loop': 'loop',
         'start_slide': 'startSlide',
         'end_slide': 'endSlide',
         'pen_color': 'penColor',
         'show_animation': 'showAnimation',
         'show_narration': 'showNarration',
+        'show_media_controls': 'showMediaControls',
         'use_timings': 'useTimings',
         'slide_show_type': 'slideShowType',
         'show_scrollbar': 'showScrollbar'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, loop=None, start_slide=None, end_slide=None, pen_color=None, show_animation=None, show_narration=None, use_timings=None, slide_show_type=None, show_scrollbar=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, loop=None, start_slide=None, end_slide=None, pen_color=None, show_animation=None, show_narration=None, show_media_controls=None, use_timings=None, slide_show_type=None, show_scrollbar=None):  # noqa: E501
         """SlideShowProperties - a model defined in Swagger"""  # noqa: E501
         super(SlideShowProperties, self).__init__(self_uri, alternate_links)
 
         self._loop = None
         self._start_slide = None
         self._end_slide = None
         self._pen_color = None
         self._show_animation = None
         self._show_narration = None
+        self._show_media_controls = None
         self._use_timings = None
         self._slide_show_type = None
         self._show_scrollbar = None
 
         if loop is not None:
             self.loop = loop
         if start_slide is not None:
@@ -95,14 +98,16 @@
             self.end_slide = end_slide
         if pen_color is not None:
             self.pen_color = pen_color
         if show_animation is not None:
             self.show_animation = show_animation
         if show_narration is not None:
             self.show_narration = show_narration
+        if show_media_controls is not None:
+            self.show_media_controls = show_media_controls
         if use_timings is not None:
             self.use_timings = use_timings
         if slide_show_type is not None:
             self.slide_show_type = slide_show_type
         if show_scrollbar is not None:
             self.show_scrollbar = show_scrollbar
 
@@ -235,14 +240,36 @@
 
         :param show_narration: The show_narration of this SlideShowProperties.  # noqa: E501
         :type: bool
         """
         self._show_narration = show_narration
 
     @property
+    def show_media_controls(self):
+        """Gets the show_media_controls of this SlideShowProperties.  # noqa: E501
+
+        Show media controls.  # noqa: E501
+
+        :return: The show_media_controls of this SlideShowProperties.  # noqa: E501
+        :rtype: bool
+        """
+        return self._show_media_controls
+
+    @show_media_controls.setter
+    def show_media_controls(self, show_media_controls):
+        """Sets the show_media_controls of this SlideShowProperties.
+
+        Show media controls.  # noqa: E501
+
+        :param show_media_controls: The show_media_controls of this SlideShowProperties.  # noqa: E501
+        :type: bool
+        """
+        self._show_media_controls = show_media_controls
+
+    @property
     def use_timings(self):
         """Gets the use_timings of this SlideShowProperties.  # noqa: E501
 
         Use timings.  # noqa: E501
 
         :return: The use_timings of this SlideShowProperties.  # noqa: E501
         :rtype: bool
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slide_show_transition.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slide_show_transition.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -73,14 +74,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -94,17 +96,17 @@
         'is_reversed': 'isReversed'
     }
 
     type_determiners = {
         'type': 'SmartArt',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SmartArt', layout=None, quick_style=None, color_style=None, nodes=None, is_reversed=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SmartArt', layout=None, quick_style=None, color_style=None, nodes=None, is_reversed=None):  # noqa: E501
         """SmartArt - a model defined in Swagger"""  # noqa: E501
-        super(SmartArt, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(SmartArt, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._layout = None
         self._quick_style = None
         self._color_style = None
         self._nodes = None
         self._is_reversed = None
         self.type = 'SmartArt'
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -69,14 +70,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -86,17 +88,17 @@
         'shape_type': 'shapeType'
     }
 
     type_determiners = {
         'type': 'SmartArtShape',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SmartArtShape', shape_type=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SmartArtShape', shape_type=None):  # noqa: E501
         """SmartArtShape - a model defined in Swagger"""  # noqa: E501
-        super(SmartArtShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(SmartArtShape, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
         self.type = 'SmartArtShape'
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -70,14 +71,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -88,17 +90,17 @@
         'sections': 'sections'
     }
 
     type_determiners = {
         'type': 'SummaryZoomFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SummaryZoomFrame', zoom_layout=None, sections=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SummaryZoomFrame', zoom_layout=None, sections=None):  # noqa: E501
         """SummaryZoomFrame - a model defined in Swagger"""  # noqa: E501
-        super(SummaryZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(SummaryZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._zoom_layout = None
         self._sections = None
         self.type = 'SummaryZoomFrame'
 
         if zoom_layout is not None:
             self.zoom_layout = zoom_layout
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -76,14 +77,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -100,17 +102,17 @@
         'description': 'description'
     }
 
     type_determiners = {
         'type': 'SummaryZoomSection',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SummaryZoomSection', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_section_index=None, title=None, description=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='SummaryZoomSection', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_section_index=None, title=None, description=None):  # noqa: E501
         """SummaryZoomSection - a model defined in Swagger"""  # noqa: E501
-        super(SummaryZoomSection, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration, target_section_index)
+        super(SummaryZoomSection, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration, target_section_index)
 
         self._title = None
         self._description = None
         self.type = 'SummaryZoomSection'
 
         if title is not None:
             self.title = title
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -78,14 +79,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -104,17 +106,17 @@
         'vertical_banding': 'verticalBanding'
     }
 
     type_determiners = {
         'type': 'Table',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Table', style=None, rows=None, columns=None, first_col=None, first_row=None, horizontal_banding=None, last_col=None, last_row=None, right_to_left=None, vertical_banding=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Table', style=None, rows=None, columns=None, first_col=None, first_row=None, horizontal_banding=None, last_col=None, last_row=None, right_to_left=None, vertical_banding=None):  # noqa: E501
         """Table - a model defined in Swagger"""  # noqa: E501
-        super(Table, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(Table, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._style = None
         self._rows = None
         self._columns = None
         self._first_col = None
         self._first_row = None
         self._horizontal_banding = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell_merge_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_merge_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table_cell_split_type.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table_cell_split_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/task.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/text_items.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/text_items.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/vba_module.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_module.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/vba_project.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_project.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/vba_reference.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/vba_reference.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/video_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -79,14 +80,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -106,17 +108,17 @@
         'trim_from_end': 'trimFromEnd'
     }
 
     type_determiners = {
         'type': 'VideoFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='VideoFrame', shape_type=None, full_screen_mode=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, rewind_video=None, volume=None, base64_data=None, picture_fill_format=None, trim_from_start=None, trim_from_end=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='VideoFrame', shape_type=None, full_screen_mode=None, hide_at_showing=None, play_loop_mode=None, play_mode=None, rewind_video=None, volume=None, base64_data=None, picture_fill_format=None, trim_from_start=None, trim_from_end=None):  # noqa: E501
         """VideoFrame - a model defined in Swagger"""  # noqa: E501
-        super(VideoFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
+        super(VideoFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, shape_type)
 
         self._full_screen_mode = None
         self._hide_at_showing = None
         self._play_loop_mode = None
         self._play_mode = None
         self._rewind_video = None
         self._volume = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -74,14 +75,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -96,17 +98,17 @@
         'target_slide_index': 'targetSlideIndex'
     }
 
     type_determiners = {
         'type': 'ZoomFrame',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='ZoomFrame', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_slide_index=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='ZoomFrame', image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None, target_slide_index=None):  # noqa: E501
         """ZoomFrame - a model defined in Swagger"""  # noqa: E501
-        super(ZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration)
+        super(ZoomFrame, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type, image_type, return_to_parent, show_background, image, transition_duration)
 
         self._target_slide_index = None
         self.type = 'ZoomFrame'
 
         if target_slide_index is not None:
             self.target_slide_index = target_slide_index
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-24.3.0/asposeslidescloud/models/zoom_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         'alternate_links': 'list[ResourceUri]',
         'name': 'str',
         'width': 'float',
         'height': 'float',
         'alternative_text': 'str',
         'alternative_text_title': 'str',
         'hidden': 'bool',
+        'is_decorative': 'bool',
         'x': 'float',
         'y': 'float',
         'z_order_position': 'int',
         'fill_format': 'FillFormat',
         'effect_format': 'EffectFormat',
         'three_d_format': 'ThreeDFormat',
         'line_format': 'LineFormat',
@@ -73,14 +74,15 @@
         'alternate_links': 'alternateLinks',
         'name': 'name',
         'width': 'width',
         'height': 'height',
         'alternative_text': 'alternativeText',
         'alternative_text_title': 'alternativeTextTitle',
         'hidden': 'hidden',
+        'is_decorative': 'isDecorative',
         'x': 'x',
         'y': 'y',
         'z_order_position': 'zOrderPosition',
         'fill_format': 'fillFormat',
         'effect_format': 'effectFormat',
         'three_d_format': 'threeDFormat',
         'line_format': 'lineFormat',
@@ -93,17 +95,17 @@
         'image': 'image',
         'transition_duration': 'transitionDuration'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type=None, image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type=None, image_type=None, return_to_parent=None, show_background=None, image=None, transition_duration=None):  # noqa: E501
         """ZoomObject - a model defined in Swagger"""  # noqa: E501
-        super(ZoomObject, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
+        super(ZoomObject, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._image_type = None
         self._return_to_parent = None
         self._show_background = None
         self._image = None
         self._transition_duration = None
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-24.3.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud/rest.py` & `asposeslidescloud-24.3.0/asposeslidescloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-24.3.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 24.2.0
+Version: 24.3.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,27 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.3
+
+* Added Markdown (**Md**) to the list of allowed export formats.
+* Added **DeletePictureCroppedAreas** method to delete cropped areas of pictures.
+* Added **SlidesLayoutOptions** property to **PdfExportOptions**, **HtmlExportOptions**, **TiffExportOptions** and **ImageExportOptions** classes. You can use it to specify handout or notes/comments layouting options.
+* Added **AnimateTextType** enum property to **Effect** class.
+* Added **NotesCommentsLayouting** property to **Html5ExportOptions** class.
+* Added **BwConversionMode** property to **TiffExportOptions** class.
+* Added **EmbedImages** boolean property to **Html5ExportOptions** class.
+* Added **ShowMediaControls** boolean property to **SlideShowProperties** class.
+* Added **IsDecorative** boolean property to **ShapeBase** class.
+
+
 ## Enhancements in Version 24.2
 
 * Added **GetCommentAuthors** method to get list of comment authors.
 
 ## Enhancements in Version 24.1
 
 * Added **GetAvailableFonts** method to get list of installed system & custom fonts.
```

### Comparing `asposeslidescloud-24.2.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-24.3.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 asposeslidescloud/models/glow_effect.py
 asposeslidescloud/models/gradient_fill.py
 asposeslidescloud/models/gradient_fill_stop.py
 asposeslidescloud/models/graphical_object.py
 asposeslidescloud/models/gray_scale_effect.py
 asposeslidescloud/models/group_shape.py
 asposeslidescloud/models/grouping_character_element.py
+asposeslidescloud/models/handout_layouting_options.py
 asposeslidescloud/models/header_footer.py
 asposeslidescloud/models/hsl_effect.py
 asposeslidescloud/models/html5_export_options.py
 asposeslidescloud/models/html_export_options.py
 asposeslidescloud/models/hyperlink.py
 asposeslidescloud/models/i_shape_export_options.py
 asposeslidescloud/models/image.py
@@ -142,14 +143,15 @@
 asposeslidescloud/models/matrix_element.py
 asposeslidescloud/models/merge.py
 asposeslidescloud/models/merging_source.py
 asposeslidescloud/models/move_to_path_segment.py
 asposeslidescloud/models/nary_operator_element.py
 asposeslidescloud/models/no_fill.py
 asposeslidescloud/models/normal_view_restored_properties.py
+asposeslidescloud/models/notes_comments_layouting_options.py
 asposeslidescloud/models/notes_slide.py
 asposeslidescloud/models/notes_slide_export_format.py
 asposeslidescloud/models/notes_slide_header_footer.py
 asposeslidescloud/models/object_exist.py
 asposeslidescloud/models/ole_object_frame.py
 asposeslidescloud/models/one_value_chart_data_point.py
 asposeslidescloud/models/one_value_series.py
@@ -221,14 +223,15 @@
 asposeslidescloud/models/slide_export_format.py
 asposeslidescloud/models/slide_modern_comment.py
 asposeslidescloud/models/slide_properties.py
 asposeslidescloud/models/slide_replace_result.py
 asposeslidescloud/models/slide_show_properties.py
 asposeslidescloud/models/slide_show_transition.py
 asposeslidescloud/models/slides.py
+asposeslidescloud/models/slides_layout_options.py
 asposeslidescloud/models/smart_art.py
 asposeslidescloud/models/smart_art_node.py
 asposeslidescloud/models/smart_art_shape.py
 asposeslidescloud/models/soft_edge_effect.py
 asposeslidescloud/models/solid_fill.py
 asposeslidescloud/models/special_slide_type.py
 asposeslidescloud/models/split_document_result.py
```

### Comparing `asposeslidescloud-24.2.0/setup.py` & `asposeslidescloud-24.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="24.2.0",
+    version="24.3.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

