# Comparing `tmp/neon-skill-audio_record-1.0.1.tar.gz` & `tmp/neon-skill-audio_record-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-audio_record-1.0.1.tar", last modified: Wed Apr  3 18:31:57 2024, max compression
+gzip compressed data, was "neon-skill-audio_record-1.0.1a1.tar", last modified: Tue Feb  6 01:04:05 2024, max compression
```

## Comparing `neon-skill-audio_record-1.0.1.tar` & `neon-skill-audio_record-1.0.1a1.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.724989 neon-skill-audio_record-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 18:31:57.724989 neon-skill-audio_record-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.692988 neon-skill-audio_record-1.0.1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.692988 neon-skill-audio_record-1.0.1/locale/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ca-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.696988 neon-skill-audio_record-1.0.1/locale/cs-cz/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/cs-cz/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.696988 neon-skill-audio_record-1.0.1/locale/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/da-dk/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.700988 neon-skill-audio_record-1.0.1/locale/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/de-de/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.700988 neon-skill-audio_record-1.0.1/locale/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/el-gr/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.704989 neon-skill-audio_record-1.0.1/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Audio.voc
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/AudioRecordSkillDeleteVerb.voc
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/AudioRecordSkillKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/AudioRecordSkillListKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/AudioRecordSkillPlayVerb.voc
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/AudioRecordSkillStopVerb.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/ConfirmFilename.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/ConfirmNo.voc
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/ConfirmYes.voc
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/FileExists.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Record.voc
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/ResumeKeyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.start.duration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.stop.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/en-us/audio.record.stop.play.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.708989 neon-skill-audio_record-1.0.1/locale/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.708989 neon-skill-audio_record-1.0.1/locale/es-lm/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/es-lm/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.708989 neon-skill-audio_record-1.0.1/locale/eu-eu/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/eu-eu/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.712989 neon-skill-audio_record-1.0.1/locale/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/fr-fr/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.712989 neon-skill-audio_record-1.0.1/locale/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/gl-es/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.716989 neon-skill-audio_record-1.0.1/locale/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/hu-hu/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.716989 neon-skill-audio_record-1.0.1/locale/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/it-it/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.716989 neon-skill-audio_record-1.0.1/locale/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/nl-nl/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.720989 neon-skill-audio_record-1.0.1/locale/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/pt-br/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.720989 neon-skill-audio_record-1.0.1/locale/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/ru-ru/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.724989 neon-skill-audio_record-1.0.1/locale/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/Delete.voc
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/Play.voc
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/PlayRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/Recording.voc
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/StartRecording.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/audio.record.disk.full.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/audio.record.no.recording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/audio.record.removed.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/locale/sv-se/audio.record.start.duration.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:31:57.724989 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:31:57.000000 neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:31:57.724989 neon-skill-audio_record-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-03 18:31:54.000000 neon-skill-audio_record-1.0.1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    25739 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.957392 neon-skill-audio_record-1.0.1a1/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.961392 neon-skill-audio_record-1.0.1a1/locale/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ca-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.961392 neon-skill-audio_record-1.0.1a1/locale/cs-cz/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/cs-cz/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.961392 neon-skill-audio_record-1.0.1a1/locale/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/da-dk/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.965392 neon-skill-audio_record-1.0.1a1/locale/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/de-de/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.965392 neon-skill-audio_record-1.0.1a1/locale/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/el-gr/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.969392 neon-skill-audio_record-1.0.1a1/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Audio.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/AudioRecordSkillDeleteVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/AudioRecordSkillKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/AudioRecordSkillListKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/AudioRecordSkillPlayVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/AudioRecordSkillStopVerb.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/ConfirmFilename.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/ConfirmNo.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/ConfirmYes.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/FileExists.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Record.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/ResumeKeyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.start.duration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.stop.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/en-us/audio.record.stop.play.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.969392 neon-skill-audio_record-1.0.1a1/locale/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.969392 neon-skill-audio_record-1.0.1a1/locale/es-lm/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/es-lm/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.973392 neon-skill-audio_record-1.0.1a1/locale/eu-eu/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/eu-eu/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.973392 neon-skill-audio_record-1.0.1a1/locale/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/fr-fr/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.973392 neon-skill-audio_record-1.0.1a1/locale/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/gl-es/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.973392 neon-skill-audio_record-1.0.1a1/locale/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/hu-hu/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.977392 neon-skill-audio_record-1.0.1a1/locale/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/it-it/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.977392 neon-skill-audio_record-1.0.1a1/locale/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/nl-nl/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.977392 neon-skill-audio_record-1.0.1a1/locale/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/pt-br/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/locale/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/ru-ru/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/locale/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/Delete.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/Play.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/PlayRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/Recording.voc
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/StartRecording.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/audio.record.disk.full.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/audio.record.no.recording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/audio.record.removed.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/locale/sv-se/audio.record.start.duration.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6351 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-06 01:04:05.000000 neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:04:05.981392 neon-skill-audio_record-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:04:02.000000 neon-skill-audio_record-1.0.1a1/version.py
```

### Comparing `neon-skill-audio_record-1.0.1/LICENSE` & `neon-skill-audio_record-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/LICENSE.md` & `neon-skill-audio_record-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/PKG-INFO` & `neon-skill-audio_record-1.0.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-audio_record
-Version: 1.0.1
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-audio_record
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-audio_record-1.0.1/README.md` & `neon-skill-audio_record-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/__init__.py` & `neon-skill-audio_record-1.0.1a1/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/locale/eu-eu/PlayRecording.intent` & `neon-skill-audio_record-1.0.1a1/locale/eu-eu/PlayRecording.intent`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/PKG-INFO` & `neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-audio-record
-Version: 1.0.1
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-audio_record
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.md
```

### Comparing `neon-skill-audio_record-1.0.1/neon_skill_audio_record.egg-info/SOURCES.txt` & `neon-skill-audio_record-1.0.1a1/neon_skill_audio_record.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/setup.py` & `neon-skill-audio_record-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/skill.json` & `neon-skill-audio_record-1.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-audio_record-1.0.1/version.py` & `neon-skill-audio_record-1.0.1a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1"
+__version__ = "1.0.1a1"
```

