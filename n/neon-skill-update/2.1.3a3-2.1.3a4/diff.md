# Comparing `tmp/neon-skill-update-2.1.3a3.tar.gz` & `tmp/neon-skill-update-2.1.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-update-2.1.3a3.tar", last modified: Mon Mar 11 23:45:50 2024, max compression
+gzip compressed data, was "neon-skill-update-2.1.3a4.tar", last modified: Wed Apr  3 00:08:01 2024, max compression
```

## Comparing `neon-skill-update-2.1.3a3.tar` & `neon-skill-update-2.1.3a4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.774740 neon-skill-update-2.1.3a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-11 23:45:50.774740 neon-skill-update-2.1.3a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.762740 neon-skill-update-2.1.3a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.762740 neon-skill-update-2.1.3a3/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.770740 neon-skill-update-2.1.3a3/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/alpha.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/ask_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/ask_download_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/ask_overwrite_drive.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/ask_update_anyways.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/ask_update_configuration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/beta.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/check_error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/check_updates.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/confirm_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/confirm_no_change_update_track.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/core_version.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/downloading_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/drive_instructions.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/error_installing_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/error_offline.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/error_unknown.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/error_updating_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/help_online.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/help_support.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/no_image_file.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/no_valid_device.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/not_updating.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_download_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_download_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_downloading_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_downloading_update.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_installation_complete.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_installation_failed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_os_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_update_available.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_update_failure.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_update_success.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/notify_writing_image.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/point.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/starting_installation.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/starting_update.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/up_to_date.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_continuing.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_core.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_in_progress.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_initramfs_success.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_os.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_restarting.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_system.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/update_track_already_set.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/word_beta.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/dialog/word_stable.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.770740 neon-skill-update-2.1.3a3/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/intent/core_version.intent
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/intent/update_configuration.intent
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/intent/update_device.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.770740 neon-skill-update-2.1.3a3/locale/en-us/vocab/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/beta.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/change.voc
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/create.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/media.voc
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/os.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/stable.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/locale/en-us/vocab/updates.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.774740 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-11 23:45:50.000000 neon-skill-update-2.1.3a3/neon_skill_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 23:45:50.774740 neon-skill-update-2.1.3a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 23:45:50.774740 neon-skill-update-2.1.3a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-03-11 23:45:47.000000 neon-skill-update-2.1.3a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.820054 neon-skill-update-2.1.3a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-03 00:08:01.820054 neon-skill-update-2.1.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    31862 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.808054 neon-skill-update-2.1.3a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.808054 neon-skill-update-2.1.3a4/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.816054 neon-skill-update-2.1.3a4/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/alpha.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/ask_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/ask_download_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/ask_overwrite_drive.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/ask_update_anyways.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/ask_update_configuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/check_error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/check_updates.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/confirm_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/confirm_no_change_update_track.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/core_version.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/downloading_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/drive_instructions.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/error_installing_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/error_offline.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/error_unknown.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/error_updating_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/help_online.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/help_support.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/no_image_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/no_valid_device.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/not_updating.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_download_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_download_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_downloading_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_downloading_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_installation_complete.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_installation_failed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_os_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_update_available.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_update_failure.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_update_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/notify_writing_image.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/point.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/starting_installation.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/starting_update.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/up_to_date.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_continuing.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_core.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_in_progress.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_initramfs_success.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_os.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_restarting.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_system.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/update_track_already_set.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/word_beta.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/dialog/word_stable.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.816054 neon-skill-update-2.1.3a4/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/intent/core_version.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/intent/update_configuration.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/intent/update_device.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.816054 neon-skill-update-2.1.3a4/locale/en-us/vocab/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/beta.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/change.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/create.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/media.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/os.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/stable.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/locale/en-us/vocab/updates.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.820054 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 00:08:01.000000 neon-skill-update-2.1.3a4/neon_skill_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:08:01.820054 neon-skill-update-2.1.3a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:08:01.820054 neon-skill-update-2.1.3a4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    21777 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 00:07:57.000000 neon-skill-update-2.1.3a4/version.py
```

### Comparing `neon-skill-update-2.1.3a3/LICENSE.md` & `neon-skill-update-2.1.3a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/PKG-INFO` & `neon-skill-update-2.1.3a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 2.1.3a3
+Version: 2.1.3a4
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-2.1.3a3/README.md` & `neon-skill-update-2.1.3a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/__init__.py` & `neon-skill-update-2.1.3a4/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,42 +53,43 @@
         self._updating = False
 
         self.add_event('mycroft.ready', self._on_ready)
         self.add_event("update.gui.continue_installation",
                        self.continue_os_installation)
         self.add_event("update.gui.finish_installation",
                        self.finish_os_installation)
-        self.add_event("update.gui.install_update", self.handle_update_device)
+        self.add_event("update.gui.install_update",
+                       self.handle_update_device)
 
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
                                    gui_before_load=False,
                                    requires_internet=True,
                                    requires_network=True,
                                    requires_gui=False,
                                    no_internet_fallback=False,
                                    no_network_fallback=False,
                                    no_gui_fallback=True)
 
     @property
-    def current_ver(self):
+    def current_ver(self) -> str:
         if not self._current_ver:
             message = (dig_for_message() or Message(""))
             if self.os_updates_supported:
                 resp = self.bus.wait_for_response(message.forward(
-                    "neon.device_updater.get_build_info"))
+                    "neon.device_updater.get_build_info"), timeout=15)
                 if resp:
                     self._current_ver = resp.data.get("build_version") or \
                         resp.data.get("core", {}).get("version")
                     LOG.info(f"Got build version: {self._current_ver}")
                     return self._current_ver
             resp = self.bus.wait_for_response(message.forward(
-                "neon.core_updater.get_version"))
+                "neon.core_updater.get_version"), timeout=15)
             if resp:
                 self._current_ver = resp.data.get("version")
         if not self._current_ver:
             LOG.error("Installed core version unknown!")
         return self._current_ver
 
     @current_ver.setter
@@ -225,15 +226,19 @@
             self._check_latest_release(message)
 
         update_stat = self._check_update_status()
         LOG.debug(f"Update status is {update_stat}")
         if not update_stat:
             # No update was attempted
             return
-        speak_version = self.pronounce_version(self.current_ver)
+        try:
+            speak_version = self.pronounce_version(self.current_ver)
+        except Exception as e:
+            LOG.error(e)
+            speak_version = ""
         if update_stat is True:
             LOG.debug("Update success")
             self.speak_dialog("notify_update_success",
                               {"version": speak_version})
         elif update_stat is False:
             LOG.warning("Update failed")
             self.speak_dialog("notify_update_failure",
```

### Comparing `neon-skill-update-2.1.3a3/neon_skill_update.egg-info/PKG-INFO` & `neon-skill-update-2.1.3a4/neon_skill_update.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-update
-Version: 2.1.3a3
+Version: 2.1.3a4
 Home-page: https://github.com/NeonGeckoCom/skill-update
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE.md
```

### Comparing `neon-skill-update-2.1.3a3/neon_skill_update.egg-info/SOURCES.txt` & `neon-skill-update-2.1.3a4/neon_skill_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/setup.py` & `neon-skill-update-2.1.3a4/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/skill.json` & `neon-skill-update-2.1.3a4/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/test/test_skill.py` & `neon-skill-update-2.1.3a4/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-update-2.1.3a3/version.py` & `neon-skill-update-2.1.3a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "2.1.3a3"
+__version__ = "2.1.3a4"
```

