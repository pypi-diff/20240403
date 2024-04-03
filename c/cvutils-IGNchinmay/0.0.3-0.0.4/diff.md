# Comparing `tmp/cvutils_IGNchinmay-0.0.3.tar.gz` & `tmp/cvutils_IGNchinmay-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvutils_IGNchinmay-0.0.3.tar", last modified: Mon Apr  1 11:25:40 2024, max compression
+gzip compressed data, was "cvutils_IGNchinmay-0.0.4.tar", last modified: Wed Apr  3 08:39:29 2024, max compression
```

## Comparing `cvutils_IGNchinmay-0.0.3.tar` & `cvutils_IGNchinmay-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,89 @@
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    11357 2024-04-01 07:09:57.000000 cvutils_IGNchinmay-0.0.3/LICENSE.txt
--rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1002 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/PKG-INFO
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       63 2024-04-01 07:16:41.000000 cvutils_IGNchinmay-0.0.3/README.md
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.893171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      763 2024-04-01 10:53:21.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/__init__.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    37749 2024-04-01 10:33:02.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/contour_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     9802 2024-04-01 06:47:18.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/draw_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    14245 2024-04-01 10:26:00.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/file_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4775 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/geom_utils.py
--rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    24718 2024-04-01 10:33:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/img_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3062 2024-03-26 11:13:44.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/json_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5694 2024-04-01 10:33:55.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/labelme_utils.py
--rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    20543 2024-04-01 10:26:11.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/mouse_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2094 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/multi_process_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12934 2024-04-01 10:54:37.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/show_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3232 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/system_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    19654 2024-04-01 10:30:03.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/transform_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1756 2024-03-26 11:27:12.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/typehint_utils.py
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      811 2024-04-01 10:49:44.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/__init__.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2927 2024-04-01 10:24:45.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/dump_frames.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2616 2024-04-01 10:24:54.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/exif_utils.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3760 2024-04-01 10:25:04.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/folder_reader.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3305 2024-04-01 10:25:14.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/play_video.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12840 2024-04-01 10:25:24.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_reader.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     8359 2024-04-01 10:25:35.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_sync.py
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4389 2024-04-01 10:25:46.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_writer.py
-drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/
--rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1002 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/PKG-INFO
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1114 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/SOURCES.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        1 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/dependency_links.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      161 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/requires.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       19 2024-04-01 11:25:40.000000 cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay.egg-info/top_level.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      730 2024-04-01 10:17:39.000000 cvutils_IGNchinmay-0.0.3/pyproject.toml
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      160 2024-04-01 11:00:55.000000 cvutils_IGNchinmay-0.0.3/requirements.txt
--rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       38 2024-04-01 11:25:40.897171 cvutils_IGNchinmay-0.0.3/setup.cfg
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.805602 cvutils_IGNchinmay-0.0.4/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    11357 2024-04-01 07:09:57.000000 cvutils_IGNchinmay-0.0.4/LICENSE.txt
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1311 2024-04-03 08:39:29.805602 cvutils_IGNchinmay-0.0.4/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       70 2024-04-03 08:39:03.000000 cvutils_IGNchinmay-0.0.4/README.md
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.797602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3297 2024-04-03 08:20:16.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4159 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/algo_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.801602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/autoui_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      776 2024-04-03 06:04:12.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/autoui_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3895 2024-04-03 05:56:57.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/autoui_utils/autogui_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    20711 2024-04-03 06:00:45.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/autoui_utils/autotest_recplayback.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2514 2024-04-03 06:01:31.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/autoui_utils/calculator_demo.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.801602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      871 2024-04-03 06:11:38.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1412 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/angle_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     6410 2024-04-03 06:04:07.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/charuco_mono_calib.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    16534 2024-04-03 06:04:50.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/charuco_stereo_calib.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    14875 2024-04-03 06:05:11.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/infer_depth.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     6011 2024-04-03 06:06:43.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/mono_calib.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3800 2024-04-03 06:06:55.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/mono_dump.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     6352 2024-04-03 06:07:05.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/mono_error_calc.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3677 2024-04-03 06:07:30.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/mono_undistort.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    44100 2024-04-03 06:07:41.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/optimize_depth.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     7942 2024-04-03 06:07:51.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/point_depth_demo.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    10619 2024-04-03 06:08:35.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/pose_estimate.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     7768 2024-04-03 06:09:11.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/rs_crop_dump.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    10702 2024-04-03 06:10:09.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/stereo_3d_error_calc.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    14600 2024-04-03 06:10:19.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/stereo_calib.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4971 2024-04-03 06:10:28.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/stereo_dump.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    10097 2024-04-03 06:10:38.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/stereo_error_calc.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5697 2024-04-03 06:10:50.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/calib_utils/stereo_record.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.801602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/cam_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      871 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/cam_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5775 2024-04-03 06:12:04.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/cam_utils/camera_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1676 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/cam_utils/gopro_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     6950 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/cam_utils/realsense_reader.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    12764 2024-04-03 08:21:04.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/clone_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5357 2024-04-03 06:47:37.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/config_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    37749 2024-04-01 10:33:02.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/contour_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4201 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/docker_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     9802 2024-04-01 06:47:18.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/draw_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    14245 2024-04-01 10:26:00.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/file_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1094 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/filter_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     8746 2024-04-03 06:48:00.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/fisheye_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4775 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/geom_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5660 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/gpu_utils.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    24718 2024-04-01 10:33:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/img_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3062 2024-03-26 11:13:44.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/json_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1663 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/keyboard_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5694 2024-04-01 10:33:55.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/labelme_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    10540 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/license_check.py
+-rwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)    20543 2024-04-01 10:26:11.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/mouse_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2094 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/multi_process_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.801602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/o3d_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/o3d_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1196 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/o3d_utils/plot_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     8528 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/o3d_utils/registration_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.801602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      788 2024-04-03 06:36:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4541 2024-04-03 06:36:45.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/ecc_register.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    18584 2024-04-03 06:36:53.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/keypoint_register.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1845 2024-04-03 06:37:00.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/register_abstract.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1287 2024-04-03 06:37:11.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/registration/register_wrapper.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12934 2024-04-01 10:54:37.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/show_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5265 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/ssh_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3232 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/system_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      993 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/timer_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    19654 2024-04-01 10:30:03.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/transform_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     5449 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/transfrom_crops.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1756 2024-03-26 11:27:12.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/typehint_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.805602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      811 2024-04-01 10:49:44.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/__init__.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2927 2024-04-01 10:24:45.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/dump_frames.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     2616 2024-04-01 10:24:54.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/exif_utils.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3760 2024-04-01 10:25:04.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/folder_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3305 2024-04-01 10:25:14.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/play_video.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)    12840 2024-04-01 10:25:24.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_reader.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     8359 2024-04-01 10:25:35.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_sync.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     4389 2024-04-01 10:25:46.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_writer.py
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3435 2024-04-01 09:49:27.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/yaml_utils.py
+drwxrwxr-x   0 chinmayanandas  (1001) chinmayanandas  (1001)        0 2024-04-03 08:39:29.805602 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/
+-rw-r--r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     1311 2024-04-03 08:39:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)     3204 2024-04-03 08:39:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)        1 2024-04-03 08:39:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      283 2024-04-03 08:39:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/requires.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       19 2024-04-03 08:39:29.000000 cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay.egg-info/top_level.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      730 2024-04-03 08:38:44.000000 cvutils_IGNchinmay-0.0.4/pyproject.toml
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)      282 2024-04-03 08:36:39.000000 cvutils_IGNchinmay-0.0.4/requirements.txt
+-rw-rw-r--   0 chinmayanandas  (1001) chinmayanandas  (1001)       38 2024-04-03 08:39:29.805602 cvutils_IGNchinmay-0.0.4/setup.cfg
```

### Comparing `cvutils_IGNchinmay-0.0.3/LICENSE.txt` & `cvutils_IGNchinmay-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/contour_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/contour_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/draw_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/draw_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/file_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/file_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/geom_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/geom_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/img_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/img_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/json_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/labelme_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/labelme_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/mouse_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/mouse_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/multi_process_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/multi_process_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/show_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/show_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/system_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/system_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/transform_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/transform_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/typehint_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/typehint_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/__init__.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/dump_frames.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/dump_frames.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/exif_utils.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/exif_utils.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/folder_reader.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/folder_reader.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/play_video.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/play_video.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_reader.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_reader.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_sync.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_sync.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/cvutils_IGNchinmay/video_utils/video_writer.py` & `cvutils_IGNchinmay-0.0.4/cvutils_IGNchinmay/video_utils/video_writer.py`

 * *Files identical despite different names*

### Comparing `cvutils_IGNchinmay-0.0.3/pyproject.toml` & `cvutils_IGNchinmay-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cvutils_IGNchinmay"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["dependencies"]              #used for requiremnts.txt file
```

