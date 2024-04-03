# Comparing `tmp/rethink-note-0.2.3.tar.gz` & `tmp/rethink-note-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rethink-note-0.2.3.tar", last modified: Thu Mar 28 17:53:09 2024, max compression
+gzip compressed data, was "rethink-note-0.2.4.tar", last modified: Wed Apr  3 16:31:12 2024, max compression
```

## Comparing `rethink-note-0.2.3.tar` & `rethink-note-0.2.4.tar`

### file list

```diff
@@ -1,450 +1,461 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.456378 rethink-note-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-28 17:53:05.000000 rethink-note-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-03-28 17:53:09.456378 rethink-note-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-03-28 17:53:05.000000 rethink-note-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-03-28 17:53:05.000000 rethink-note-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-28 17:53:09.456378 rethink-note-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.344378 rethink-note-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.348378 rethink-note-0.2.3/src/rethink/
--rw-r--r--   0 runner    (1001) docker     (127)     4085 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/.env.local
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.348378 rethink-note-0.2.3/src/rethink/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.348378 rethink-note-0.2.3/src/rethink/controllers/files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/files/upload_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/controllers/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/node/node_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/node/trash_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/controllers/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/schemas/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/controllers/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/search/node_search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/controllers/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/user/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/user/user_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/controllers/verify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/verify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/controllers/verify/v_captcha.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.352378 rethink-note-0.2.3/src/rethink/core/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/get.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/importing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6016 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/text/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/text/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/files/importing/sync_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/sync_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/importing/sync_tasks/editor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/files/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    14515 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/core/verify/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/verify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/verify/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/core/verify/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.356378 rethink-note-0.2.3/src/rethink/depend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.360378 rethink-note-0.2.3/src/rethink/depend/mongita/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/command_cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/database.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.360378 rethink-note-0.2.3/src/rethink/depend/mongita/engines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/engines/disk_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/engines/engine_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/engines/memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/mongita_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/mongitasync.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/read_concern.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/mongita/write_concern.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.360378 rethink-note-0.2.3/src/rethink/depend/sso/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/facebook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/google.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/microsoft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/depend/sso/qq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.364378 rethink-note-0.2.3/src/rethink/dist-local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.364378 rethink-note-0.2.3/src/rethink/dist-local/css/
--rw-r--r--   0 runner    (1001) docker     (127)   169947 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/css/app.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.340378 rethink-note-0.2.3/src/rethink/dist-local/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.340378 rethink-note-0.2.3/src/rethink/dist-local/dist/css/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.364378 rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/ant-design.css
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/light.css
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/wechat.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.364378 rethink-note-0.2.3/src/rethink/dist-local/dist/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.368378 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/
--rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/b3log.png
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/chainbook.png
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/doge.png
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/hacpai.png
--rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/huaji.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/latke.png
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/liandi.png
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/lute.png
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/octocat.png
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/pipe.png
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/siyuan.png
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/solo.png
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/sym.png
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/trollface.png
--rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/vditor.png
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/wide.png
--rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/wulian.png
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/img-loading.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.344378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.368378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/abcjs/
--rw-r--r--   0 runner    (1001) docker     (127)   363243 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/abcjs/abcjs_basic.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.368378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/echarts/
--rw-r--r--   0 runner    (1001) docker     (127)   762119 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/echarts/echarts.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.368378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/flowchart.js/
--rw-r--r--   0 runner    (1001) docker     (127)   125802 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/flowchart.js/flowchart.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.376378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/graphviz/
--rw-r--r--   0 runner    (1001) docker     (127)  4423759 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/graphviz/full.render.js
--rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/graphviz/viz.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.376378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/
--rw-r--r--   0 runner    (1001) docker     (127)   376423 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/highlight.pack.js
--rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/solidity.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.384378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/abap.css
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/algol.css
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/algol_nu.css
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/ant-design.css
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/arduino.css
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/autumn.css
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/borland.css
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/bw.css
--rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/colorful.css
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/dracula.css
--rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/emacs.css
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/friendly.css
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/fruity.css
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/github.css
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/igor.css
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/lovelace.css
--rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/manni.css
--rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/monokai.css
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/monokailight.css
--rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/murphy.css
--rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/native.css
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/pastie.css
--rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/perldoc.css
--rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/pygments.css
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/rainbow_dash.css
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/rrt.css
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark256.css
--rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/swapoff.css
--rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/tango.css
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/trac.css
--rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/vim.css
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/vs.css
--rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/xcode.css
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/yul.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.388378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/en_US.js
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/fr_FR.js
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ja_JP.js
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ko_KR.js
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/pt_BR.js
--rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ru_RU.js
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/sv_SE.js
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/zh_CN.js
--rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/zh_TW.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.388378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    42983 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/icons/ant.js
--rw-r--r--   0 runner    (1001) docker     (127)    20896 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/icons/material.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.388378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.400378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/katex.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   277038 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/katex.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/mhchem.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.400378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/lute/
--rw-r--r--   0 runner    (1001) docker     (127)  3785836 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/lute/lute.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.408378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/
--rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/katex.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   824275 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/markmap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/prism.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.408378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.412378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/assistive-mml.js
--rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/complexity.js
--rw-r--r--   0 runner    (1001) docker     (127)    32640 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/explorer.js
--rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/semantic-enrich.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.416378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/
--rw-r--r--   0 runner    (1001) docker     (127)   106067 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/asciimath.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.416378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/mml/
--rw-r--r--   0 runner    (1001) docker     (127)    33265 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/mml/entities.js
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/mml.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.344378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.420378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/action.js
--rw-r--r--   0 runner    (1001) docker     (127)   147205 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/all-packages.js
--rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/ams.js
--rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/amscd.js
--rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/autoload.js
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bbox.js
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/boldsymbol.js
--rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/braket.js
--rw-r--r--   0 runner    (1001) docker     (127)    17174 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bussproofs.js
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/cancel.js
--rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/color.js
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/colorV2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/configMacros.js
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/enclose.js
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/extpfeil.js
--rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/html.js
--rw-r--r--   0 runner    (1001) docker     (127)    36819 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/mhchem.js
--rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/newcommand.js
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noerrors.js
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noundefined.js
--rw-r--r--   0 runner    (1001) docker     (127)    23443 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/physics.js
--rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/require.js
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/tagFormat.js
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/textmacros.js
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/unicode.js
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/verb.js
--rw-r--r--   0 runner    (1001) docker     (127)   129130 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex-base.js
--rw-r--r--   0 runner    (1001) docker     (127)   270488 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex-full.js
--rw-r--r--   0 runner    (1001) docker     (127)   163954 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.420378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.428378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/
--rw-r--r--   0 runner    (1001) docker     (127)   326869 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/de.js
--rw-r--r--   0 runner    (1001) docker     (127)   423424 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/en.js
--rw-r--r--   0 runner    (1001) docker     (127)   326446 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/es.js
--rw-r--r--   0 runner    (1001) docker     (127)   321576 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/fr.js
--rw-r--r--   0 runner    (1001) docker     (127)  1795679 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/mathmaps_ie.js
--rw-r--r--   0 runner    (1001) docker     (127)   301796 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/nemeth.js
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/sre-node.js
--rw-r--r--   0 runner    (1001) docker     (127)   874345 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/sre_browser.js
--rw-r--r--   0 runner    (1001) docker     (127)  1811419 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/tex-svg-full.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.428378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mermaid/
--rw-r--r--   0 runner    (1001) docker     (127)  1084448 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/mermaid/mermaid.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.428378 rethink-note-0.2.3/src/rethink/dist-local/dist/js/plantuml/
--rw-r--r--   0 runner    (1001) docker     (127)    29433 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/dist/js/plantuml/plantuml-encoder.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    38078 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.436378 rethink-note-0.2.3/src/rethink/dist-local/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/2023_Obsidian_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/back.svg
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/checked-success.svg
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/chevron-double-left.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/circle-user.svg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/cross.svg
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/diagonal-arrow-right-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/dropdown-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/expand-down.svg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/expand-up.svg
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/expand.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/eye-closed.svg
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/eye-open.svg
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/github-mark.svg
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/home.svg
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/import.svg
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/list.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/loading-dots.gif
--rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/loading.gif
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/menu.svg
--rw-r--r--   0 runner    (1001) docker     (127)    85421 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/morvanQR.png
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/node.svg
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/plugin.svg
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/plus.svg
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/recentoutline.svg
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/return-arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/search.svg
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/sort.svg
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/tab.svg
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/text.svg
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/three-dots-vertical.svg
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/tick.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/trash.svg
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/upload.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/view-grid.svg
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/img/white-cross.svg
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.440378 rethink-note-0.2.3/src/rethink/dist-local/js/
--rw-r--r--   0 runner    (1001) docker     (127)  1821997 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/js/app.js
--rw-r--r--   0 runner    (1001) docker     (127)  1266654 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/js/chunk-vendors.js
--rw-r--r--   0 runner    (1001) docker     (127)   121728 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/js/highlight.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.440378 rethink-note-0.2.3/src/rethink/dist-local/media/
--rw-r--r--   0 runner    (1001) docker     (127)  3429085 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/dist-local/media/demo.mp4
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14446 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/coll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/db_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/indexing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/models/search_engine/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/baidu_stopwords.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/cn_stopwords.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    22343 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/engine_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/search_engine/engine_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/models/tps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.344378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/_static/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/templates/side.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.344378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/_static/image/
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/_static/image/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.448378 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/templates/side.html
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/register.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.452378 rethink-note-0.2.3/src/rethink/plugins/schedule/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/schedule/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/plugins/schedule/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.452378 rethink-note-0.2.3/src/rethink/routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/trash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/routes/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8321 2024-03-28 17:53:05.000000 rethink-note-0.2.3/src/rethink/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.456378 rethink-note-0.2.3/src/rethink_note.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-03-28 17:53:09.000000 rethink-note-0.2.3/src/rethink_note.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19085 2024-03-28 17:53:09.000000 rethink-note-0.2.3/src/rethink_note.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:53:09.000000 rethink-note-0.2.3/src/rethink_note.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-28 17:53:09.000000 rethink-note-0.2.3/src/rethink_note.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-28 17:53:09.000000 rethink-note-0.2.3/src/rethink_note.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:53:09.456378 rethink-note-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24771 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_core_files_obsidian.py
--rw-r--r--   0 runner    (1001) docker     (127)    17748 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_core_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_core_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_data_restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_search_es.py
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_search_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_sso.py
--rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-03-28 17:53:05.000000 rethink-note-0.2.3/tests/test_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.053400 rethink-note-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-03 16:31:07.000000 rethink-note-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-03 16:31:12.053400 rethink-note-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-03 16:31:07.000000 rethink-note-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 16:31:07.000000 rethink-note-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 16:31:12.053400 rethink-note-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.941400 rethink-note-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.945400 rethink-note-0.2.4/src/rethink/
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/.env.local
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10206 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.945400 rethink-note-0.2.4/src/rethink/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.945400 rethink-note-0.2.4/src/rethink/controllers/files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/files/upload_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.945400 rethink-note-0.2.4/src/rethink/controllers/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/node/node_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/node/trash_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/controllers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/schemas/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/controllers/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/search/node_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/controllers/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/user/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6731 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/user/user_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/controllers/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/controllers/verify/v_captcha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/core/files/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/get.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/core/files/importing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.949401 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.953400 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/text/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/text/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.953400 rethink-note-0.2.4/src/rethink/core/files/importing/sync_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/sync_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/importing/sync_tasks/editor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/files/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.953400 rethink-note-0.2.4/src/rethink/core/node/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/node/backup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13141 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/node/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9389 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.953400 rethink-note-0.2.4/src/rethink/core/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/verify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/verify/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/core/verify/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.953400 rethink-note-0.2.4/src/rethink/depend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.957400 rethink-note-0.2.4/src/rethink/depend/mongita/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44121 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/command_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.957400 rethink-note-0.2.4/src/rethink/depend/mongita/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/engines/disk_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/engines/engine_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/engines/memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/mongita_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/mongitasync.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/read_concern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/mongita/write_concern.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.957400 rethink-note-0.2.4/src/rethink/depend/sso/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11277 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/facebook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/microsoft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/depend/sso/qq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.957400 rethink-note-0.2.4/src/rethink/dist-local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.957400 rethink-note-0.2.4/src/rethink/dist-local/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   171986 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/css/app.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.937400 rethink-note-0.2.4/src/rethink/dist-local/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.937400 rethink-note-0.2.4/src/rethink/dist-local/dist/css/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.961400 rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/ant-design.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/wechat.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.961400 rethink-note-0.2.4/src/rethink/dist-local/dist/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.961400 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/b3log.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/chainbook.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/doge.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/hacpai.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13662 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/huaji.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/latke.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/liandi.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/lute.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/octocat.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/pipe.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/siyuan.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/solo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/sym.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/trollface.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/vditor.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/wide.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8469 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/wulian.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/img-loading.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.937400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.961400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/abcjs/
+-rw-r--r--   0 runner    (1001) docker     (127)   363243 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/abcjs/abcjs_basic.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.965400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/echarts/
+-rw-r--r--   0 runner    (1001) docker     (127)   762119 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/echarts/echarts.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.965400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/flowchart.js/
+-rw-r--r--   0 runner    (1001) docker     (127)   125802 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/flowchart.js/flowchart.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.973400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/graphviz/
+-rw-r--r--   0 runner    (1001) docker     (127)  4423759 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/graphviz/full.render.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11468 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/graphviz/viz.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.973400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/
+-rw-r--r--   0 runner    (1001) docker     (127)   376423 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/highlight.pack.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/solidity.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.981400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/abap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol_nu.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/ant-design.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/arduino.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/autumn.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/borland.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/bw.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8006 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/colorful.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/dracula.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/emacs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/friendly.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/fruity.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/github.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/igor.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/lovelace.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7248 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/manni.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokai.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokailight.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7646 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/murphy.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7139 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/native.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7988 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pastie.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6754 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/perldoc.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7041 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rainbow_dash.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rrt.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark256.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7780 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/swapoff.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8775 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/tango.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/trac.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6007 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vim.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     6672 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/xcode.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/yul.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.981400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/en_US.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/fr_FR.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ja_JP.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ko_KR.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/pt_BR.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ru_RU.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/sv_SE.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_CN.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2512 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_TW.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.981400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    42983 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/icons/ant.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20896 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/icons/material.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.985400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.997400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    63632 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    33516 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    28076 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    12368 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    12344 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     7656 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19584 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19572 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    13208 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    51336 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    29912 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25324 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    32968 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16780 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    33580 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    19676 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16988 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    53580 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    26272 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31196 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18668 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16400 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31308 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18748 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    16440 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    24504 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14408 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    22364 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12028 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12316 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16648 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5468 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    27556 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16028 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13568 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    23196 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   277038 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33730 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/mhchem.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.997400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/lute/
+-rw-r--r--   0 runner    (1001) docker     (127)  3785836 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/lute/lute.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.005400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/
+-rw-r--r--   0 runner    (1001) docker     (127)    23112 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/katex.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   824275 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/markmap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/prism.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.005400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.009400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/assistive-mml.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/complexity.js
+-rw-r--r--   0 runner    (1001) docker     (127)    32640 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/explorer.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/semantic-enrich.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.009400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/
+-rw-r--r--   0 runner    (1001) docker     (127)   106067 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/asciimath.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.009400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml/
+-rw-r--r--   0 runner    (1001) docker     (127)    33265 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml/entities.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.937400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.017400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/action.js
+-rw-r--r--   0 runner    (1001) docker     (127)   147205 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/all-packages.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23357 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/ams.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7056 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/amscd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7019 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/autoload.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bbox.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/boldsymbol.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7150 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/braket.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17174 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bussproofs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/cancel.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/color.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/colorV2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4764 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/configMacros.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/enclose.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/extpfeil.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3572 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/html.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36819 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/mhchem.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10840 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/newcommand.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noerrors.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noundefined.js
+-rw-r--r--   0 runner    (1001) docker     (127)    23443 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/physics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6521 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/require.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/tagFormat.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/textmacros.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/unicode.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/verb.js
+-rw-r--r--   0 runner    (1001) docker     (127)   129130 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-base.js
+-rw-r--r--   0 runner    (1001) docker     (127)   270488 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-full.js
+-rw-r--r--   0 runner    (1001) docker     (127)   163954 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.017400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.021400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/
+-rw-r--r--   0 runner    (1001) docker     (127)   326869 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/de.js
+-rw-r--r--   0 runner    (1001) docker     (127)   423424 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/en.js
+-rw-r--r--   0 runner    (1001) docker     (127)   326446 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/es.js
+-rw-r--r--   0 runner    (1001) docker     (127)   321576 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1795679 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/mathmaps_ie.js
+-rw-r--r--   0 runner    (1001) docker     (127)   301796 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/nemeth.js
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/sre-node.js
+-rw-r--r--   0 runner    (1001) docker     (127)   874345 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/sre_browser.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1811419 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/tex-svg-full.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.025400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mermaid/
+-rw-r--r--   0 runner    (1001) docker     (127)  1084448 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/mermaid/mermaid.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.025400 rethink-note-0.2.4/src/rethink/dist-local/dist/js/plantuml/
+-rw-r--r--   0 runner    (1001) docker     (127)    29433 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/dist/js/plantuml/plantuml-encoder.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38078 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.033400 rethink-note-0.2.4/src/rethink/dist-local/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5369 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/2023_Obsidian_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/checked-success.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/chevron-double-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/circle-user.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/diagonal-arrow-right-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/dropdown-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/expand-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/expand-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/expand.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/eye-closed.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/eye-open.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/github-mark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/home.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/import.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/list.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16729 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/loading-dots.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    19402 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/menu.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    85421 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/morvanQR.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/node.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/plugin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/recentoutline.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/restore.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/return-arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/search.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/sort.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/text.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/three-dots-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/tick.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/trash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/upload.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/view-grid.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/img/white-cross.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.037400 rethink-note-0.2.4/src/rethink/dist-local/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1848178 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1266654 2024-04-03 16:31:07.000000 rethink-note-0.2.4/src/rethink/dist-local/js/chunk-vendors.js
+-rw-r--r--   0 runner    (1001) docker     (127)   121728 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/dist-local/js/highlight.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.037400 rethink-note-0.2.4/src/rethink/dist-local/media/
+-rw-r--r--   0 runner    (1001) docker     (127)  3429085 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/dist-local/media/demo.mp4
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.041400 rethink-note-0.2.4/src/rethink/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13660 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/coll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/db_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/indexing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/models/search_engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/baidu_stopwords.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/cn_stopwords.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22344 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/engine_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10979 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/search_engine/engine_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/models/tps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.941400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/_static/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/side.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:11.941400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/_static/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/_static/image/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/templates/side.html
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/register.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.045400 rethink-note-0.2.4/src/rethink/plugins/schedule/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/schedule/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/plugins/schedule/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.049400 rethink-note-0.2.4/src/rethink/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/trash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/routes/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8323 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.049400 rethink-note-0.2.4/src/rethink/version_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/version_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/version_manager/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-03 16:31:08.000000 rethink-note-0.2.4/src/rethink/version_manager/recover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.053400 rethink-note-0.2.4/src/rethink_note.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-03 16:31:11.000000 rethink-note-0.2.4/src/rethink_note.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19403 2024-04-03 16:31:11.000000 rethink-note-0.2.4/src/rethink_note.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:31:11.000000 rethink-note-0.2.4/src/rethink_note.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 16:31:11.000000 rethink-note-0.2.4/src/rethink_note.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 16:31:11.000000 rethink-note-0.2.4/src/rethink_note.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:31:12.053400 rethink-note-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24771 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_core_files_obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18610 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_core_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16152 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_core_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_data_restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8679 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_search_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_search_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9083 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-03 16:31:08.000000 rethink-note-0.2.4/tests/test_version_manager.py
```

### Comparing `rethink-note-0.2.3/LICENSE` & `rethink-note-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/PKG-INFO` & `rethink-note-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rethink-note
-Version: 0.2.3
+Version: 0.2.4
 Summary: note taking app
 Home-page: https://github.com/MorvanZhou/rethink
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/rethink/issues
 Project-URL: Source, https://github.com/MorvanZhou/rethink
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rethink-note Version: 0.2.3 Summary: note taking
+Metadata-Version: 2.1 Name: rethink-note Version: 0.2.4 Summary: note taking
 app Home-page: https://github.com/MorvanZhou/rethink Author: MorvanZhou Author-
 email: morvanzhou@hotmail.com Project-URL: Bug Tracker, https://github.com/
 MorvanZhou/rethink/issues Project-URL: Source, https://github.com/MorvanZhou/
 rethink Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `rethink-note-0.2.3/README.md` & `rethink-note-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/setup.cfg` & `rethink-note-0.2.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = rethink-note
-version = 0.2.3
+version = 0.2.4
 author = MorvanZhou
 author_email = morvanzhou@hotmail.com
 description = note taking app
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/MorvanZhou/rethink
 project_urls =
```

### Comparing `rethink-note-0.2.3/src/rethink/.env.local` & `rethink-note-0.2.4/src/rethink/.env.local`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 ONE_USER=true
+DEBUG=false
 VERIFY_REFERER=false
 PLUGINS=true
 DB_NAME=rethink
 JWT_KEY_PUB="ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQC7EqXzFLuLAFWTrcRi8UTA8sEpsoP+peDR+1KgBiOzwfn9PoJhAE6XsrsDC7tRr0nNKWPD95dAM6ySEHNEUPmkxvKRYGvkgp8s4Axv+9Lar63v7ZPJRbumI/JRzOOJvqBAYFUBX9OIGWGDJow8Dq0tLaj9t39lq2AStmIA3zIBreaFAH/cH1Ig5Z5zdD/M1T4AGl0kHoYKBh+jew7syyZcM22cKLCilT9oWTWpmJx17mf/Q17+7t4F8NS3ccQ6NpqpWYT03D6tgC/HgzIT6iMuJxdtil+e5/PcCeqaigBqehxwCDy5si9W7aOXALGZqmM5M68Lp2mn6386MKXh0WPf0Q2D1HSQNU2fdbdJ4EfHFwq/kWiFLd2u3AdxSnZaNYBH1pd4X2TXEtdmtAFwuJ/i5GQBs3Fy/Ukbdfrkc8ywzpsxTlCUnyiWXmWbh1YHME+7E5C4HlinvaD3x+znKmdoRnzo3gAlE9Q5fxq0D72RipDOqo0RH/PV9p904ZN9t+gj3TTNAbLf0ISbsVjw8ZLYg43pPAeHVwQVKLlR7YCHdsD8LoDqZSzWXx047JFlRFkvmBKUuPLDNMwGLhZzmwWoQIcxwDhcn+5NeeV8S3TS7QpXfEc/Z+hSwR10zoFrpNxEoygqhed8AlqrmFkzWy7d54HrhvHFOWmW6rA76VFPTQ=="
 JWT_KEY="-----BEGIN PRIVATE KEY-----
 MIIJQwIBADANBgkqhkiG9w0BAQEFAASCCS0wggkpAgEAAoICAQC7EqXzFLuLAFWT
 rcRi8UTA8sEpsoP+peDR+1KgBiOzwfn9PoJhAE6XsrsDC7tRr0nNKWPD95dAM6yS
```

### Comparing `rethink-note-0.2.3/src/rethink/application.py` & `rethink-note-0.2.4/src/rethink/application.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import webbrowser
 
 from fastapi import FastAPI, HTTPException
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi.responses import HTMLResponse, FileResponse
 from fastapi.staticfiles import StaticFiles
 from starlette.middleware.base import BaseHTTPMiddleware
 
@@ -90,46 +91,55 @@
             backup_count=10,
         )
     logger.debug(f'startup_event LOCAL_STORAGE_PATH: {os.environ.get("LOCAL_STORAGE_PATH")}')
     logger.debug(f'startup_event VUE_APP_MODE: {os.environ.get("VUE_APP_MODE")}')
     logger.debug(f'startup_event VUE_APP_API_PORT: {os.environ.get("VUE_APP_API_PORT")}')
     logger.debug(f'startup_event VUE_APP_LANGUAGE: {os.environ.get("VUE_APP_LANGUAGE")}')
     await client.init()
-    logger.info("db initialized")
+    logger.debug("db initialized")
 
     register_official_plugins()
 
+    host = os.getenv('RETHINK_HOSTNAME')
+    port = os.getenv('VUE_APP_API_PORT')
+    if os.getenv("RETHINK_HEADLESS", "0") == "0" and host and port:
+        webbrowser.open_new_tab(
+            f"http://{host}:{port}"
+        )
+
+    if config.is_local_db():
+        print(f"Rethink running on http://{host}:{port} (Press CTRL+C to quit)")
+
 
 @app.on_event("shutdown")
 async def shutdown_event():
     try:
         await client.search.es.close()
     except (AttributeError, ValueError):
         pass
-    logger.info("db closed")
+    logger.debug("db closed")
 
 
 try:
     for name in ["css", "js", "img", "dist"]:
         app.mount(
             f"/{name}",
             StaticFiles(directory=const.FRONTEND_DIR / name),
             name=name,
         )
 except RuntimeError:
-    logger.info("mount frontend failed")
+    logger.debug("mount frontend failed")
 
 
 @app.get("/", response_class=HTMLResponse)
 @app.get("/login", response_class=HTMLResponse)
 @app.get("/about", response_class=HTMLResponse)
 @app.get("/r", response_class=HTMLResponse)
 @app.get("/r/{path}", response_class=HTMLResponse)
 @app.get("/r/plugin/{pid}", response_class=HTMLResponse)
-@app.get("/r/plugins", response_class=HTMLResponse)
 @app.get("/n/{nid}", response_class=HTMLResponse)
 async def index() -> HTMLResponse:
     content = (const.FRONTEND_DIR / "index.html").read_text(encoding="utf-8")
     content += f"<script>window.VUE_APP_API_PORT = {os.getenv('VUE_APP_API_PORT')}</script>"
     return HTMLResponse(
         content=content,
         status_code=200,
```

### Comparing `rethink-note-0.2.3/src/rethink/config.py` & `rethink-note-0.2.4/src/rethink/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pydantic_settings import BaseSettings, SettingsConfigDict
 
 from rethink.logger import logger
 
 
 class Settings(BaseSettings):
     ONE_USER: bool = Field(default=1, env='ONE_USER')
+    DEBUG: bool = Field(default=False, env='DEBUG')
     VERIFY_REFERER: bool = Field(default=False, env='VERIFY_REFERER')
     PLUGINS: bool = Field(default=False, env='PLUGINS')
     LOCAL_STORAGE_PATH: Optional[DirectoryPath] = Field(env='LOCAL_STORAGE_PATH', default=None)
     DB_NAME: str = Field(env='DB_NAME', default="")
     DB_USER: str = Field(env='DB_USER', default="")
     DB_PASSWORD: str = Field(env='DB_PASSWORD', default="")
     DB_HOST: str = Field(env='DB_HOST', default="")
@@ -41,23 +42,27 @@
     OAUTH_CLIENT_SEC_QQ: str = Field(env='OAUTH_CLIENT_SEC_QQ', default="")
     OAUTH_CLIENT_ID_FACEBOOK: str = Field(env='OAUTH_CLIENT_ID_QQ', default="")
     OAUTH_CLIENT_SEC_FACEBOOK: str = Field(env='OAUTH_CLIENT_SEC_QQ', default="")
     COS_SECRET_ID: str = Field(env='COS_SECRET_ID', default="")
     COS_SECRET_KEY: str = Field(env="COS_SECRET_KEY", default="")
     COS_REGION: str = Field(env="COS_REGION", default="")
     COS_BUCKET_NAME: str = Field(env="COS_BUCKET_NAME", default="")
+    MD_BACKUP_INTERVAL: int = Field(env="MD_BACKUP_INTERVAL", default=60 * 5)  # 5 minutes
 
     model_config = SettingsConfigDict(
         env_file=".env",
         env_file_encoding='utf-8',
         case_sensitive=True,
     )
 
     def __init__(self):
         super().__init__()
+        if self.DEBUG:
+            logger.setLevel("DEBUG")
+
         logger.debug(f'config - LOCAL_STORAGE_PATH: {self.LOCAL_STORAGE_PATH}')
         if self.LOCAL_STORAGE_PATH is None and self.DB_HOST == "":
             raise ValueError("LOCAL_STORAGE_PATH and DB_HOST cannot be empty at the same time")
         if self.DB_SALT == "":
             self.DB_SALT = bcrypt.gensalt(4).decode("utf-8")
         if self.JWT_KEY == b"" or self.JWT_KEY_PUB == b"":
             key = rsa.generate_private_key(
```

### Comparing `rethink-note-0.2.3/src/rethink/const.py` & `rethink-note-0.2.4/src/rethink/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 RECOMMEND_CONTENT_MAX_LENGTH = 200
 EMAIL_MAX_LENGTH = 100
 PASSWORD_MAX_LENGTH = 20
 NICKNAME_MAX_LENGTH = 20
 IMG_RESIZE_THRESHOLD = 1024 * 1024 * 3  # 3MB
 MAX_UPLOAD_FILE_SIZE = 1024 * 1024 * 50  # 50MB
 PLUGIN_ID_MAX_LENGTH = 40
+MAX_MD_BACKUP_VERSIONS = 10
 
 
 class NodeType(Enum):
     FILE = 0
     MARKDOWN = auto()
 
 
@@ -55,14 +56,15 @@
     USER_SPACE_NOT_ENOUGH = 25
     INVALID_NODE_DISPLAY_SORT_KEY = 26
     INVALID_EMAIL = 27
     REQUEST_INPUT_ERROR = 28
     INVALID_SETTING = 29
     OLD_PASSWORD_ERROR = 30
     PLUGIN_NOT_FOUND = 31
+    COS_ERROR = 32
 
 
 INT_CODE_MAP = {
     c.value: c for c in Code
 }
 
 
@@ -103,14 +105,15 @@
     Code.USER_SPACE_NOT_ENOUGH: CodeMessage(zh="用户空间不足", en="User space not enough"),
     Code.INVALID_NODE_DISPLAY_SORT_KEY: CodeMessage(zh="无效的排序方式", en="Invalid sort key"),
     Code.INVALID_EMAIL: CodeMessage(zh="邮箱格式错误", en="Email format error"),
     Code.REQUEST_INPUT_ERROR: CodeMessage(zh="请求输入错误", en="Request input error"),
     Code.INVALID_SETTING: CodeMessage(zh="无效的设置", en="Invalid setting"),
     Code.OLD_PASSWORD_ERROR: CodeMessage(zh="旧密码错误", en="Old password error"),
     Code.PLUGIN_NOT_FOUND: CodeMessage(zh="插件未找到", en="Plugin not found"),
+    Code.COS_ERROR: CodeMessage(zh="COS 错误", en="COS error"),
 }
 
 DEFAULT_USER = {
     "nickname": "rethink",
     "email": "rethink@rethink.run",
     "avatar": "",
 }
```

### Comparing `rethink-note-0.2.3/src/rethink/controllers/auth.py` & `rethink-note-0.2.4/src/rethink/controllers/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     match = bcrypt.checkpw(base_pw, u["hashed"].encode("utf-8"))
     return match
 
 
 def _base_password(password: str, email: str) -> bytes:
     # update hash strategy
     s = f"{password}&&{config.get_settings().DB_SALT}$${email}"
-    logger.info(f"hashing: {s}")
+    logger.debug(f"hashing: {s}")
     return base64.b64encode(
         hashlib.sha256(s.encode("utf-8")).digest()
     )
 
 
 def hash_password(password: str, email: str) -> str:
     bpw = _base_password(password=password, email=email)
```

### Comparing `rethink-note-0.2.3/src/rethink/controllers/email.py` & `rethink-note-0.2.4/src/rethink/controllers/email.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/files/upload_files.py` & `rethink-note-0.2.4/src/rethink/controllers/files/upload_files.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/node/node_ops.py` & `rethink-note-0.2.4/src/rethink/controllers/node/node_ops.py`

 * *Files 17% similar despite different names*

```diff
@@ -185,7 +185,54 @@
                     score=0,
                     type=n["type"],
                     createdAt=datetime2str(n["_id"].generation_time),
                     modifiedAt=datetime2str(n["modifiedAt"]),
                 ) for n in nodes],
         ),
     )
+
+
+async def get_hist_editions(
+        td: TokenDecode,
+        req: schemas.node.HistEditionsRequest,
+) -> schemas.node.HistEditionsResponse:
+    if td.code != const.Code.OK:
+        return schemas.node.HistEditionsResponse(
+            code=td.code.value,
+            message=const.get_msg_by_code(td.code, td.language),
+            requestId=req.requestId,
+            versions=[],
+        )
+    versions, code = await core.node.get_hist_editions(
+        uid=td.uid,
+        nid=req.nid,
+    )
+    return schemas.node.HistEditionsResponse(
+        code=code.value,
+        message=const.get_msg_by_code(code, td.language),
+        requestId=req.requestId,
+        versions=versions,
+    )
+
+
+async def get_hist_edition_md(
+        td: TokenDecode,
+        req: schemas.node.HistEditionMdRequest,
+) -> schemas.node.HistEditionMdResponse:
+    if td.code != const.Code.OK:
+        return schemas.node.HistEditionMdResponse(
+            code=td.code.value,
+            message=const.get_msg_by_code(td.code, td.language),
+            requestId=req.requestId,
+            md="",
+        )
+    md, code = await core.node.get_hist_edition_md(
+        uid=td.uid,
+        nid=req.nid,
+        version=req.version,
+    )
+    return schemas.node.HistEditionMdResponse(
+        code=code.value,
+        message=const.get_msg_by_code(code, td.language),
+        requestId=req.requestId,
+        md=md,
+    )
```

### Comparing `rethink-note-0.2.3/src/rethink/controllers/node/trash_ops.py` & `rethink-note-0.2.4/src/rethink/controllers/node/trash_ops.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/oauth.py` & `rethink-note-0.2.4/src/rethink/controllers/oauth.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/plugin.py` & `rethink-note-0.2.4/src/rethink/controllers/plugin.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/schemas/files.py` & `rethink-note-0.2.4/src/rethink/controllers/schemas/files.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/schemas/node.py` & `rethink-note-0.2.4/src/rethink/controllers/schemas/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,7 +81,32 @@
 
 
 class CoreNodesResponse(BaseModel):
     code: NonNegativeInt
     message: str
     data: NodesSearchResponse.Data
     requestId: str = Field(default="", max_length=const.REQUEST_ID_MAX_LENGTH)
+
+
+class HistEditionsRequest(BaseModel):
+    nid: str = Field(max_length=const.NID_MAX_LENGTH)
+    requestId: str = Field(default="", max_length=const.REQUEST_ID_MAX_LENGTH)
+
+
+class HistEditionsResponse(BaseModel):
+    code: NonNegativeInt
+    message: str
+    requestId: str
+    versions: List[str] = Field(default_factory=list)
+
+
+class HistEditionMdRequest(BaseModel):
+    nid: str = Field(max_length=const.NID_MAX_LENGTH)
+    version: str = Field(max_length=30)
+    requestId: str = Field(default="", max_length=const.REQUEST_ID_MAX_LENGTH)
+
+
+class HistEditionMdResponse(BaseModel):
+    code: NonNegativeInt
+    message: str
+    requestId: str
+    md: str
```

### Comparing `rethink-note-0.2.3/src/rethink/controllers/schemas/plugin.py` & `rethink-note-0.2.4/src/rethink/controllers/schemas/plugin.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/schemas/search.py` & `rethink-note-0.2.4/src/rethink/controllers/schemas/search.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/schemas/user.py` & `rethink-note-0.2.4/src/rethink/controllers/schemas/user.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/search/node_search.py` & `rethink-note-0.2.4/src/rethink/controllers/search/node_search.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/user/password.py` & `rethink-note-0.2.4/src/rethink/controllers/user/password.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/user/user_ops.py` & `rethink-note-0.2.4/src/rethink/controllers/user/user_ops.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/controllers/utils.py` & `rethink-note-0.2.4/src/rethink/controllers/utils.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/get.py` & `rethink-note-0.2.4/src/rethink/core/files/get.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/__init__.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/ops.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,14 @@
             nid = short_uuid()
             exist_path2nid[path] = nid
         md = f"{md[: span[0]]}[@{filename}](/n/{nid}){md[span[1]:]}"
     return md
 
 
 def _decode_filename(filepath: str) -> str:
-    # 尝试使用不同的编码格式解码文件名
     encodings = ['utf-8', 'gbk', 'cp437']
     for encoding in encodings:
         try:
             return filepath.encode('cp437').decode(encoding)
         except (UnicodeDecodeError, UnicodeEncodeError):
             continue
     return filepath
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/obsidian/task.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/obsidian/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,54 +27,54 @@
         unzipped_files = ops.unzip_obsidian(bytes_data)
     except zipfile.BadZipFile as e:
         await utils.set_running_false(
             uid,
             const.Code.INVALID_FILE_TYPE,
             msg=f"unzip failed: {e}"
         )
-        logger.info(f"invalid file type: {filename}, uid: {uid}")
+        logger.error(f"invalid file type: {filename}, uid: {uid}")
         return
     t1 = time.time()
-    logger.info(f"obsidian upload, uid={uid}, unzip time: {t1 - t0:.2f}")
+    logger.debug(f"obsidian upload, uid={uid}, unzip time: {t1 - t0:.2f}")
 
     existed_path2nid = doc.get("obsidian", {}).copy()
     md_count = len(unzipped_files.md_full)
     if md_count == 0:
         await utils.set_running_false(
             uid,
             const.Code.INVALID_FILE_TYPE,
             msg="no md file found",
         )
-        logger.info(f"no md file found, uid: {uid}")
+        logger.debug(f"no md file found, uid: {uid}")
         return
     elif md_count > 2000:
         await utils.set_running_false(
             uid,
             const.Code.TOO_MANY_FILES,
             msg=f"md file count: {md_count} > 2000",
         )
-        logger.info(f"too many md files: {md_count}, uid: {uid}")
+        logger.debug(f"too many md files: {md_count}, uid: {uid}")
         return
 
     # check file size
     for full in [unzipped_files.md_full, unzipped_files.others_full]:
         for full_path, meta in full.items():
             meta: ops.UnzipObsidian.Meta
 
             if meta.size > max_file_size:
                 await utils.set_running_false(
                     uid,
                     const.Code.TOO_LARGE_FILE,
                     msg=f"file size > {max_file_size}: {full_path}",
                 )
-                logger.info(f"too large file: {full_path}, uid: {uid}")
+                logger.debug(f"too large file: {full_path}, uid: {uid}")
                 return
 
     t2 = time.time()
-    logger.info(f"obsidian upload, uid={uid}, filter time: {t2 - t1:.2f}")
+    logger.debug(f"obsidian upload, uid={uid}, filter time: {t2 - t1:.2f}")
 
     # add new md files with only title
     for i, (full_path, meta) in enumerate(unzipped_files.md_full.items()):
         meta: ops.UnzipObsidian.Meta
 
         if full_path in existed_path2nid:
             continue
@@ -105,35 +105,35 @@
             doc, code = await utils.update_process(uid=uid, type_=type_, process=int(i / md_count * 10))
             if code != const.Code.OK:
                 await utils.set_running_false(
                     uid,
                     code,
                     msg="process updating failed",
                 )
-                logger.info(f"error: {code}, filepath: {full_path}, uid: {uid}")
+                logger.error(f"error: {code}, filepath: {full_path}, uid: {uid}")
                 return
             if not doc["running"]:
                 break
     t3 = time.time()
-    logger.info(f"obsidian upload, uid={uid}, add new md time: {t3 - t2:.2f}")
+    logger.debug(f"obsidian upload, uid={uid}, add new md time: {t3 - t2:.2f}")
 
     # update all md content and update md files
     for i, (full_path, meta) in enumerate(unzipped_files.md_full.items()):
         meta: ops.UnzipObsidian.Meta
 
         try:
             md = meta.file.decode("utf-8")
         except (FileNotFoundError, OSError, UnicodeDecodeError) as e:
             logger.error(f"error: {e}. filepath: {full_path}")
             await utils.set_running_false(
                 uid,
                 const.Code.FILE_OPEN_ERROR,
                 msg=f"file decode utf-8 failed, {e}: {full_path}",
             )
-            logger.info(f"error: {const.Code.FILE_OPEN_ERROR}, filepath: {full_path}, uid: {uid}")
+            logger.error(f"error: {const.Code.FILE_OPEN_ERROR}, filepath: {full_path}, uid: {uid}")
             return
 
         md = await ops.replace_inner_link_and_upload(
             uid=uid,
             md=md,
             exist_path2nid=existed_path2nid,
             others_full=unzipped_files.others_full,
@@ -155,39 +155,39 @@
             )
             if code != const.Code.OK:
                 await utils.set_running_false(
                     uid,
                     code,
                     msg=f"file insert failed: {full_path}",
                 )
-                logger.info(f"error: {code}, filepath: {full_path}, uid: {uid}")
+                logger.error(f"error: {code}, filepath: {full_path}, uid: {uid}")
                 return
             existed_path2nid[full_path] = n["id"]
         elif code != const.Code.OK:
             await utils.set_running_false(
                 uid,
                 code,
                 msg=f"file updating failed: {full_path}",
             )
-            logger.info(f"error: {code}, filepath: {full_path}, uid: {uid}")
+            logger.error(f"error: {code}, filepath: {full_path}, uid: {uid}")
             return
         if i % 20 == 0:
             doc, code = await utils.update_process(uid=uid, type_=type_, process=int(i / md_count * 80 + 10))
             if code != const.Code.OK:
                 await utils.set_running_false(
                     uid,
                     code,
                     msg="uploading process update failed",
                 )
-                logger.info(f"error: {code}, filepath: {full_path}, uid: {uid}")
+                logger.error(f"error: {code}, filepath: {full_path}, uid: {uid}")
                 return
             if not doc["running"]:
                 break
     t4 = time.time()
-    logger.info(f"obsidian upload, uid={uid}, update all files time: {t4 - t3:.2f}")
+    logger.debug(f"obsidian upload, uid={uid}, update all files time: {t4 - t3:.2f}")
 
     # update for old obsidian files
     count = 0
     for base_name, nid in doc["obsidian"].items():
         if base_name not in existed_path2nid:
             n, code = await core.node.get(uid=uid, nid=nid)
             if code != const.Code.OK:
@@ -205,18 +205,18 @@
                 uid=uid, type_=type_, process=int(count / len(doc["obsidian"]) * 10 + 90))
             if code != const.Code.OK:
                 await utils.set_running_false(
                     uid,
                     code,
                     msg="uploading process update failed",
                 )
-                logger.info(f"error: {code}, uid: {uid}")
+                logger.error(f"error: {code}, uid: {uid}")
                 return
             if not doc["running"]:
                 break
 
         count += 1
 
     t5 = time.time()
-    logger.info(f"obsidian upload, uid={uid}, update for old obsidian files time: {t5 - t4:.2f}")
+    logger.debug(f"obsidian upload, uid={uid}, update for old obsidian files time: {t5 - t4:.2f}")
 
     await utils.finish_task(uid=uid, obsidian=existed_path2nid)
```

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/text/task.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/text/task.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/async_tasks/utils.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/async_tasks/utils.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/importing/sync_tasks/editor.py` & `rethink-note-0.2.4/src/rethink/core/files/importing/sync_tasks/editor.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/saver.py` & `rethink-note-0.2.4/src/rethink/core/files/saver.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/files/upload.py` & `rethink-note-0.2.4/src/rethink/core/files/upload.py`

 * *Files 9% similar despite different names*

```diff
@@ -138,18 +138,18 @@
         uid=uid,
         files=files,
     )
 
 
 async def fetch_image_vditor(uid: str, url: str, count=0) -> Tuple[str, const.Code]:
     if count > 2:
-        logger.info(f"too many 30X code, failed to get {url}")
+        logger.debug(f"too many 30X code, failed to get {url}")
         return "", const.Code.FILE_OPEN_ERROR
     if ssrf_check(url):
-        logger.info(f"ssrf check failed: {url}")
+        logger.debug(f"ssrf check failed: {url}")
         return "", const.Code.FILE_OPEN_ERROR
     u, code = await core.user.get(uid=uid)
     if code != const.Code.OK:
         return "", code
     if await core.user.user_space_not_enough(u=u):
         return "", const.Code.USER_SPACE_NOT_ENOUGH
     async with httpx.AsyncClient() as client:
@@ -163,15 +163,15 @@
         except (
                 httpx.ConnectTimeout,
                 RuntimeError,
                 httpx.ConnectError,
                 httpx.ReadTimeout,
                 httpx.HTTPError
         ) as e:
-            logger.info(f"failed to get {url}: {e}")
+            logger.debug(f"failed to get {url}: {e}")
             return "", const.Code.FILE_OPEN_ERROR
         if response.status_code in [301, 302]:
             return await fetch_image_vditor(uid=uid, url=response.headers["Location"], count=count + 1)
         elif response.status_code != 200:
             return "", const.Code.FILE_OPEN_ERROR
 
         content = response.content
```

### Comparing `rethink-note-0.2.3/src/rethink/core/node.py` & `rethink-note-0.2.4/src/rethink/core/node/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,76 +1,22 @@
 import copy
 import datetime
-from pathlib import Path
-from typing import List, Optional, Set, Tuple, Dict, Any
+from typing import List, Optional, Tuple, Dict, Any
 
 from bson import ObjectId
 from bson.tz_util import utc
 
 from rethink import config, const, utils, regex
 from rethink import plugins
+from rethink.core import user
 from rethink.logger import logger
 from rethink.models import tps, db_ops
 from rethink.models.client import client
 from rethink.models.search_engine.engine import SearchDoc
-from . import user
-
-
-def __get_linked_nodes(new_md) -> Tuple[set, const.Code]:
-    # last first
-    cache_current_to_nid: Set[str] = set()
-
-    for match in list(regex.MD_AT_LINK.finditer(new_md))[::-1]:
-        l0, l1 = match.span(1)
-        link = new_md[l0:l1]
-        if link.startswith("/n/"):
-            # check existed nodes
-            to_nid = link[3:]
-            cache_current_to_nid.add(to_nid)
-    return cache_current_to_nid, const.Code.OK
-
-
-async def __flush_to_node_ids(
-        nid: str,
-        orig_to_nid: List[str],
-        new_md: str
-) -> Tuple[List[str], const.Code]:
-    new_to_nid, code = __get_linked_nodes(new_md=new_md)
-    if code != const.Code.OK:
-        return [], code
-
-    # remove fromNodes for linked nodes
-    orig_to_nid = set(orig_to_nid)
-    for to_nid in orig_to_nid.difference(new_to_nid):
-        await db_ops.remove_from_node(from_nid=nid, to_nid=to_nid)
-
-    # add fromNodes for linked nodes
-    for to_nid in new_to_nid.difference(orig_to_nid):
-        await db_ops.node_add_to_set(id_=to_nid, key="fromNodeIds", value=nid)
-
-    return list(new_to_nid), const.Code.OK
-
-
-def __local_usage_write_file(nid: str, md: str):
-    if not config.is_local_db():
-        return
-    md_dir = Path(config.get_settings().LOCAL_STORAGE_PATH) / ".data" / "md"
-    md_dir.mkdir(parents=True, exist_ok=True)
-    with open(md_dir / f"{nid}.md", "w", encoding="utf-8") as f:
-        f.write(md)
-
-
-def __local_usage_delete_files(nids: List[str]):
-    if not config.is_local_db():
-        return
-    dir_ = Path(config.get_settings().LOCAL_STORAGE_PATH) / ".data" / "md"
-    for nid in nids:
-        md_dir = dir_ / f"{nid}.md"
-        if md_dir.exists():
-            md_dir.unlink()
+from . import backup, node_utils
 
 
 @plugins.handler.on_node_added
 async def add(  # noqa: C901
         uid: str,
         md: str,
         type_: int = const.NodeType.MARKDOWN.value,
@@ -97,15 +43,15 @@
         from_nids.append(from_nid)
         res = await db_ops.node_add_to_set(from_nid, "toNodeIds", nid)
         if res.modified_count != 1:
             return None, const.Code.OPERATION_FAILED
 
     new_to_node_ids = []
     if md != "":
-        new_to_node_ids, code = await __flush_to_node_ids(nid=nid, orig_to_nid=[], new_md=md)
+        new_to_node_ids, code = await node_utils.flush_to_node_ids(nid=nid, orig_to_nid=[], new_md=md)
         if code != const.Code.OK:
             return None, code
     _id = ObjectId()
     data: tps.Node = {
         "_id": _id,
         "id": nid,
         "uid": uid,
@@ -115,45 +61,33 @@
         "type": type_,
         "disabled": False,
         "inTrash": False,
         "modifiedAt": _id.generation_time,
         "inTrashAt": None,
         "fromNodeIds": from_nids,
         "toNodeIds": new_to_node_ids,
+        "history": [],
     }
     res = await client.coll.nodes.insert_one(data)
     if not res.acknowledged:
         return None, const.Code.OPERATION_FAILED
 
     await user.update_used_space(uid=uid, delta=new_size)
 
-    __local_usage_write_file(nid=nid, md=md)
+    code = await backup.storage_md(node=data, keep_hist=False)
+    if code != const.Code.OK:
+        return data, code
 
     if type_ == const.NodeType.MARKDOWN.value:
         code = await client.search.add(uid=uid, doc=SearchDoc(nid=nid, title=title, body=body))
         if code != const.Code.OK:
             logger.error(f"add search index failed, code: {code}")
     return data, const.Code.OK
 
 
-async def __set_linked_nodes(
-        docs: List[tps.Node],
-        with_disabled: bool = False,
-):
-    for doc in docs:
-        doc["fromNodes"] = await client.coll.nodes.find({
-            "id": {"$in": doc["fromNodeIds"]},
-            "disabled": with_disabled,
-        }).to_list(length=None)
-        doc["toNodes"] = await client.coll.nodes.find({
-            "id": {"$in": doc["toNodeIds"]},
-            "disabled": with_disabled,
-        }).to_list(length=None)
-
-
 async def get(
         uid: str,
         nid: str,
         with_disabled: bool = False,
         in_trash: bool = False,
 ) -> Tuple[Optional[tps.Node], const.Code]:
     docs, code = await get_batch(
@@ -183,15 +117,15 @@
     if not with_disabled:
         c["disabled"] = False
     docs = await client.coll.nodes.find(c).to_list(length=None)
     if len(docs) != len(nids):
         logger.error(f"docs len != nids len: {nids}")
         return [], const.Code.NODE_NOT_EXIST
 
-    await __set_linked_nodes(
+    await node_utils.set_linked_nodes(
         docs=docs,
         with_disabled=with_disabled,
     )
     return docs, const.Code.OK
 
 
 @plugins.handler.on_node_updated
@@ -230,23 +164,23 @@
     if n["title"] != title:
         # update it's title in fromNodes md's link
         from_nodes = await client.coll.nodes.find({"id": {"$in": n["fromNodeIds"]}}).to_list(length=None)
         for from_node in from_nodes:
             new_md = utils.change_link_title(md=from_node["md"], nid=nid, new_title=title)
             n, old_n, code = await update(uid=uid, nid=from_node["id"], md=new_md)
             if code != const.Code.OK:
-                logger.info(f"update fromNode {from_node['id']} failed")
+                logger.error(f"update fromNode {from_node['id']} failed")
         new_data["title"] = title
 
     if n["md"] != md:
         new_data["md"] = md
         if n["snippet"] != snippet:
             new_data["snippet"] = snippet
 
-    new_data["toNodeIds"], code = await __flush_to_node_ids(
+    new_data["toNodeIds"], code = await node_utils.flush_to_node_ids(
         nid=n["id"], orig_to_nid=n["toNodeIds"], new_md=md)
     if code != const.Code.OK:
         return None, old_n, code
 
     if not config.is_local_db():
         doc = await client.coll.nodes.find_one_and_update(
             {"id": nid},
@@ -262,26 +196,29 @@
         if res.modified_count != 1:
             logger.error(f"update node {nid} failed")
             return None, old_n, const.Code.OPERATION_FAILED
         doc = await client.coll.nodes.find_one({"id": nid})
 
     if doc is None:
         return None, old_n, const.Code.NODE_NOT_EXIST
-    await __set_linked_nodes(
+    await node_utils.set_linked_nodes(
         docs=[doc],
         with_disabled=False,
     )
 
     await user.update_used_space(uid=uid, delta=len(md.encode("utf-8")) - old_md_size)
 
-    __local_usage_write_file(nid=nid, md=md)
     if doc["type"] == const.NodeType.MARKDOWN.value:
         code = await client.search.update(uid=uid, doc=SearchDoc(nid=nid, title=title, body=body))
         if code != const.Code.OK:
             logger.error(f"update search index failed, code: {code}")
+
+    code = await backup.storage_md(node=doc, keep_hist=True)
+    if code != const.Code.OK:
+        return doc, old_n, code
     return doc, old_n, code
 
 
 async def to_trash(uid: str, nid: str) -> const.Code:
     return await batch_to_trash(uid=uid, nids=[nid])
 
 
@@ -382,19 +319,20 @@
 
     # remove node
     res = await client.coll.nodes.delete_many({"id": {"$in": nids}, "uid": uid})
     if res.deleted_count != len(nids):
         logger.error(f"delete nodes {nids} failed")
         return const.Code.OPERATION_FAILED
 
-    __local_usage_delete_files(nids=nids)
+    backup.delete_node_md(uid=uid, nids=nids)
 
     code = await client.search.delete_batch(uid=uid, nids=nids)
     if code != const.Code.OK:
         logger.error(f"delete search index failed, code: {code}")
+
     return code
 
 
 async def disable(
         uid: str,
         nid: str,
 ) -> const.Code:
@@ -441,7 +379,23 @@
         return code
     _, code = await add(
         uid=uid,
         md=lns[1].format(n["id"]),
     )
     await client.search.refresh()
     return code
+
+
+async def get_hist_editions(uid: str, nid: str) -> Tuple[List[str], const.Code]:
+    n, code = await get(uid=uid, nid=nid)
+    if code != const.Code.OK:
+        return [], code
+    return n.get("history", []), const.Code.OK
+
+
+async def get_hist_edition_md(uid: str, nid: str, version: str) -> Tuple[str, const.Code]:
+    n, code = await get(uid=uid, nid=nid)
+    if code != const.Code.OK:
+        return "", code
+    if version not in n["history"]:
+        return "", const.Code.NODE_NOT_EXIST
+    return backup.get_md(uid=uid, nid=nid, version=version)
```

### Comparing `rethink-note-0.2.3/src/rethink/core/search.py` & `rethink-note-0.2.4/src/rethink/core/search.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/user.py` & `rethink-note-0.2.4/src/rethink/core/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,16 @@
         },
         "settings": {
             "language": language,
             "theme": const.AppTheme.LIGHT.value,
             "editorMode": const.EditorMode.WYSIWYG.value,
             "editorFontSize": 15,
             "editorCodeTheme": const.EditorCodeTheme.GITHUB.value,
+            "editorSepRightWidth": 200,
+            "editorSideCurrentToolId": "",
         }
     }
     # catch if id is duplicated
     while True:
         try:
             res = await client.coll.users.insert_one(data)
             if not res.acknowledged:
```

### Comparing `rethink-note-0.2.3/src/rethink/core/verify/email.py` & `rethink-note-0.2.4/src/rethink/core/verify/email.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/core/verify/verification.py` & `rethink-note-0.2.4/src/rethink/core/verify/verification.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/__init__.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/__init__.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/collection.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/collection.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/command_cursor.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/command_cursor.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/common.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/common.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/cursor.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/cursor.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/database.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/database.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/engines/disk_engine.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/engines/disk_engine.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/engines/engine_common.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/engines/engine_common.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/engines/memory_engine.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/engines/memory_engine.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/errors.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/errors.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/mongita_client.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/mongita_client.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/mongitasync.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/mongitasync.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/results.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/results.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/mongita/write_concern.py` & `rethink-note-0.2.4/src/rethink/depend/mongita/write_concern.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/base.py` & `rethink-note-0.2.4/src/rethink/depend/sso/base.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/facebook.py` & `rethink-note-0.2.4/src/rethink/depend/sso/facebook.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/generic.py` & `rethink-note-0.2.4/src/rethink/depend/sso/generic.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/github.py` & `rethink-note-0.2.4/src/rethink/depend/sso/github.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/gitlab.py` & `rethink-note-0.2.4/src/rethink/depend/sso/gitlab.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/google.py` & `rethink-note-0.2.4/src/rethink/depend/sso/google.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/microsoft.py` & `rethink-note-0.2.4/src/rethink/depend/sso/microsoft.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/depend/sso/qq.py` & `rethink-note-0.2.4/src/rethink/depend/sso/qq.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/css/app.css` & `rethink-note-0.2.4/src/rethink/dist-local/css/app.css`

 * *Files 0% similar despite different names*

```diff
@@ -3663,30 +3663,85 @@
   padding: 0 0 8px 0;
   line-height: 1.5em;
   color: #919090;
   white-space: break-spaces;
   overflow-wrap: break-word;
   overflow: hidden;
 }
+
 .snippet-expanded[data-v-404f2c61] {
   max-height: 400px;
   overflow-y: auto;
   white-space: break-spaces;
   overflow-wrap: break-word;
 }
 
+/*!**********************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
+  !*** css ./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css ***!
+  \**********************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
+
+.history-editions[data-v-7e97cf55] {
+  width: 100%;
+  height: 100%;
+  overflow-y: auto;
+  color: rgba(0, 0, 0, 0.88);
+}
+
+.no-versions[data-v-7e97cf55] {
+  padding-top: 2rem;
+  text-align: center;
+}
+
+.heading[data-v-7e97cf55] {
+  padding: 1rem;
+  font-weight: bold;
+  border-bottom: 1px solid var(--border-color);
+}
+
+.version[data-v-7e97cf55] {
+  padding: 1rem 1rem 0 1rem;
+  border-bottom: 1px solid var(--border-color);
+}
+
+.version-info[data-v-7e97cf55] {
+  display: flex;
+  justify-content: space-between;
+  align-items: center;
+}
+
+.time[data-v-7e97cf55] {
+  font-size: 0.7rem;
+  color: rgba(0, 0, 0, 0.6);
+}
+
+.right-buttons[data-v-7e97cf55] {
+  display: flex;
+  align-items: center;
+  padding: 0 0.5rem;
+  cursor: pointer;
+}
+
+.right-buttons img[data-v-7e97cf55] {
+  width: 20px;
+}
+
+.restore-notice[data-v-7e97cf55] {
+  font-size: 0.7rem;
+}
+
+
 /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** css ./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/SideBarItemView.vue?vue&type=style&index=0&id=41948506&scoped=true&lang=css ***!
   \**************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
 
 .item-view[data-v-41948506] {
   width: 200px;
   overflow-x: hidden;
+  border-top: 1px solid #e0e0e0;
 }
-
 .plugin[data-v-41948506] {
   width: 100%;
   height: 100%;
   border-style: outset;
   border-width: 1px;
 }
 
@@ -3758,14 +3813,20 @@
   align-items: center;
   text-align: center;
   display: flex;
   font-size: 0.9em;
   padding: 0 30px;
   height: 30px;
 }
+
+.sm[data-v-0c69ff34] {
+  justify-content: center;
+  width: 20px;
+}
+
 .create-node[data-v-0c69ff34]:hover {
   background: #f64324;
 }
 .create-node-img[data-v-0c69ff34] {
   height: 60%;
   background: transparent;
 }
```

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/ant-design.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/ant-design.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/dark.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/dark.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/light.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/light.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/css/content-theme/wechat.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/css/content-theme/wechat.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/b3log.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/b3log.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/chainbook.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/chainbook.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/doge.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/doge.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/hacpai.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/hacpai.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/huaji.gif` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/huaji.gif`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/latke.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/latke.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/liandi.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/liandi.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/lute.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/lute.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/octocat.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/octocat.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/pipe.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/pipe.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/siyuan.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/siyuan.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/solo.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/solo.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/sym.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/sym.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/trollface.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/trollface.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/vditor.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/vditor.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/wide.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/wide.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/emoji/wulian.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/emoji/wulian.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/img-loading.svg` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/img-loading.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/images/logo.png` & `rethink-note-0.2.4/src/rethink/dist-local/dist/images/logo.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/abcjs/abcjs_basic.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/abcjs/abcjs_basic.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/echarts/echarts.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/echarts/echarts.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/flowchart.js/flowchart.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/flowchart.js/flowchart.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/graphviz/full.render.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/graphviz/full.render.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/graphviz/viz.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/graphviz/viz.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/highlight.pack.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/solidity.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/solidity.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/abap.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/abap.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/algol.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/algol_nu.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/algol_nu.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/ant-design.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/ant-design.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/arduino.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/arduino.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/autumn.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/autumn.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/borland.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/borland.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/bw.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/bw.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/colorful.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/colorful.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/dracula.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/dracula.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/emacs.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/emacs.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/friendly.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/friendly.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/fruity.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/fruity.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/github.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/github.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/igor.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/igor.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/lovelace.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/lovelace.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/manni.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/manni.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/monokai.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokai.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/monokailight.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/monokailight.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/murphy.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/murphy.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/native.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/native.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-dark.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-dark.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-light.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/paraiso-light.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/pastie.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pastie.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/perldoc.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/perldoc.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/pygments.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/pygments.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/rainbow_dash.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rainbow_dash.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/rrt.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/rrt.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark256.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-dark256.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-light.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/solarized-light.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/swapoff.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/swapoff.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/tango.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/tango.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/trac.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/trac.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/vim.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vim.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/vs.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/vs.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/styles/xcode.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/styles/xcode.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/highlight.js/yul.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/highlight.js/yul.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/en_US.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/en_US.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/fr_FR.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/fr_FR.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ja_JP.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ja_JP.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ko_KR.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ko_KR.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/pt_BR.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/pt_BR.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/ru_RU.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/ru_RU.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/sv_SE.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/sv_SE.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/zh_CN.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_CN.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/i18n/zh_TW.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/i18n/zh_TW.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/icons/ant.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/icons/ant.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/icons/material.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/icons/material.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.ttf` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.ttf`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff2` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/katex.min.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/katex.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/katex.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/katex/mhchem.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/katex/mhchem.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/lute/lute.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/lute/lute.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/katex.min.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/katex.min.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/markmap.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/markmap.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/markmap/prism.css` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/markmap/prism.css`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/LICENSE` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/LICENSE`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/assistive-mml.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/assistive-mml.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/complexity.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/complexity.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/explorer.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/explorer.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/a11y/semantic-enrich.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/a11y/semantic-enrich.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/asciimath.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/asciimath.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/mml/entities.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml/entities.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/mml.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/mml.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/action.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/action.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/all-packages.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/all-packages.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/ams.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/ams.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/amscd.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/amscd.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/autoload.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/autoload.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bbox.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bbox.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/boldsymbol.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/boldsymbol.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/braket.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/braket.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bussproofs.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/bussproofs.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/cancel.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/cancel.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/color.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/color.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/colorV2.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/colorV2.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/configMacros.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/configMacros.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/enclose.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/enclose.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/extpfeil.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/extpfeil.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/html.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/html.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/mhchem.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/mhchem.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/newcommand.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/newcommand.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noerrors.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noerrors.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noundefined.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/noundefined.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/physics.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/physics.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/require.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/require.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/tagFormat.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/tagFormat.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/textmacros.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/textmacros.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/unicode.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/unicode.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/verb.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex/extensions/verb.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex-base.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-base.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex-full.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex-full.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/input/tex.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/input/tex.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/de.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/de.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/en.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/en.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/es.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/es.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/fr.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/fr.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/mathmaps_ie.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/mathmaps_ie.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/nemeth.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/mathmaps/nemeth.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/sre/sre_browser.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/sre/sre_browser.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mathjax/tex-svg-full.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mathjax/tex-svg-full.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/mermaid/mermaid.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/mermaid/mermaid.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/dist/js/plantuml/plantuml-encoder.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/dist/js/plantuml/plantuml-encoder.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/favicon.ico` & `rethink-note-0.2.4/src/rethink/dist-local/favicon.ico`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/2023_Obsidian_logo.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/2023_Obsidian_logo.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/checked-success.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/checked-success.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/circle-user.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/circle-user.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/cross.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/cross.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/diagonal-arrow-right-up.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/diagonal-arrow-right-up.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/dropdown-arrow.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/dropdown-arrow.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/eye-closed.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/eye-closed.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/eye-open.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/eye-open.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/github-mark.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/github-mark.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/home.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/home.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/import.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/import.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/loading-dots.gif` & `rethink-note-0.2.4/src/rethink/dist-local/img/loading-dots.gif`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/loading.gif` & `rethink-note-0.2.4/src/rethink/dist-local/img/loading.gif`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/morvanQR.png` & `rethink-note-0.2.4/src/rethink/dist-local/img/morvanQR.png`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/node.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/node.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/plugin.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/plugin.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/recentoutline.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/recentoutline.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/return-arrow.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/return-arrow.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/search.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/search.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/sort.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/sort.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/three-dots-vertical.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/three-dots-vertical.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/trash.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/trash.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/upload.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/upload.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/view-grid.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/view-grid.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/img/white-cross.svg` & `rethink-note-0.2.4/src/rethink/dist-local/img/white-cross.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/index.html` & `rethink-note-0.2.4/src/rethink/dist-local/index.html`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/js/app.js` & `rethink-note-0.2.4/src/rethink/dist-local/js/app.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -270,14 +270,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_editor_renderMd__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/editor/renderMd */ \"./src/utils/app/editor/renderMd.ts\");\n/* harmony import */ var _assets_images_icons_cross_svg__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/assets/images/icons/cross.svg */ \"./src/assets/images/icons/cross.svg\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _router__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/router */ \"./src/router/index.ts\");\n/* harmony import */ var _assets_images_icons_diagonal_arrow_right_up_svg__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/assets/images/icons/diagonal-arrow-right-up.svg */ \"./src/assets/images/icons/diagonal-arrow-right-up.svg\");\n\n\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'RecommendPopupWindow',\n  props: {\n    rid: {\n      type: String,\n      required: true\n    }\n  },\n  emits: [\"changeShowDetailNid\"],\n  setup(__props, {\n    expose: __expose,\n    emit: __emit\n  }) {\n    __expose();\n    const props = __props;\n    const emit = __emit;\n    const html = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(\"\");\n    (0,vue__WEBPACK_IMPORTED_MODULE_0__.onMounted)(async () => {\n      // popup a window in the center of the screen\n      // blur the background\n      html.value = await (0,_utils_app_editor_renderMd__WEBPACK_IMPORTED_MODULE_1__.renderNid)(props.rid);\n    });\n    const mq = (0,_utils_mq__WEBPACK_IMPORTED_MODULE_3__.useMQ)();\n    const __returned__ = {\n      props,\n      emit,\n      html,\n      mq,\n      get CrossIcon() {\n        return _assets_images_icons_cross_svg__WEBPACK_IMPORTED_MODULE_2__;\n      },\n      get router() {\n        return _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"];\n      },\n      get DiagonalArrowRightUp() {\n        return _assets_images_icons_diagonal_arrow_right_up_svg__WEBPACK_IMPORTED_MODULE_5__;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
+        "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true":
+            /*!*************************************************************************************************************************************************************************************************************************************************************!*\
+  !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true ***!
+  \*************************************************************************************************************************************************************************************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_editor_sidebar_historyEditions__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/editor/sidebar/historyEditions */ \"./src/utils/app/editor/sidebar/historyEditions.ts\");\n/* harmony import */ var _assets_images_icons_restore_svg__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/assets/images/icons/restore.svg */ \"./src/assets/images/icons/restore.svg\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'HistRestore',\n  props: {\n    nid: {\n      type: String,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const {\n      versions,\n      onClickRestore\n    } = (0,_utils_app_editor_sidebar_historyEditions__WEBPACK_IMPORTED_MODULE_1__.useHistEditions)(props.nid);\n    const __returned__ = {\n      props,\n      versions,\n      onClickRestore,\n      get RestoreIcon() {\n        return _assets_images_icons_restore_svg__WEBPACK_IMPORTED_MODULE_2__;\n      },\n      get mLang() {\n        return _utils_multiLang__WEBPACK_IMPORTED_MODULE_3__[\"default\"];\n      },\n      get utc2localFull() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__.utc2localFull;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+
+                /***/
+            }),
+
+        /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=script&lang=ts&setup=true":
             /*!*************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=script&lang=ts&setup=true ***!
   \*************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -303,15 +316,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/SideBarItemView.vue?vue&type=script&lang=ts&setup=true":
             /*!*****************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/SideBarItemView.vue?vue&type=script&lang=ts&setup=true ***!
   \*****************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _components_app_editor_sidebar_LinkedNodes_vue__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/components/app/editor/sidebar/LinkedNodes.vue */ \"./src/components/app/editor/sidebar/LinkedNodes.vue\");\n/* harmony import */ var _utils_app_editor_sidebar__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/editor/sidebar */ \"./src/utils/app/editor/sidebar/index.ts\");\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'SideBarItemView',\n  props: {\n    toNodes: {\n      type: Array,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const {\n      sideActivatedItem,\n      sideIframe\n    } = (0,_utils_app_editor_sidebar__WEBPACK_IMPORTED_MODULE_2__.useSidebarItemView)();\n    const __returned__ = {\n      props,\n      sideActivatedItem,\n      sideIframe,\n      LinkedNodes: _components_app_editor_sidebar_LinkedNodes_vue__WEBPACK_IMPORTED_MODULE_1__[\"default\"]\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/SideBarItemView.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _components_app_editor_sidebar_LinkedNodes_vue__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/components/app/editor/sidebar/LinkedNodes.vue */ \"./src/components/app/editor/sidebar/LinkedNodes.vue\");\n/* harmony import */ var _components_app_editor_sidebar_HistRestore_vue__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/components/app/editor/sidebar/HistRestore.vue */ \"./src/components/app/editor/sidebar/HistRestore.vue\");\n/* harmony import */ var _utils_app_editor_sidebar__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/app/editor/sidebar */ \"./src/utils/app/editor/sidebar/index.ts\");\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'SideBarItemView',\n  props: {\n    toNodes: {\n      type: Array,\n      required: true\n    },\n    nid: {\n      type: String,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const {\n      sideActivatedItem,\n      sideIframe\n    } = (0,_utils_app_editor_sidebar__WEBPACK_IMPORTED_MODULE_3__.useSidebarItemView)();\n    const __returned__ = {\n      props,\n      sideActivatedItem,\n      sideIframe,\n      LinkedNodes: _components_app_editor_sidebar_LinkedNodes_vue__WEBPACK_IMPORTED_MODULE_1__[\"default\"],\n      HistoryRestore: _components_app_editor_sidebar_HistRestore_vue__WEBPACK_IMPORTED_MODULE_2__[\"default\"]\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/SideBarItemView.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/left/AppLeftNav.vue?vue&type=script&lang=ts&setup=true":
             /*!******************************************************************************************************************************************************************************************************************************************************!*\
@@ -485,15 +498,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SMSearchResults.vue?vue&type=script&lang=ts&setup=true":
             /*!*****************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SMSearchResults.vue?vue&type=script&lang=ts&setup=true ***!
   \*****************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _components_app_tools_ResultTitleHeader_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/tools/ResultTitleHeader.vue */ \"./src/components/app/tools/ResultTitleHeader.vue\");\n/* harmony import */ var _components_WaitLoading_vue__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/components/WaitLoading.vue */ \"./src/components/WaitLoading.vue\");\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'SMSearchResults',\n  props: {\n    searchResult: {\n      type: Object,\n      required: true\n    },\n    isSearching: {\n      type: Boolean,\n      required: true\n    }\n  },\n  emits: [\"selectResult\", \"searchMore\"],\n  setup(__props, {\n    expose: __expose,\n    emit: __emit\n  }) {\n    __expose();\n    const props = __props;\n    const emit = __emit;\n    const __returned__ = {\n      props,\n      emit,\n      get utc2local() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_1__.utc2local;\n      },\n      get mLang() {\n        return _utils_multiLang__WEBPACK_IMPORTED_MODULE_2__[\"default\"];\n      },\n      ResultTitleHeader: _components_app_tools_ResultTitleHeader_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      WaitLoading: _components_WaitLoading_vue__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/search/SMSearchResults.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _components_app_tools_ResultTitleHeader_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/tools/ResultTitleHeader.vue */ \"./src/components/app/tools/ResultTitleHeader.vue\");\n/* harmony import */ var _components_WaitLoading_vue__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/components/WaitLoading.vue */ \"./src/components/WaitLoading.vue\");\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'SMSearchResults',\n  props: {\n    searchResult: {\n      type: Object,\n      required: true\n    },\n    isSearching: {\n      type: Boolean,\n      required: true\n    }\n  },\n  emits: [\"selectResult\", \"searchMore\"],\n  setup(__props, {\n    expose: __expose,\n    emit: __emit\n  }) {\n    __expose();\n    const props = __props;\n    const emit = __emit;\n    const __returned__ = {\n      props,\n      emit,\n      get utc2localApproximate() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_1__.utc2localApproximate;\n      },\n      get mLang() {\n        return _utils_multiLang__WEBPACK_IMPORTED_MODULE_2__[\"default\"];\n      },\n      ResultTitleHeader: _components_app_tools_ResultTitleHeader_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      WaitLoading: _components_WaitLoading_vue__WEBPACK_IMPORTED_MODULE_4__[\"default\"]\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/search/SMSearchResults.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SearchTool.vue?vue&type=script&lang=ts&setup=true":
             /*!************************************************************************************************************************************************************************************************************************************************************!*\
@@ -550,15 +563,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/CardNode.vue?vue&type=script&lang=ts&setup=true":
             /*!****************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/CardNode.vue?vue&type=script&lang=ts&setup=true ***!
   \****************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_const__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/const */ \"./src/utils/const.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/nodesDisplay/display/NodeOperations.vue */ \"./src/components/app/nodesDisplay/display/NodeOperations.vue\");\n/* harmony import */ var _components_app_tools_ShowNotice_vue__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/components/app/tools/ShowNotice.vue */ \"./src/components/app/tools/ShowNotice.vue\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n/* harmony import */ var _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/batchFilesOps */ \"./src/utils/app/batchFilesOps.ts\");\n\n\n\n\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'CardNode',\n  props: {\n    n: {\n      type: Object,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const user = (0,_utils_app_user__WEBPACK_IMPORTED_MODULE_6__.useUser)();\n    const sortKey = (0,vue__WEBPACK_IMPORTED_MODULE_0__.computed)(() => user.value?.lastState.nodeDisplaySortKey);\n    const mq = (0,_utils_mq__WEBPACK_IMPORTED_MODULE_5__.useMQ)();\n    const __returned__ = {\n      props,\n      user,\n      sortKey,\n      mq,\n      get CONST() {\n        return _utils_const__WEBPACK_IMPORTED_MODULE_1__[\"default\"];\n      },\n      get clipText() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.clipText;\n      },\n      get stripMdTitle() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.stripMdTitle;\n      },\n      get utc2local() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.utc2local;\n      },\n      NodeOperations: _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      DelayNoticeShow: _components_app_tools_ShowNotice_vue__WEBPACK_IMPORTED_MODULE_4__[\"default\"],\n      get select() {\n        return _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_7__.select;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/CardNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_const__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/const */ \"./src/utils/const.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/nodesDisplay/display/NodeOperations.vue */ \"./src/components/app/nodesDisplay/display/NodeOperations.vue\");\n/* harmony import */ var _components_app_tools_ShowNotice_vue__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/components/app/tools/ShowNotice.vue */ \"./src/components/app/tools/ShowNotice.vue\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n/* harmony import */ var _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/batchFilesOps */ \"./src/utils/app/batchFilesOps.ts\");\n\n\n\n\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'CardNode',\n  props: {\n    n: {\n      type: Object,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const user = (0,_utils_app_user__WEBPACK_IMPORTED_MODULE_6__.useUser)();\n    const sortKey = (0,vue__WEBPACK_IMPORTED_MODULE_0__.computed)(() => user.value?.lastState.nodeDisplaySortKey);\n    const mq = (0,_utils_mq__WEBPACK_IMPORTED_MODULE_5__.useMQ)();\n    const __returned__ = {\n      props,\n      user,\n      sortKey,\n      mq,\n      get CONST() {\n        return _utils_const__WEBPACK_IMPORTED_MODULE_1__[\"default\"];\n      },\n      get clipText() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.clipText;\n      },\n      get stripMdTitle() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.stripMdTitle;\n      },\n      get utc2localApproximate() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.utc2localApproximate;\n      },\n      NodeOperations: _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      DelayNoticeShow: _components_app_tools_ShowNotice_vue__WEBPACK_IMPORTED_MODULE_4__[\"default\"],\n      get select() {\n        return _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_7__.select;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/CardNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListDisplay.vue?vue&type=script&lang=ts&setup=true":
             /*!*******************************************************************************************************************************************************************************************************************************************************************!*\
@@ -576,15 +589,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListNode.vue?vue&type=script&lang=ts&setup=true":
             /*!****************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListNode.vue?vue&type=script&lang=ts&setup=true ***!
   \****************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_const__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/const */ \"./src/utils/const.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/nodesDisplay/display/NodeOperations.vue */ \"./src/components/app/nodesDisplay/display/NodeOperations.vue\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/batchFilesOps */ \"./src/utils/app/batchFilesOps.ts\");\n/* harmony import */ var _utils_app_nodesDisplay__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/nodesDisplay */ \"./src/utils/app/nodesDisplay.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'ListNode',\n  props: {\n    node: {\n      type: Object,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const user = (0,_utils_app_user__WEBPACK_IMPORTED_MODULE_7__.useUser)();\n    const sortKey = (0,vue__WEBPACK_IMPORTED_MODULE_0__.computed)(() => user.value?.lastState.nodeDisplaySortKey);\n    const mq = (0,_utils_mq__WEBPACK_IMPORTED_MODULE_4__.useMQ)();\n    const __returned__ = {\n      props,\n      user,\n      sortKey,\n      mq,\n      get CONST() {\n        return _utils_const__WEBPACK_IMPORTED_MODULE_1__[\"default\"];\n      },\n      get clipText() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.clipText;\n      },\n      get stripMdTitle() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.stripMdTitle;\n      },\n      get utc2local() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.utc2local;\n      },\n      NodeOperations: _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      get select() {\n        return _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_5__.select;\n      },\n      get push2Page() {\n        return _utils_app_nodesDisplay__WEBPACK_IMPORTED_MODULE_6__.push2Page;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/ListNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_const__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/const */ \"./src/utils/const.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n/* harmony import */ var _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/components/app/nodesDisplay/display/NodeOperations.vue */ \"./src/components/app/nodesDisplay/display/NodeOperations.vue\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/batchFilesOps */ \"./src/utils/app/batchFilesOps.ts\");\n/* harmony import */ var _utils_app_nodesDisplay__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/nodesDisplay */ \"./src/utils/app/nodesDisplay.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\n\n\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (/*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.defineComponent)({\n  __name: 'ListNode',\n  props: {\n    node: {\n      type: Object,\n      required: true\n    }\n  },\n  setup(__props, {\n    expose: __expose\n  }) {\n    __expose();\n    const props = __props;\n    const user = (0,_utils_app_user__WEBPACK_IMPORTED_MODULE_7__.useUser)();\n    const sortKey = (0,vue__WEBPACK_IMPORTED_MODULE_0__.computed)(() => user.value?.lastState.nodeDisplaySortKey);\n    const mq = (0,_utils_mq__WEBPACK_IMPORTED_MODULE_4__.useMQ)();\n    const __returned__ = {\n      props,\n      user,\n      sortKey,\n      mq,\n      get CONST() {\n        return _utils_const__WEBPACK_IMPORTED_MODULE_1__[\"default\"];\n      },\n      get clipText() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.clipText;\n      },\n      get stripMdTitle() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.stripMdTitle;\n      },\n      get utc2localApproximate() {\n        return _utils_app_textOps__WEBPACK_IMPORTED_MODULE_2__.utc2localApproximate;\n      },\n      NodeOperations: _components_app_nodesDisplay_display_NodeOperations_vue__WEBPACK_IMPORTED_MODULE_3__[\"default\"],\n      get select() {\n        return _utils_app_batchFilesOps__WEBPACK_IMPORTED_MODULE_5__.select;\n      },\n      get push2Page() {\n        return _utils_app_nodesDisplay__WEBPACK_IMPORTED_MODULE_6__.push2Page;\n      }\n    };\n    Object.defineProperty(__returned__, '__isScriptSetup', {\n      enumerable: false,\n      value: true\n    });\n    return __returned__;\n  }\n}));\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/ListNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/NodeOperations.vue?vue&type=script&lang=ts&setup=true":
             /*!**********************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1278,15 +1291,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/AppNodeEditPanel.vue?vue&type=template&id=220b40cb&scoped=true&ts=true":
             /*!***********************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/AppNodeEditPanel.vue?vue&type=template&id=220b40cb&scoped=true&ts=true ***!
   \***********************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-220b40cb\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"container\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      \"work-place-sm\": $setup.mq.sm\n    }, \"work-place\"])\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"WaitLoading\"], {\n    circle: true,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([$setup.editorClass, \"md-editor\"]),\n    loading: !$setup.ready,\n    style: {\n      \"border\": \"none\",\n      \"width\": \"100%\"\n    }\n  }, null, 8 /* PROPS */, [\"class\", \"loading\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    id: $setup.editorDivId,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([$setup.editorClass, \"md-editor\"])\n  }, null, 2 /* CLASS */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.ready]]), $setup.ready && $setup.node && !$setup.mq.sm && $setup.sideActivatedItem ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SepLine\"], {\n    key: 0\n  })) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true), $setup.ready && $setup.node && !$setup.mq.sm && $setup.sideActivatedItem ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SideBarItemView\"], {\n    key: 1,\n    \"to-nodes\": $setup.node.toNodes\n  }, null, 8 /* PROPS */, [\"to-nodes\"])) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)]), $setup.node && !$setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SideBar\"], {\n    key: 0\n  })) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)], 2 /* CLASS */), $setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SearchWindowSM\"], {\n    key: 0,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"nid\"])) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SearchWindow\"], {\n    key: 1,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"nid\"]))], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/AppNodeEditPanel.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-220b40cb\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"container\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      \"work-place-sm\": $setup.mq.sm\n    }, \"work-place\"])\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"WaitLoading\"], {\n    circle: true,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([$setup.editorClass, \"md-editor\"]),\n    loading: !$setup.ready,\n    style: {\n      \"border\": \"none\",\n      \"width\": \"100%\"\n    }\n  }, null, 8 /* PROPS */, [\"class\", \"loading\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    id: $setup.editorDivId,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([$setup.editorClass, \"md-editor\"])\n  }, null, 2 /* CLASS */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.ready]]), $setup.ready && $setup.node && !$setup.mq.sm && $setup.sideActivatedItem ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SepLine\"], {\n    key: 0\n  })) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true), $setup.ready && $setup.node && !$setup.mq.sm && $setup.sideActivatedItem ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SideBarItemView\"], {\n    key: 1,\n    \"to-nodes\": $setup.node.toNodes,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"to-nodes\", \"nid\"])) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)]), $setup.node && !$setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SideBar\"], {\n    key: 0\n  })) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)], 2 /* CLASS */), $setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SearchWindowSM\"], {\n    key: 0,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"nid\"])) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"SearchWindow\"], {\n    key: 1,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"nid\"]))], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/AppNodeEditPanel.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/cursorSearch/SearchBar.vue?vue&type=template&id=a7f024e4&scoped=true&ts=true":
             /*!*****************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1401,14 +1414,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.array.push.js */ \"./node_modules/core-js/modules/es.array.push.js\");\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_1__.pushScopeId)(\"data-v-68a8b995\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_1__.popScopeId)(), n);\nconst _hoisted_1 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"div\", {\n  class: \"overlay\"\n}, null, -1 /* HOISTED */));\nconst _hoisted_2 = {\n  class: \"popup\"\n};\nconst _hoisted_3 = {\n  class: \"header\"\n};\nconst _hoisted_4 = [\"src\"];\nconst _hoisted_5 = [\"src\"];\nconst _hoisted_6 = [\"innerHTML\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_1__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_1__.Fragment, null, [_hoisted_1, (0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"div\", _hoisted_2, [(0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"div\", _hoisted_3, [(0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"img\", {\n    src: $setup.CrossIcon,\n    alt: \"close\",\n    class: \"close\",\n    onClick: _cache[0] || (_cache[0] = (0,vue__WEBPACK_IMPORTED_MODULE_1__.withModifiers)($event => $setup.emit('changeShowDetailNid', ''), [\"stop\"]))\n  }, null, 8 /* PROPS */, _hoisted_4), (0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"img\", {\n    src: $setup.DiagonalArrowRightUp,\n    alt: \"goto\",\n    class: \"goto\",\n    onClick: _cache[1] || (_cache[1] = (0,vue__WEBPACK_IMPORTED_MODULE_1__.withModifiers)(() => {\n      $setup.emit(\"changeShowDetailNid\", \"\");\n      $setup.router.push({\n        name: \"node\",\n        params: {\n          id: $props.rid\n        }\n      });\n    }, [\"stop\"]))\n  }, null, 8 /* PROPS */, _hoisted_5)]), (0,vue__WEBPACK_IMPORTED_MODULE_1__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_1__.normalizeClass)([{\n      'detail-md-content-sm': $setup.mq.sm\n    }, \"detail-md-content\"]),\n    innerHTML: $setup.html\n  }, null, 10 /* CLASS, PROPS */, _hoisted_6)])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
+        "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true":
+            /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
+  !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true ***!
+  \**************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-7e97cf55\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"history-editions\"\n};\nconst _hoisted_2 = {\n  key: 0,\n  class: \"no-versions\"\n};\nconst _hoisted_3 = {\n  key: 1\n};\nconst _hoisted_4 = {\n  class: \"heading\"\n};\nconst _hoisted_5 = {\n  class: \"version-info\"\n};\nconst _hoisted_6 = {\n  class: \"time\"\n};\nconst _hoisted_7 = [\"onClick\"];\nconst _hoisted_8 = [\"src\"];\nconst _hoisted_9 = {\n  class: \"restore-notice\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_1, [$setup.versions.length == 0 ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_2, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"nodeHistEditionRestoreNoVersions\")), 1 /* TEXT */)) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_3, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_4, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"nodeHistEditionRestoreHeading\")), 1 /* TEXT */), ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(true), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, (0,vue__WEBPACK_IMPORTED_MODULE_0__.renderList)($setup.versions, v => {\n    return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n      key: v,\n      class: \"version\"\n    }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_5, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_6, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localFull(v)), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n      class: \"right-buttons hover-node-bg\",\n      onClick: $event => $setup.onClickRestore(v)\n    }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"img\", {\n      src: $setup.RestoreIcon,\n      alt: \"restore\"\n    }, null, 8 /* PROPS */, _hoisted_8), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", _hoisted_9, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"nodeHistEditionRestoreNotice\")), 1 /* TEXT */)], 8 /* PROPS */, _hoisted_7)])]);\n  }), 128 /* KEYED_FRAGMENT */))]))]);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+
+                /***/
+            }),
+
+        /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=template&id=404f2c61&scoped=true&ts=true":
             /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=template&id=404f2c61&scoped=true&ts=true ***!
   \**************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -1434,15 +1460,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/SideBarItemView.vue?vue&type=template&id=41948506&scoped=true&ts=true":
             /*!******************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/SideBarItemView.vue?vue&type=template&id=41948506&scoped=true&ts=true ***!
   \******************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-41948506\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  key: 0,\n  class: \"item-view\"\n};\nconst _hoisted_2 = {\n  key: 1,\n  ref: \"sideIframe\",\n  class: \"plugin\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return $setup.sideActivatedItem !== null ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_1, [$setup.sideActivatedItem === 'linkedNodes' ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"LinkedNodes\"], {\n    key: 0,\n    \"to-nodes\": $setup.props.toNodes\n  }, null, 8 /* PROPS */, [\"to-nodes\"])) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"iframe\", _hoisted_2, null, 512 /* NEED_PATCH */))])) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/SideBarItemView.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-41948506\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  key: 0,\n  class: \"item-view\"\n};\nconst _hoisted_2 = {\n  key: 2,\n  ref: \"sideIframe\",\n  class: \"plugin\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return $setup.sideActivatedItem !== null ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_1, [$setup.sideActivatedItem === 'linkedNodes' ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"LinkedNodes\"], {\n    key: 0,\n    \"to-nodes\": $setup.props.toNodes\n  }, null, 8 /* PROPS */, [\"to-nodes\"])) : $setup.sideActivatedItem === 'histRestore' ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createBlock)($setup[\"HistoryRestore\"], {\n    key: 1,\n    nid: $setup.props.nid\n  }, null, 8 /* PROPS */, [\"nid\"])) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"iframe\", _hoisted_2, null, 512 /* NEED_PATCH */))])) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/SideBarItemView.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/left/AppLeftNav.vue?vue&type=template&id=86347dae&ts=true":
             /*!*******************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1551,15 +1577,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/CreateNodeButton.vue?vue&type=template&id=0c69ff34&scoped=true&ts=true":
             /*!************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/CreateNodeButton.vue?vue&type=template&id=0c69ff34&scoped=true&ts=true ***!
   \************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-0c69ff34\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = [\"src\"];\nconst _hoisted_2 = {\n  key: 0,\n  class: \"white-font\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n    class: \"create-node\",\n    onClick: _cache[0] || (_cache[0] =\n    //@ts-ignore\n    (...args) => $setup.goNewNodePage && $setup.goNewNodePage(...args))\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"img\", {\n    src: $setup.PlusIcon,\n    alt: \"create new\",\n    class: \"create-node-img\"\n  }, null, 8 /* PROPS */, _hoisted_1), !$setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"span\", _hoisted_2, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"headerBarNewThink\")), 1 /* TEXT */)) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)]);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/CreateNodeButton.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-0c69ff34\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = [\"src\"];\nconst _hoisted_2 = {\n  key: 0,\n  class: \"white-font\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      sm: $setup.mq.sm\n    }, \"create-node\"]),\n    onClick: _cache[0] || (_cache[0] =\n    //@ts-ignore\n    (...args) => $setup.goNewNodePage && $setup.goNewNodePage(...args))\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"img\", {\n    src: $setup.PlusIcon,\n    alt: \"create new\",\n    class: \"create-node-img\"\n  }, null, 8 /* PROPS */, _hoisted_1), !$setup.mq.sm ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"span\", _hoisted_2, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"headerBarNewThink\")), 1 /* TEXT */)) : (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\"v-if\", true)], 2 /* CLASS */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/CreateNodeButton.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/EditorHeader.vue?vue&type=template&id=55779ec4&scoped=true&ts=true":
             /*!********************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1616,15 +1642,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SMSearchResults.vue?vue&type=template&id=19c64c31&scoped=true&ts=true":
             /*!******************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SMSearchResults.vue?vue&type=template&id=19c64c31&scoped=true&ts=true ***!
   \******************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-19c64c31\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = [\"onClick\"];\nconst _hoisted_2 = {\n  class: \"node-time\"\n};\nconst _hoisted_3 = [\"innerHTML\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: \"no-search-result\"\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('noSearchResult')), 513 /* TEXT, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.props.searchResult.nodes.length === 0]]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: \"search-results\",\n    onScroll: _cache[0] || (_cache[0] = $event => $setup.emit('searchMore', $event))\n  }, [((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(true), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, (0,vue__WEBPACK_IMPORTED_MODULE_0__.renderList)($props.searchResult.nodes, result => {\n    return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n      key: result.id,\n      class: \"search-result hover-node-bg\",\n      onClick: $event => $setup.emit('selectResult', result.id)\n    }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"ResultTitleHeader\"], {\n      title: result.titleHighlight\n    }, null, 8 /* PROPS */, [\"title\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_2, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2local(result.modifiedAt)), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n      class: \"node-hl\",\n      innerHTML: result.bodyHighlights[0]\n    }, null, 8 /* PROPS */, _hoisted_3)], 8 /* PROPS */, _hoisted_1);\n  }), 128 /* KEYED_FRAGMENT */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"WaitLoading\"], {\n    circle: false,\n    loading: $props.isSearching,\n    style: {\n      \"border\": \"none\",\n      \"height\": \"4rem\"\n    }\n  }, null, 8 /* PROPS */, [\"loading\"])], 544 /* NEED_HYDRATION, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.props.searchResult.nodes.length > 0]])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/search/SMSearchResults.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-19c64c31\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = [\"onClick\"];\nconst _hoisted_2 = {\n  class: \"node-time\"\n};\nconst _hoisted_3 = [\"innerHTML\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: \"no-search-result\"\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('noSearchResult')), 513 /* TEXT, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.props.searchResult.nodes.length === 0]]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: \"search-results\",\n    onScroll: _cache[0] || (_cache[0] = $event => $setup.emit('searchMore', $event))\n  }, [((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(true), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, (0,vue__WEBPACK_IMPORTED_MODULE_0__.renderList)($props.searchResult.nodes, result => {\n    return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n      key: result.id,\n      class: \"search-result hover-node-bg\",\n      onClick: $event => $setup.emit('selectResult', result.id)\n    }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"ResultTitleHeader\"], {\n      title: result.titleHighlight\n    }, null, 8 /* PROPS */, [\"title\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_2, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localApproximate(result.modifiedAt)), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n      class: \"node-hl\",\n      innerHTML: result.bodyHighlights[0]\n    }, null, 8 /* PROPS */, _hoisted_3)], 8 /* PROPS */, _hoisted_1);\n  }), 128 /* KEYED_FRAGMENT */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"WaitLoading\"], {\n    circle: false,\n    loading: $props.isSearching,\n    style: {\n      \"border\": \"none\",\n      \"height\": \"4rem\"\n    }\n  }, null, 8 /* PROPS */, [\"loading\"])], 544 /* NEED_HYDRATION, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, $setup.props.searchResult.nodes.length > 0]])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nav/top/search/SMSearchResults.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nav/top/search/SearchTool.vue?vue&type=template&id=48038053&scoped=true&ts=true":
             /*!*************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1681,15 +1707,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/CardNode.vue?vue&type=template&id=e1905aa2&scoped=true&ts=true":
             /*!*****************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/CardNode.vue?vue&type=template&id=e1905aa2&scoped=true&ts=true ***!
   \*****************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-e1905aa2\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"top-right\"\n};\nconst _hoisted_2 = [\"id\", \"value\"];\nconst _hoisted_3 = {\n  key: 1,\n  class: \"time\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'block-header-sm': $setup.mq.sm\n    }, \"block-header\"])\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'title-sm': $setup.mq.sm\n    }, \"title\"])\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.stripMdTitle($setup.props.n.title, 20)), 3 /* TEXT, CLASS */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"NodeOperations\"], {\n    node: $props.n\n  }, null, 8 /* PROPS */, [\"node\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: $setup.props.n.id,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'cb-hide': $setup.mq.lg\n    }, \"checkbox node-checkbox\"]),\n    value: $setup.props.n.id,\n    type: \"checkbox\",\n    onClick: _cache[0] || (_cache[0] = (0,vue__WEBPACK_IMPORTED_MODULE_0__.withModifiers)($event => $setup.select($event, $setup.props.n.id), [\"stop\"]))\n  }, null, 10 /* CLASS, PROPS */, _hoisted_2)])], 2 /* CLASS */), $setup.sortKey === $setup.CONST.nodeSortType.ModifiedAt ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n    key: 0,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'time-sm': $setup.mq.sm\n    }, \"time\"])\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2local($setup.props.n.modifiedAt)), 3 /* TEXT, CLASS */)) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_3, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2local($setup.props.n.createdAt)), 1 /* TEXT */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"DelayNoticeShow\"], {\n    msg: $setup.props.n.snippet\n  }, {\n    default: (0,vue__WEBPACK_IMPORTED_MODULE_0__.withCtx)(() => [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n      class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"snippet\", {\n        'snippet-sm': $setup.mq.sm\n      }])\n    }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.clipText($setup.props.n.snippet, 60)), 3 /* TEXT, CLASS */)]),\n    _: 1 /* STABLE */\n  }, 8 /* PROPS */, [\"msg\"])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/CardNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-e1905aa2\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"top-right\"\n};\nconst _hoisted_2 = [\"id\", \"value\"];\nconst _hoisted_3 = {\n  key: 1,\n  class: \"time\"\n};\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'block-header-sm': $setup.mq.sm\n    }, \"block-header\"])\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'title-sm': $setup.mq.sm\n    }, \"title\"])\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.stripMdTitle($setup.props.n.title, 20)), 3 /* TEXT, CLASS */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"NodeOperations\"], {\n    node: $props.n\n  }, null, 8 /* PROPS */, [\"node\"]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: $setup.props.n.id,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'cb-hide': $setup.mq.lg\n    }, \"checkbox node-checkbox\"]),\n    value: $setup.props.n.id,\n    type: \"checkbox\",\n    onClick: _cache[0] || (_cache[0] = (0,vue__WEBPACK_IMPORTED_MODULE_0__.withModifiers)($event => $setup.select($event, $setup.props.n.id), [\"stop\"]))\n  }, null, 10 /* CLASS, PROPS */, _hoisted_2)])], 2 /* CLASS */), $setup.sortKey === $setup.CONST.nodeSortType.ModifiedAt ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", {\n    key: 0,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'time-sm': $setup.mq.sm\n    }, \"time\"])\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localApproximate($setup.props.n.modifiedAt)), 3 /* TEXT, CLASS */)) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_3, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localApproximate($setup.props.n.createdAt)), 1 /* TEXT */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"DelayNoticeShow\"], {\n    msg: $setup.props.n.snippet\n  }, {\n    default: (0,vue__WEBPACK_IMPORTED_MODULE_0__.withCtx)(() => [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", {\n      class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"snippet\", {\n        'snippet-sm': $setup.mq.sm\n      }])\n    }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.clipText($setup.props.n.snippet, 60)), 3 /* TEXT, CLASS */)]),\n    _: 1 /* STABLE */\n  }, 8 /* PROPS */, [\"msg\"])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/CardNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListDisplay.vue?vue&type=template&id=5a8668d7&ts=true":
             /*!********************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -1707,15 +1733,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListNode.vue?vue&type=template&id=97a6cb86&ts=true":
             /*!*****************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/ListNode.vue?vue&type=template&id=97a6cb86&ts=true ***!
   \*****************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _hoisted_1 = {\n  class: \"multi-select\"\n};\nconst _hoisted_2 = [\"id\", \"value\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: $setup.props.node.id,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'cb-hide': $setup.mq.lg\n    }, \"checkbox node-checkbox\"]),\n    value: $setup.props.node.id,\n    type: \"checkbox\",\n    onClick: _cache[0] || (_cache[0] = $event => $setup.select($event, $setup.props.node.id))\n  }, null, 10 /* CLASS, PROPS */, _hoisted_2)]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", {\n    class: \"title\",\n    onClick: _cache[1] || (_cache[1] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.stripMdTitle($setup.props.node.title, 20)), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", {\n    class: \"snippet\",\n    onClick: _cache[2] || (_cache[2] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.clipText($setup.props.node.snippet, 20)), 513 /* TEXT, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, !$setup.mq.sm]]), $setup.sortKey === $setup.CONST.nodeSortType.ModifiedAt ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"td\", {\n    key: 0,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"time\", {\n      'time-sm': $setup.mq.sm\n    }]),\n    onClick: _cache[3] || (_cache[3] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2local($setup.props.node.modifiedAt)), 3 /* TEXT, CLASS */)) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"td\", {\n    key: 1,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"time\", {\n      'time-sm': $setup.mq.sm\n    }]),\n    onClick: _cache[4] || (_cache[4] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2local($setup.props.node.createdAt)), 3 /* TEXT, CLASS */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"NodeOperations\"], {\n    node: $setup.props.node\n  }, null, 8 /* PROPS */, [\"node\"])])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/ListNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _hoisted_1 = {\n  class: \"multi-select\"\n};\nconst _hoisted_2 = [\"id\", \"value\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(vue__WEBPACK_IMPORTED_MODULE_0__.Fragment, null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: $setup.props.node.id,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([{\n      'cb-hide': $setup.mq.lg\n    }, \"checkbox node-checkbox\"]),\n    value: $setup.props.node.id,\n    type: \"checkbox\",\n    onClick: _cache[0] || (_cache[0] = $event => $setup.select($event, $setup.props.node.id))\n  }, null, 10 /* CLASS, PROPS */, _hoisted_2)]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", {\n    class: \"title\",\n    onClick: _cache[1] || (_cache[1] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.stripMdTitle($setup.props.node.title, 20)), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", {\n    class: \"snippet\",\n    onClick: _cache[2] || (_cache[2] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.clipText($setup.props.node.snippet, 20)), 513 /* TEXT, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vShow, !$setup.mq.sm]]), $setup.sortKey === $setup.CONST.nodeSortType.ModifiedAt ? ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"td\", {\n    key: 0,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"time\", {\n      'time-sm': $setup.mq.sm\n    }]),\n    onClick: _cache[3] || (_cache[3] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localApproximate($setup.props.node.modifiedAt)), 3 /* TEXT, CLASS */)) : ((0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"td\", {\n    key: 1,\n    class: (0,vue__WEBPACK_IMPORTED_MODULE_0__.normalizeClass)([\"time\", {\n      'time-sm': $setup.mq.sm\n    }]),\n    onClick: _cache[4] || (_cache[4] = $event => $setup.push2Page($setup.props.node.id))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.utc2localApproximate($setup.props.node.createdAt)), 3 /* TEXT, CLASS */)), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"td\", null, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createVNode)($setup[\"NodeOperations\"], {\n    node: $setup.props.node\n  }, null, 8 /* PROPS */, [\"node\"])])], 64 /* STABLE_FRAGMENT */);\n}\n\n//# sourceURL=webpack://rethink/./src/components/app/nodesDisplay/display/ListNode.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/nodesDisplay/display/NodeOperations.vue?vue&type=template&id=6484916a&scoped=true&ts=true":
             /*!***********************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -2045,15 +2071,15 @@
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/signin/LoginPanel.vue?vue&type=template&id=249a04e8&scoped=true&ts=true":
             /*!*************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/signin/LoginPanel.vue?vue&type=template&id=249a04e8&scoped=true&ts=true ***!
   \*************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-249a04e8\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"login-register-form\"\n};\nconst _hoisted_2 = {\n  class: \"flow-label\",\n  for: \"account\"\n};\nconst _hoisted_3 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n  class: \"required\"\n}, \"*\", -1 /* HOISTED */));\nconst _hoisted_4 = {\n  class: \"flow-input\"\n};\nconst _hoisted_5 = [\"placeholder\", \"title\"];\nconst _hoisted_6 = {\n  class: \"flow-label\",\n  for: \"password\"\n};\nconst _hoisted_7 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n  class: \"required\"\n}, \"*\", -1 /* HOISTED */));\nconst _hoisted_8 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"br\", null, null, -1 /* HOISTED */));\nconst _hoisted_9 = {\n  style: {\n    \"font-weight\": \"normal\",\n    \"font-size\": \"0.8em\",\n    \"color\": \"grey\"\n  }\n};\nconst _hoisted_10 = {\n  class: \"flow-input\"\n};\nconst _hoisted_11 = [\"src\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"label\", _hoisted_2, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)((0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewAccountLabel\")), 1 /* TEXT */), _hoisted_3]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_4, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: \"account\",\n    \"onUpdate:modelValue\": _cache[0] || (_cache[0] = $event => $setup.account = $event),\n    placeholder: $setup.mLang.get('loginViewAccountPlaceholder'),\n    title: $setup.mLang.get('loginViewAccountInputTitle'),\n    name: \"account\",\n    required: \"\",\n    type: \"email\"\n  }, null, 8 /* PROPS */, _hoisted_5), [[vue__WEBPACK_IMPORTED_MODULE_0__.vModelText, $setup.account, void 0, {\n    trim: true\n  }]])]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"label\", _hoisted_6, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)((0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewPasswordLabel\")), 1 /* TEXT */), _hoisted_7, (0,vue__WEBPACK_IMPORTED_MODULE_0__.createCommentVNode)(\" TODO 一个月后去掉这个\"), _hoisted_8, (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", _hoisted_9, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)(\" 2024年2月22日进行了安全升级，如登录失败，请点击\"), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"a\", {\n    style: {\n      \"color\": \"#0E0EFF\"\n    },\n    onClick: _cache[1] || (_cache[1] = $event => $setup.emit('showForgetPasswordWindow'))\n  }, \"忘记密码\"), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)(\"，进行密码重置。 \")])]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_10, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: \"password\",\n    ref: \"passwordElement\",\n    \"onUpdate:modelValue\": _cache[2] || (_cache[2] = $event => $setup.password = $event),\n    name: \"password\",\n    required: \"\",\n    type: \"password\",\n    onKeydown: _cache[3] || (_cache[3] = (0,vue__WEBPACK_IMPORTED_MODULE_0__.withKeys)(\n    //@ts-ignore\n    (...args) => $setup.loginByEnter && $setup.loginByEnter(...args), [\"enter\"]))\n  }, null, 544 /* NEED_HYDRATION, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vModelText, $setup.password, void 0, {\n    trim: true\n  }]]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"show-hide-password\",\n    tabindex: \"-1\",\n    onClick: _cache[4] || (_cache[4] =\n    //@ts-ignore\n    (...args) => $setup.showHidePassword && $setup.showHidePassword(...args))\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"img\", {\n    src: $setup.EyeOpenIcon,\n    alt: \"view\"\n  }, null, 8 /* PROPS */, _hoisted_11)])]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n    class: \"forget-password\",\n    onClick: _cache[5] || (_cache[5] = $event => $setup.emit('showForgetPasswordWindow'))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewForgetPassword\")), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"login-button\",\n    onClick: _cache[6] || (_cache[6] =\n    //@ts-ignore\n    (...args) => $setup.handleLogin && $setup.handleLogin(...args))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('loginViewLoginButton')), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"signup-button\",\n    onClick: _cache[7] || (_cache[7] = $event => $setup.emit('showSignupWindow'))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('loginViewSignupButton')), 1 /* TEXT */)]);\n}\n\n//# sourceURL=webpack://rethink/./src/components/signin/LoginPanel.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* binding */ render; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n\nconst _withScopeId = n => ((0,vue__WEBPACK_IMPORTED_MODULE_0__.pushScopeId)(\"data-v-249a04e8\"), n = n(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.popScopeId)(), n);\nconst _hoisted_1 = {\n  class: \"login-register-form\"\n};\nconst _hoisted_2 = {\n  class: \"flow-label\",\n  for: \"account\"\n};\nconst _hoisted_3 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n  class: \"required\"\n}, \"*\", -1 /* HOISTED */));\nconst _hoisted_4 = {\n  class: \"flow-input\"\n};\nconst _hoisted_5 = [\"placeholder\", \"title\"];\nconst _hoisted_6 = {\n  class: \"flow-label\",\n  for: \"password\"\n};\nconst _hoisted_7 = /*#__PURE__*/_withScopeId(() => /*#__PURE__*/(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n  class: \"required\"\n}, \"*\", -1 /* HOISTED */));\nconst _hoisted_8 = {\n  class: \"flow-input\"\n};\nconst _hoisted_9 = [\"src\"];\nfunction render(_ctx, _cache, $props, $setup, $data, $options) {\n  return (0,vue__WEBPACK_IMPORTED_MODULE_0__.openBlock)(), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementBlock)(\"div\", _hoisted_1, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"label\", _hoisted_2, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)((0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewAccountLabel\")), 1 /* TEXT */), _hoisted_3]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_4, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: \"account\",\n    \"onUpdate:modelValue\": _cache[0] || (_cache[0] = $event => $setup.account = $event),\n    placeholder: $setup.mLang.get('loginViewAccountPlaceholder'),\n    title: $setup.mLang.get('loginViewAccountInputTitle'),\n    name: \"account\",\n    required: \"\",\n    type: \"email\"\n  }, null, 8 /* PROPS */, _hoisted_5), [[vue__WEBPACK_IMPORTED_MODULE_0__.vModelText, $setup.account, void 0, {\n    trim: true\n  }]])]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"label\", _hoisted_6, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createTextVNode)((0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewPasswordLabel\")), 1 /* TEXT */), _hoisted_7]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"div\", _hoisted_8, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.withDirectives)((0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"input\", {\n    id: \"password\",\n    ref: \"passwordElement\",\n    \"onUpdate:modelValue\": _cache[1] || (_cache[1] = $event => $setup.password = $event),\n    name: \"password\",\n    required: \"\",\n    type: \"password\",\n    onKeydown: _cache[2] || (_cache[2] = (0,vue__WEBPACK_IMPORTED_MODULE_0__.withKeys)(\n    //@ts-ignore\n    (...args) => $setup.loginByEnter && $setup.loginByEnter(...args), [\"enter\"]))\n  }, null, 544 /* NEED_HYDRATION, NEED_PATCH */), [[vue__WEBPACK_IMPORTED_MODULE_0__.vModelText, $setup.password, void 0, {\n    trim: true\n  }]]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"show-hide-password\",\n    tabindex: \"-1\",\n    onClick: _cache[3] || (_cache[3] =\n    //@ts-ignore\n    (...args) => $setup.showHidePassword && $setup.showHidePassword(...args))\n  }, [(0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"img\", {\n    src: $setup.EyeOpenIcon,\n    alt: \"view\"\n  }, null, 8 /* PROPS */, _hoisted_9)])]), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"span\", {\n    class: \"forget-password\",\n    onClick: _cache[4] || (_cache[4] = $event => $setup.emit('showForgetPasswordWindow'))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get(\"loginViewForgetPassword\")), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"login-button\",\n    onClick: _cache[5] || (_cache[5] =\n    //@ts-ignore\n    (...args) => $setup.handleLogin && $setup.handleLogin(...args))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('loginViewLoginButton')), 1 /* TEXT */), (0,vue__WEBPACK_IMPORTED_MODULE_0__.createElementVNode)(\"button\", {\n    class: \"signup-button\",\n    onClick: _cache[6] || (_cache[6] = $event => $setup.emit('showSignupWindow'))\n  }, (0,vue__WEBPACK_IMPORTED_MODULE_0__.toDisplayString)($setup.mLang.get('loginViewSignupButton')), 1 /* TEXT */)]);\n}\n\n//# sourceURL=webpack://rethink/./src/components/signin/LoginPanel.vue?./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use%5B1%5D!./node_modules/vue-loader/dist/templateLoader.js??ruleSet%5B1%5D.rules%5B4%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
         "./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/signin/OauthButton.vue?vue&type=template&id=61b664a8&scoped=true&ts=true":
             /*!**************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
@@ -2435,15 +2461,15 @@
         "./src/utils/app/dataImport/importProcess.ts":
             /*!***************************************************!*\
   !*** ./src/utils/app/dataImport/importProcess.ts ***!
   \***************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var axios__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! axios */ \"./node_modules/axios/lib/axios.js\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_requestId__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/requestId */ \"./src/utils/requestId.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n\n\n\n\n\n\nfunction useImportProcess() {\n  const process = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(0);\n  const jobName = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(\"\");\n  const startAt = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(\"\");\n  const msg = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)([]);\n  const code = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(0);\n  const hasTask = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(false);\n  const timer = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(null);\n  async function renewProcess() {\n    try {\n      const resp = await axios__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(`${_utils_configs__WEBPACK_IMPORTED_MODULE_1__[\"default\"].apiUrl}/api/files/uploadProcess`, {\n        headers: {\n          token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_3__.getToken)(),\n          rid: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_2__[\"default\"])()\n        }\n      });\n      if (resp.status !== 200) {\n        console.log(resp);\n        return;\n      }\n      process.value = resp.data.process;\n      jobName.value = resp.data.type;\n      startAt.value = (0,_utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__.utc2local)(resp.data.startAt);\n      msg.value = resp.data.msg;\n      code.value = resp.data.code;\n      hasTask.value = resp.data.startAt !== \"\";\n    } catch (err) {\n      console.log(err);\n    }\n  }\n  (0,vue__WEBPACK_IMPORTED_MODULE_0__.onMounted)(async () => {\n    await renewProcess();\n    timer.value = setInterval(renewProcess, 5000);\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_0__.onUnmounted)(() => {\n    if (!timer.value) return;\n    clearInterval(timer.value);\n    timer.value = null;\n  });\n  return {\n    process,\n    jobName,\n    startAt,\n    msg,\n    code,\n    hasTask\n  };\n}\n/* harmony default export */ __webpack_exports__[\"default\"] = (useImportProcess);\n\n//# sourceURL=webpack://rethink/./src/utils/app/dataImport/importProcess.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var axios__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! axios */ \"./node_modules/axios/lib/axios.js\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_requestId__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/requestId */ \"./src/utils/requestId.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/textOps */ \"./src/utils/app/textOps.ts\");\n\n\n\n\n\n\nfunction useImportProcess() {\n  const process = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(0);\n  const jobName = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(\"\");\n  const startAt = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(\"\");\n  const msg = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)([]);\n  const code = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(0);\n  const hasTask = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(false);\n  const timer = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)(null);\n  async function renewProcess() {\n    try {\n      const resp = await axios__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(`${_utils_configs__WEBPACK_IMPORTED_MODULE_1__[\"default\"].apiUrl}/api/files/uploadProcess`, {\n        headers: {\n          token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_3__.getToken)(),\n          rid: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_2__[\"default\"])()\n        }\n      });\n      if (resp.status !== 200) {\n        console.log(resp);\n        return;\n      }\n      process.value = resp.data.process;\n      jobName.value = resp.data.type;\n      startAt.value = (0,_utils_app_textOps__WEBPACK_IMPORTED_MODULE_4__.utc2localApproximate)(resp.data.startAt);\n      msg.value = resp.data.msg;\n      code.value = resp.data.code;\n      hasTask.value = resp.data.startAt !== \"\";\n    } catch (err) {\n      console.log(err);\n    }\n  }\n  (0,vue__WEBPACK_IMPORTED_MODULE_0__.onMounted)(async () => {\n    await renewProcess();\n    timer.value = setInterval(renewProcess, 5000);\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_0__.onUnmounted)(() => {\n    if (!timer.value) return;\n    clearInterval(timer.value);\n    timer.value = null;\n  });\n  return {\n    process,\n    jobName,\n    startAt,\n    msg,\n    code,\n    hasTask\n  };\n}\n/* harmony default export */ __webpack_exports__[\"default\"] = (useImportProcess);\n\n//# sourceURL=webpack://rethink/./src/utils/app/dataImport/importProcess.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/dropFile.ts":
             /*!***********************************!*\
@@ -2487,15 +2513,15 @@
         "./src/utils/app/editor/editor.ts":
             /*!****************************************!*\
   !*** ./src/utils/app/editor/editor.ts ***!
   \****************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vditor__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vditor */ \"./node_modules/vditor/dist/index.min.js\");\n/* harmony import */ var vditor__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(vditor__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _assets_css_vditor_vditor_css__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/assets/css/vditor/vditor.css */ \"./src/assets/css/vditor/vditor.css\");\n/* harmony import */ var vue_router__WEBPACK_IMPORTED_MODULE_20__ = __webpack_require__(/*! vue-router */ \"./node_modules/vue-router/dist/vue-router.mjs\");\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_node__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/app/node */ \"./src/utils/app/node.ts\");\n/* harmony import */ var _router__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/router */ \"./src/router/index.ts\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__(/*! @/utils/app/editor/atTag */ \"./src/utils/app/editor/atTag.ts\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/keyEvent */ \"./src/utils/app/editor/eventHandle/keyEvent.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_meta__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__(/*! @/utils/meta */ \"./src/utils/meta.ts\");\n/* harmony import */ var _utils_app_editor_recommend__WEBPACK_IMPORTED_MODULE_14__ = __webpack_require__(/*! @/utils/app/editor/recommend */ \"./src/utils/app/editor/recommend.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_15__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/codeBlock */ \"./src/utils/app/editor/eventHandle/codeBlock.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/updateOutline */ \"./src/utils/app/editor/eventHandle/updateOutline.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/updateSyncTime */ \"./src/utils/app/editor/eventHandle/updateSyncTime.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/checkbox */ \"./src/utils/app/editor/eventHandle/checkbox.ts\");\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nconst ready = (0,vue__WEBPACK_IMPORTED_MODULE_2__.ref)(false);\nasync function updateTextEl() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n  (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_9__.replaceATag)();\n}\nlet mobileFocused = false;\nfunction createEditor(id) {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value || !_utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value) return;\n  const text = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md);\n  let toolbar;\n  if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n    toolbar = [\"undo\", \"redo\", \"headings\", \"check\", \"upload\"];\n  } else {\n    toolbar = [\"outline\", \"|\", \"undo\", \"redo\", \"|\", \"headings\", \"check\", \"code\", \"table\", \"upload\", \"|\", \"fullscreen\"];\n  }\n  const ideaColor = \"#f87575\";\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value = new (vditor__WEBPACK_IMPORTED_MODULE_0___default())(id, {\n    cdn: _utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].vditorCDN,\n    width: \"100%\",\n    icon: \"material\",\n    lang: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].getGlobalLang() === \"zh\" ? \"zh_CN\" : \"en_US\",\n    mode: _utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value.settings.editorMode,\n    placeholder: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"editorContentPlaceholder\"),\n    outline: {\n      enable: false,\n      position: \"left\"\n    },\n    tab: \"    \",\n    // comment: {enable: true,},\n    toolbar: [{\n      name: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"goBackIcon\"),\n      tipPosition: \"nw\",\n      tip: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"goBackIcon\"),\n      icon: '<svg width=\"800px\" height=\"800px\" viewBox=\"0 0 1024 1024\" xmlns=\"http://www.w3.org/2000/svg\">\\n' + '    <path fill=\"#000000\" d=\"M224 480h640a32 32 0 1 1 0 64H224a32 32 0 0 1 0-64z\"/>\\n' + '    <path fill=\"#000000\"\\n' + '          d=\"m237.248 512 265.408 265.344a32 32 0 0 1-45.312 45.312l-288-288a32 32 0 0 1 ' + '0-45.312l288-288a32 32 0 1 1 45.312 45.312L237.248 512z\"/>\\n' + '</svg>',\n      click: () => _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1)\n    }, {\n      name: \"idea\",\n      tipPosition: \"nw\",\n      tip: \"idea\",\n      icon: `<svg fill=\"${ideaColor}\" width=\"194px\" height=\"194px\" viewBox=\"0 0 32.00 32.00\" id=\"icon\"` + ` xmlns=\"http://www.w3.org/2000/svg\" stroke=\"${ideaColor}\" stroke-width=\"0.8\">` + '<g id=\"SVGRepo_bgCarrier\" stroke-width=\"0\"/>' + '<g id=\"SVGRepo_tracerCarrier\" stroke-linecap=\"round\" stroke-linejoin=\"round\"/>' + '<g id=\"SVGRepo_iconCarrier\"><defs><style>.cls-1{fill:none;}</style></defs><title>' + 'idea</title><rect x=\"11\" y=\"24\" width=\"10\" height=\"2\"/><rect x=\"13\" y=\"28\" width=\"6\" height=\"2\"/>' + '<path d=\"M16,2A10,10,0,0,0,6,12a9.19,9.19,0,0,0,3.46,7.62c1,.93,1.54,1.46,1.54,2.38h2c0-1.84-1.11-' + '2.87-2.19-3.86A7.2,7.2,0,0,1,8,12a8,8,0,0,1,16,0,7.2,7.2,0,0,1-2.82,6.14c-1.07,1-2.18,2-2.18,3.86h2c0-' + '.92.53-1.45,1.54-2.39A9.18,9.18,0,0,0,26,12,10,10,0,0,0,16,2Z\" transform=\"translate(0 0)\"/></g></svg>',\n      click: () => {\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar) return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements) return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements.idea) return;\n        // change the icon svg color to blue\n        const icon = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements.idea;\n        const svg = icon.children[0].children[0];\n        if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value) {\n          svg.setAttribute(\"stroke\", ideaColor);\n          svg.setAttribute(\"fill\", ideaColor);\n        } else {\n          svg.setAttribute(\"stroke\", \"#586069\");\n          svg.setAttribute(\"fill\", \"#586069\");\n        }\n        _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value = !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value;\n      }\n    }, ...toolbar],\n    toolbarConfig: {\n      hide: false,\n      pin: true\n    },\n    undoDelay: 500,\n    upload: {\n      // 图片, audio, video, application/pdf, text/*\n      accept: \"image/*,\" + \"video/*,\" + \"audio/*,\" + \"application/pdf,\" + \"text/*,\" + \"application/msword,\" + \"application/vnd.openxmlformats-officedocument.wordprocessingml.document,\" + \"application/vnd.ms-excel,\" + \"application/vnd.openxmlformats-officedocument.spreadsheetml.sheet,\" + \"application/vnd.ms-powerpoint,\" + \"application/vnd.openxmlformats-officedocument.presentationml.presentation\",\n      max: 50 * 1024 * 1024,\n      headers: {\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_12__.getToken)()\n      },\n      multiple: false,\n      url: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].apiUrl}/api/files/vditor/upload`,\n      linkToImgUrl: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].apiUrl}/api/files/vditor/imageFetch`,\n      filename(name) {\n        // eslint-disable-next-line no-useless-escape\n        return name.replace(/[^(a-zA-Z0-9\\u4e00-\\u9fa5\\.)]/g, '').\n        // eslint-disable-next-line no-useless-escape\n        replace(/[\\?\\\\/:|<>\\*\\[\\]\\(\\)\\$%\\{\\}@~]/g, '').replace('/\\\\s/g', '');\n      }\n    },\n    preview: {\n      markdown: {\n        sanitize: true,\n        // gfmAutoLink: true,\n        mark: true,\n        codeBlockPreview: true\n        // autoSpace: true,\n        // linkPrefix: \"https://\",\n      },\n      hljs: {\n        enable: true,\n        lineNumber: false,\n        defaultLang: \"python\",\n        style: _utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value.settings.editorCodeTheme,\n        langs: [\"bash\", \"c\", \"csharp\", \"cpp\", \"css\", \"diff\", \"go\", \"xml\", \"http\", \"html\", \"java\", \"javascript\", \"json\", \"lua\", \"markdown\", \"nginx\", \"php\", \"python\", \"r\", \"ruby\", \"scss\", \"shell\", \"sql\", \"swift\", \"typescript\", \"xml\", \"yaml\", \"matlab\"]\n      },\n      theme: {\n        current: \"light\",\n        path: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].vditorCDN}/dist/css/content-theme`\n      }\n    },\n    cache: {\n      enable: true,\n      id: _utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].mdCacheId,\n      after: async md => {\n        const updated = await trySyncNode(md);\n        if (!updated) return;\n        await updateTextEl();\n        (0,_utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__.updateSyncStatue)();\n        (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav)();\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n        await (0,_utils_app_editor_recommend__WEBPACK_IMPORTED_MODULE_14__.resetRecommend)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.id);\n      }\n    },\n    image: {\n      preview: bom => {\n        // if external link, open a confirm dialog\n        let src = null;\n        if (bom.classList.contains(\"vditor-ir__marker--link\")) {\n          // the bom is looks like: <span class=\"vditor-ir__marker vditor-ir__marker--link\">https://baidu.com</span>\n          src = bom.textContent;\n        } else {\n          // the bom is looks like: <img src=\"https://baidu.com\">\n          src = bom.getAttribute(\"src\") || \"\";\n        }\n        if (!src) return;\n        if (src.startsWith(\"http\")) {\n          // create a new div to show the image\n          // this div is on top of the editor, it has a cross to close the div\n          const div = document.createElement(\"div\");\n          div.style.position = \"fixed\";\n          div.style.top = \"0\";\n          div.style.left = \"0\";\n          div.style.width = \"100%\";\n          div.style.height = \"100%\";\n          div.style.zIndex = \"999\";\n          div.style.backgroundColor = \"rgba(0, 0, 0, 0.8)\";\n          div.style.display = \"flex\";\n          div.style.alignItems = \"center\";\n          div.style.justifyContent = \"center\";\n          div.addEventListener(\"click\", () => {\n            div.remove();\n          });\n          const img = document.createElement(\"img\");\n          img.src = src;\n          // set img init width to 90% of the screen\n          // but when the height exceeds the screen, set width to auto and height to 90%\n          img.style.width = \"90%\";\n          img.style.objectFit = \"contain\";\n          img.addEventListener(\"load\", () => {\n            if (img.height > window.innerHeight) {\n              img.style.width = \"auto\";\n              img.style.height = \"90%\";\n            }\n          });\n          div.appendChild(img);\n          document.body.appendChild(div);\n        }\n      }\n    },\n    after: async () => {\n      if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.setValue(text);\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.getValue();\n      await updateTextEl();\n      const el = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.element;\n      // when cursor selection changed, hide the preview element\n      for (const eventName of [\"input\", \"keyup\", \"compositionend\", \"click\"]) {\n        el.addEventListener(eventName, _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__.hideCodePreview);\n      }\n      el.addEventListener(\"keyup\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.onKeyup);\n      // when at mobie mode, click the editor, set the editor's height to 40%\n      el.addEventListener(\"click\", e => {\n        if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() !== \"sm\") return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n        // editor.value.vditor.element.style.height = \"auto\"\n        if (mobileFocused) return;\n        e.target.scrollIntoView({\n          behavior: \"smooth\",\n          block: \"center\"\n        });\n        mobileFocused = true;\n      });\n      // add checkbox click event\n      el.addEventListener(\"click\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.handleCheckBox);\n      (0,_utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed)();\n      // check @ input\n      el.addEventListener(\"beforeinput\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.beforeInput);\n      if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n        el.blur();\n        // move toolbar to outside of the editor\n        const toolbar = el.querySelector(\".vditor-toolbar\");\n        if (toolbar) {\n          const parentEl = document.querySelector(\"#sm-sticky-panel\");\n          parentEl?.appendChild(toolbar);\n        }\n      }\n      // outline button click event\n      (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.getOutlineNav)()?.addEventListener(\"click\", _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav);\n      ready.value = true;\n    },\n    blur: () => {\n      if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n      if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n        mobileFocused = false;\n      }\n    }\n  });\n}\nasync function trySyncNode(md = \"\") {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return false;\n  if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n    if (md === \"\") {\n      md = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.getValue().trim();\n    }\n    md = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(md.trim());\n    // skip if not changed\n    const oldMd = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md.trim());\n    if (oldMd !== md) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.updateNode)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.id, md);\n      return true;\n    }\n  }\n  return false;\n}\nfunction useEditor(id, nid) {\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onBeforeMount)(() => {\n    ready.value = false;\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onMounted)(async () => {\n    // reset recommendNodes\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.recommendNodes.value = [];\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.getNode)(nid);\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n      _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1);\n      return;\n    }\n    createEditor(id);\n    (0,_utils_meta__WEBPACK_IMPORTED_MODULE_13__[\"default\"])(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title + \" - Rethink\", _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title, _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.snippet);\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editorSyncStatus.value = _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"editorSyncStatusLastSaved\") + (0,_utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__.syncTimeString)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.modifiedAt);\n  });\n  (0,vue_router__WEBPACK_IMPORTED_MODULE_20__.onBeforeRouteUpdate)(async (to, from, next) => {\n    if (to.params.id === from.params.id) return next();\n    // for the case that the node is changed\n    // hide the at-search-result\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.isAtSearch.value = false;\n    // reset the linedNodeExpanded\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.linedNodeExpanded.value.forEach((_, i) => {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.linedNodeExpanded.value[i] = false;\n    });\n    if (typeof to.params.id !== \"string\") return next(false);\n    // get new node\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.getNode)(to.params.id);\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n      _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1);\n      return next(false);\n    }\n    // reset editor\n    if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.setValue((0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md));\n      // change HTML document\n      (0,_utils_meta__WEBPACK_IMPORTED_MODULE_13__[\"default\"])(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title + \" - Rethink\", _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title, _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.snippet);\n      await updateTextEl();\n      (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav)();\n      (0,_utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed)();\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.clearStack();\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.clearCache();\n      // scroll to top\n      const es = document.querySelectorAll(\"pre.vditor-reset\");\n      for (const e of es) {\n        e.scroll({\n          top: 0,\n          behavior: \"smooth\"\n        });\n      }\n    }\n    // reset recommendNodes\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.recommendNodes.value = [];\n    return next();\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onUnmounted)(async () => {\n    await trySyncNode();\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n    const el = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.element;\n    el.removeEventListener(\"keyup\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.onKeyup);\n    el.removeEventListener(\"beforeinput\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.beforeInput);\n    el.removeEventListener(\"click\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.handleCheckBox);\n    for (const eventName of [\"input\", \"keyup\", \"compositionend\", \"click\"]) {\n      el.removeEventListener(eventName, _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__.hideCodePreview);\n    }\n    (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.getOutlineNav)()?.removeEventListener(\"click\", _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav);\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.destroy();\n  });\n  return {\n    node: _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node,\n    ready\n  };\n}\n/* harmony default export */ __webpack_exports__[\"default\"] = (useEditor);\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/editor.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var vditor__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vditor */ \"./node_modules/vditor/dist/index.min.js\");\n/* harmony import */ var vditor__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(vditor__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _assets_css_vditor_vditor_css__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/assets/css/vditor/vditor.css */ \"./src/assets/css/vditor/vditor.css\");\n/* harmony import */ var vue_router__WEBPACK_IMPORTED_MODULE_20__ = __webpack_require__(/*! vue-router */ \"./node_modules/vue-router/dist/vue-router.mjs\");\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_app_node__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/app/node */ \"./src/utils/app/node.ts\");\n/* harmony import */ var _router__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/router */ \"./src/router/index.ts\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__(/*! @/utils/app/editor/atTag */ \"./src/utils/app/editor/atTag.ts\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/keyEvent */ \"./src/utils/app/editor/eventHandle/keyEvent.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_meta__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__(/*! @/utils/meta */ \"./src/utils/meta.ts\");\n/* harmony import */ var _utils_app_editor_recommend__WEBPACK_IMPORTED_MODULE_14__ = __webpack_require__(/*! @/utils/app/editor/recommend */ \"./src/utils/app/editor/recommend.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_15__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/codeBlock */ \"./src/utils/app/editor/eventHandle/codeBlock.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/updateOutline */ \"./src/utils/app/editor/eventHandle/updateOutline.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/updateSyncTime */ \"./src/utils/app/editor/eventHandle/updateSyncTime.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/checkbox */ \"./src/utils/app/editor/eventHandle/checkbox.ts\");\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nconst ready = (0,vue__WEBPACK_IMPORTED_MODULE_2__.ref)(false);\nasync function updateTextEl() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n  (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_9__.replaceATag)();\n}\nlet mobileFocused = false;\nfunction createEditor(id) {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value || !_utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value) return;\n  const text = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md);\n  let toolbar;\n  if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n    toolbar = [\"undo\", \"redo\", \"headings\", \"check\", \"upload\"];\n  } else {\n    toolbar = [\"outline\", \"|\", \"undo\", \"redo\", \"|\", \"headings\", \"check\", \"code\", \"table\", \"upload\", \"|\", \"fullscreen\"];\n  }\n  const ideaColor = \"#f87575\";\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value = new (vditor__WEBPACK_IMPORTED_MODULE_0___default())(id, {\n    cdn: _utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].vditorCDN,\n    width: \"100%\",\n    icon: \"material\",\n    lang: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].getGlobalLang() === \"zh\" ? \"zh_CN\" : \"en_US\",\n    mode: _utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value.settings.editorMode,\n    placeholder: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"editorContentPlaceholder\"),\n    outline: {\n      enable: false,\n      position: \"left\"\n    },\n    tab: \"    \",\n    // comment: {enable: true,},\n    toolbar: [{\n      name: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"goBackIcon\"),\n      tipPosition: \"nw\",\n      tip: _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"goBackIcon\"),\n      icon: '<svg width=\"800px\" height=\"800px\" viewBox=\"0 0 1024 1024\" xmlns=\"http://www.w3.org/2000/svg\">\\n' + '    <path fill=\"#000000\" d=\"M224 480h640a32 32 0 1 1 0 64H224a32 32 0 0 1 0-64z\"/>\\n' + '    <path fill=\"#000000\"\\n' + '          d=\"m237.248 512 265.408 265.344a32 32 0 0 1-45.312 45.312l-288-288a32 32 0 0 1 ' + '0-45.312l288-288a32 32 0 1 1 45.312 45.312L237.248 512z\"/>\\n' + '</svg>',\n      click: () => _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1)\n    }, {\n      name: \"idea\",\n      tipPosition: \"nw\",\n      tip: \"idea\",\n      icon: `<svg fill=\"${ideaColor}\" width=\"194px\" height=\"194px\" viewBox=\"0 0 32.00 32.00\" id=\"icon\"` + ` xmlns=\"http://www.w3.org/2000/svg\" stroke=\"${ideaColor}\" stroke-width=\"0.8\">` + '<g id=\"SVGRepo_bgCarrier\" stroke-width=\"0\"/>' + '<g id=\"SVGRepo_tracerCarrier\" stroke-linecap=\"round\" stroke-linejoin=\"round\"/>' + '<g id=\"SVGRepo_iconCarrier\"><defs><style>.cls-1{fill:none;}</style></defs><title>' + 'idea</title><rect x=\"11\" y=\"24\" width=\"10\" height=\"2\"/><rect x=\"13\" y=\"28\" width=\"6\" height=\"2\"/>' + '<path d=\"M16,2A10,10,0,0,0,6,12a9.19,9.19,0,0,0,3.46,7.62c1,.93,1.54,1.46,1.54,2.38h2c0-1.84-1.11-' + '2.87-2.19-3.86A7.2,7.2,0,0,1,8,12a8,8,0,0,1,16,0,7.2,7.2,0,0,1-2.82,6.14c-1.07,1-2.18,2-2.18,3.86h2c0-' + '.92.53-1.45,1.54-2.39A9.18,9.18,0,0,0,26,12,10,10,0,0,0,16,2Z\" transform=\"translate(0 0)\"/></g></svg>',\n      click: () => {\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar) return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements) return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements.idea) return;\n        // change the icon svg color to blue\n        const icon = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.toolbar.elements.idea;\n        const svg = icon.children[0].children[0];\n        if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value) {\n          svg.setAttribute(\"stroke\", ideaColor);\n          svg.setAttribute(\"fill\", ideaColor);\n        } else {\n          svg.setAttribute(\"stroke\", \"#586069\");\n          svg.setAttribute(\"fill\", \"#586069\");\n        }\n        _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value = !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.collapseRecommend.value;\n      }\n    }, ...toolbar],\n    toolbarConfig: {\n      hide: false,\n      pin: true\n    },\n    undoDelay: 500,\n    upload: {\n      // 图片, audio, video, application/pdf, text/*\n      accept: \"image/*,\" + \"video/*,\" + \"audio/*,\" + \"application/pdf,\" + \"text/*,\" + \"application/msword,\" + \"application/vnd.openxmlformats-officedocument.wordprocessingml.document,\" + \"application/vnd.ms-excel,\" + \"application/vnd.openxmlformats-officedocument.spreadsheetml.sheet,\" + \"application/vnd.ms-powerpoint,\" + \"application/vnd.openxmlformats-officedocument.presentationml.presentation\",\n      max: 50 * 1024 * 1024,\n      headers: {\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_12__.getToken)()\n      },\n      multiple: false,\n      url: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].apiUrl}/api/files/vditor/upload`,\n      linkToImgUrl: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].apiUrl}/api/files/vditor/imageFetch`,\n      filename(name) {\n        // eslint-disable-next-line no-useless-escape\n        return name.replace(/[^(a-zA-Z0-9\\u4e00-\\u9fa5\\.)]/g, '').\n        // eslint-disable-next-line no-useless-escape\n        replace(/[\\?\\\\/:|<>\\*\\[\\]\\(\\)\\$%\\{\\}@~]/g, '').replace('/\\\\s/g', '');\n      }\n    },\n    preview: {\n      markdown: {\n        sanitize: true,\n        // gfmAutoLink: true,\n        mark: true,\n        codeBlockPreview: true\n        // autoSpace: true,\n        // linkPrefix: \"https://\",\n      },\n      hljs: {\n        enable: true,\n        lineNumber: false,\n        defaultLang: \"python\",\n        style: _utils_app_user__WEBPACK_IMPORTED_MODULE_15__.user.value.settings.editorCodeTheme,\n        langs: [\"bash\", \"c\", \"csharp\", \"cpp\", \"css\", \"diff\", \"go\", \"xml\", \"http\", \"html\", \"java\", \"javascript\", \"json\", \"lua\", \"markdown\", \"nginx\", \"php\", \"python\", \"r\", \"ruby\", \"scss\", \"shell\", \"sql\", \"swift\", \"typescript\", \"xml\", \"yaml\", \"matlab\"]\n      },\n      theme: {\n        current: \"light\",\n        path: `${_utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].vditorCDN}/dist/css/content-theme`\n      }\n    },\n    cache: {\n      enable: true,\n      id: _utils_configs__WEBPACK_IMPORTED_MODULE_6__[\"default\"].mdCacheId,\n      after: async md => {\n        const updated = await trySyncNode(md);\n        if (!updated) return;\n        await updateTextEl();\n        (0,_utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__.updateSyncStatue)();\n        (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav)();\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n        await (0,_utils_app_editor_recommend__WEBPACK_IMPORTED_MODULE_14__.resetRecommend)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.id);\n      }\n    },\n    image: {\n      preview: bom => {\n        // if external link, open a confirm dialog\n        let src = null;\n        if (bom.classList.contains(\"vditor-ir__marker--link\")) {\n          // the bom is looks like: <span class=\"vditor-ir__marker vditor-ir__marker--link\">https://baidu.com</span>\n          src = bom.textContent;\n        } else {\n          // the bom is looks like: <img src=\"https://baidu.com\">\n          src = bom.getAttribute(\"src\") || \"\";\n        }\n        if (!src) return;\n        if (src.startsWith(\"http\")) {\n          // create a new div to show the image\n          // this div is on top of the editor, it has a cross to close the div\n          const div = document.createElement(\"div\");\n          div.style.position = \"fixed\";\n          div.style.top = \"0\";\n          div.style.left = \"0\";\n          div.style.width = \"100%\";\n          div.style.height = \"100%\";\n          div.style.zIndex = \"999\";\n          div.style.backgroundColor = \"rgba(0, 0, 0, 0.8)\";\n          div.style.display = \"flex\";\n          div.style.alignItems = \"center\";\n          div.style.justifyContent = \"center\";\n          div.addEventListener(\"click\", () => {\n            div.remove();\n          });\n          const img = document.createElement(\"img\");\n          img.src = src;\n          // set img init width to 90% of the screen\n          // but when the height exceeds the screen, set width to auto and height to 90%\n          img.style.width = \"90%\";\n          img.style.objectFit = \"contain\";\n          img.addEventListener(\"load\", () => {\n            if (img.height > window.innerHeight) {\n              img.style.width = \"auto\";\n              img.style.height = \"90%\";\n            }\n          });\n          div.appendChild(img);\n          document.body.appendChild(div);\n        }\n      }\n    },\n    after: async () => {\n      if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) return;\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.setValue(text);\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.getValue();\n      await updateTextEl();\n      const el = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.element;\n      // when cursor selection changed, hide the preview element\n      for (const eventName of [\"input\", \"keyup\", \"compositionend\", \"click\"]) {\n        el.addEventListener(eventName, _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__.hideCodePreview);\n        el.addEventListener(eventName, _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.recordRange);\n      }\n      el.addEventListener(\"keyup\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.onKeyup);\n      // when at mobie mode, click the editor, set the editor's height to 40%\n      el.addEventListener(\"click\", e => {\n        if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() !== \"sm\") return;\n        if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n        // editor.value.vditor.element.style.height = \"auto\"\n        if (mobileFocused) return;\n        e.target.scrollIntoView({\n          behavior: \"smooth\",\n          block: \"center\"\n        });\n        mobileFocused = true;\n      });\n      // add checkbox click event\n      el.addEventListener(\"click\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.handleCheckBox);\n      (0,_utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed)();\n      el.addEventListener(\"input\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed);\n      // check @ input\n      el.addEventListener(\"beforeinput\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.beforeInput);\n      if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n        el.blur();\n        // move toolbar to outside of the editor\n        const toolbar = el.querySelector(\".vditor-toolbar\");\n        if (toolbar) {\n          const parentEl = document.querySelector(\"#sm-sticky-panel\");\n          parentEl?.appendChild(toolbar);\n        }\n      }\n      // outline button click event\n      (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.getOutlineNav)()?.addEventListener(\"click\", _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav);\n      ready.value = true;\n    },\n    blur: () => {\n      if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n      if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_10__.getMQ)() === \"sm\") {\n        mobileFocused = false;\n      }\n    }\n  });\n}\nasync function trySyncNode(md = \"\") {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return false;\n  if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n    if (md === \"\") {\n      md = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.getValue().trim();\n    }\n    md = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(md.trim());\n    // skip if not changed\n    const oldMd = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md.trim());\n    if (oldMd !== md) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.updateNode)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.id, md);\n      return true;\n    }\n  }\n  return false;\n}\nfunction useEditor(id, nid) {\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onBeforeMount)(() => {\n    ready.value = false;\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onMounted)(async () => {\n    // reset recommendNodes\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.recommendNodes.value = [];\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.getNode)(nid);\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n      _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1);\n      return;\n    }\n    createEditor(id);\n    (0,_utils_meta__WEBPACK_IMPORTED_MODULE_13__[\"default\"])(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title + \" - Rethink\", _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title, _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.snippet);\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editorSyncStatus.value = _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"editorSyncStatusLastSaved\") + (0,_utils_app_editor_eventHandle_updateSyncTime__WEBPACK_IMPORTED_MODULE_18__.syncTimeString)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.modifiedAt);\n  });\n  (0,vue_router__WEBPACK_IMPORTED_MODULE_20__.onBeforeRouteUpdate)(async (to, from, next) => {\n    if (to.params.id === from.params.id) return next();\n    // for the case that the node is changed\n    // hide the at-search-result\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.isAtSearch.value = false;\n    // reset the linedNodeExpanded\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.linedNodeExpanded.value.forEach((_, i) => {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.linedNodeExpanded.value[i] = false;\n    });\n    if (typeof to.params.id !== \"string\") return next(false);\n    // get new node\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_3__.getNode)(to.params.id);\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value) {\n      _router__WEBPACK_IMPORTED_MODULE_4__[\"default\"].go(-1);\n      return next(false);\n    }\n    // reset editor\n    if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.setValue((0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_8__.stripWhitespace)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.md));\n      // change HTML document\n      (0,_utils_meta__WEBPACK_IMPORTED_MODULE_13__[\"default\"])(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title + \" - Rethink\", _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.title, _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node.value.snippet);\n      await updateTextEl();\n      (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav)();\n      (0,_utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed)();\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.clearStack();\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.clearCache();\n      // scroll to top\n      const es = document.querySelectorAll(\"pre.vditor-reset\");\n      for (const e of es) {\n        e.scroll({\n          top: 0,\n          behavior: \"smooth\"\n        });\n      }\n    }\n    // reset recommendNodes\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.recommendNodes.value = [];\n    return next();\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_2__.onUnmounted)(async () => {\n    await trySyncNode();\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value) return;\n    const el = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.vditor.element;\n    el.removeEventListener(\"keyup\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.onKeyup);\n    el.removeEventListener(\"beforeinput\", _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.beforeInput);\n    el.removeEventListener(\"click\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.handleCheckBox);\n    for (const eventName of [\"input\", \"keyup\", \"compositionend\", \"click\"]) {\n      el.removeEventListener(eventName, _utils_app_editor_eventHandle_codeBlock__WEBPACK_IMPORTED_MODULE_16__.hideCodePreview);\n      el.removeEventListener(eventName, _utils_app_editor_eventHandle_keyEvent__WEBPACK_IMPORTED_MODULE_11__.recordRange);\n    }\n    el.removeEventListener(\"input\", _utils_app_editor_eventHandle_checkbox__WEBPACK_IMPORTED_MODULE_19__.setCheckedBoxCrossed);\n    (0,_utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.getOutlineNav)()?.removeEventListener(\"click\", _utils_app_editor_eventHandle_updateOutline__WEBPACK_IMPORTED_MODULE_17__.updateOutlineNav);\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.editor.value.destroy();\n  });\n  return {\n    node: _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_7__.node,\n    ready\n  };\n}\n/* harmony default export */ __webpack_exports__[\"default\"] = (useEditor);\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/editor.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/editor/eventHandle/atSearch.ts":
             /*!******************************************************!*\
@@ -2539,15 +2565,15 @@
         "./src/utils/app/editor/eventHandle/keyEvent.ts":
             /*!******************************************************!*\
   !*** ./src/utils/app/editor/eventHandle/keyEvent.ts ***!
   \******************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   beforeInput: function() { return /* binding */ beforeInput; },\n/* harmony export */   onKeyup: function() { return /* binding */ onKeyup; }\n/* harmony export */ });\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/editor/atTag */ \"./src/utils/app/editor/atTag.ts\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/atSearch */ \"./src/utils/app/editor/eventHandle/atSearch.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\n\nconst HTTPRegex = /(^|\\s)(https?:\\/\\/[^\\s]+)/g;\nfunction tryReplaceHttpToNodeLink() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value || !_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value) return;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__.getRange)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor);\n  if (!sel || !range) return;\n  const startContainer = range.startContainer;\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor.element.contains(startContainer)) return;\n  const text = startContainer.textContent;\n  if (text === null) return;\n  const textBeforeCursor = text.slice(0, range.startOffset);\n  const match = HTTPRegex.exec(textBeforeCursor);\n  if (!match) return;\n  const start = match.index;\n  if (start === undefined) return;\n  const url = match[2].trim();\n  const urlStart = start + match[1].length;\n  const urlEnd = urlStart + match[2].length;\n  let linkNode = null;\n  if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n    linkNode = document.createElement(\"a\");\n    linkNode.href = url;\n    linkNode.textContent = url;\n  } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n    linkNode = document.createElement(\"span\");\n    linkNode.setAttribute(\"data-type\", \"a\");\n    linkNode.className = \"vditor-ir__node\";\n    const span1 = document.createElement(\"span\");\n    span1.className = \"vditor-ir__marker vditor-ir__marker--bracket\";\n    span1.textContent = \"[\";\n    linkNode.appendChild(span1);\n    const span2 = document.createElement(\"span\");\n    span2.className = \"vditor-ir__link\";\n    span2.textContent = url;\n    linkNode.appendChild(span2);\n    const span3 = document.createElement(\"span\");\n    span3.className = \"vditor-ir__marker vditor-ir__marker--bracket\";\n    span3.textContent = \"]\";\n    linkNode.appendChild(span3);\n    const span4 = document.createElement(\"span\");\n    span4.className = \"vditor-ir__marker vditor-ir__marker--paren\";\n    span4.textContent = \"(\";\n    linkNode.appendChild(span4);\n    const span5 = document.createElement(\"span\");\n    span5.className = \"vditor-ir__marker vditor-ir__marker--link\";\n    span5.textContent = url;\n    linkNode.appendChild(span5);\n    const span6 = document.createElement(\"span\");\n    span6.className = \"vditor-ir__marker vditor-ir__marker--paren\";\n    span6.textContent = \")\";\n    linkNode.appendChild(span6);\n  } else {\n    return;\n  }\n  range.setStart(startContainer, urlStart);\n  range.setEnd(startContainer, urlEnd);\n  range.deleteContents();\n  range.insertNode(linkNode);\n  range.setStartAfter(linkNode);\n  sel.removeAllRanges();\n  sel.addRange(range);\n  sel.collapseToEnd();\n}\nasync function onKeyup(event) {\n  if (!_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value) return;\n  if ([\"ArrowLeft\", \"ArrowRight\"].includes(event.key)) {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    const {\n      isIn,\n      range,\n      anchorElement\n    } = (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInNodeLink)(vditor);\n    if (!isIn) {\n      // await tryAtSearch()\n      return;\n    }\n    if (!isIn || !range || !anchorElement || !anchorElement.textContent) return;\n    if (event.key === \"ArrowLeft\") {\n      range.setStartBefore(anchorElement);\n      range.collapse(true);\n    } else {\n      range.setEndAfter(anchorElement);\n      range.collapse(false);\n    }\n  } else if ([\"ArrowDown\", \"ArrowUp\"].includes(event.key)) {\n    (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.moveCursorOutATag)();\n  } else if (event.key === \"Backspace\") {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    let func = null;\n    if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n      func = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInNodeLink;\n    } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n      func = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInSpanLink;\n    } else {\n      return;\n    }\n    const {\n      isIn,\n      range,\n      anchorElement\n    } = func(vditor);\n    // fix vditor bug\n    if (range && _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.cursorQueryText.value === \"\" && (!range.endContainer.nextSibling || range.endContainer.nextSibling?.textContent === \"\")) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.isAtSearch.value = false;\n    }\n    if (!isIn || !range || !anchorElement || !anchorElement.textContent) return;\n    const atTextRange = document.createRange();\n    atTextRange.setStartBefore(anchorElement);\n    atTextRange.setEndAfter(anchorElement);\n    atTextRange.deleteContents();\n  } else if (event.key === \"Delete\") {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__.getRange)(vditor);\n    if (!sel || !range) return;\n    // fix vditor bug\n    if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.cursorQueryText.value === \"\" && (!range.endContainer.nextSibling || range.endContainer.nextSibling?.textContent === \"\")) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.isAtSearch.value = false;\n    }\n    const firstNode = range.endContainer.firstChild;\n    let check = null;\n    if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n      check = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isNodeAnchorEl;\n    } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n      check = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isNodeSpanEl;\n    } else {\n      return;\n    }\n    if (firstNode && check(firstNode)) {\n      event.preventDefault();\n      const atTextRange = document.createRange();\n      atTextRange.setStartBefore(firstNode);\n      atTextRange.setEndAfter(firstNode);\n      atTextRange.deleteContents();\n      return;\n    }\n    const isCursorAtEnd = range.endOffset === range.endContainer.textContent?.length;\n    if (!isCursorAtEnd) return;\n    const nextEl = range.endContainer.nextSibling;\n    if (!nextEl) return;\n    if (![\"A\", \"SPAN\"].includes(nextEl.tagName)) return;\n    if (!check(nextEl)) return;\n    event.preventDefault();\n    const atTextRange = document.createRange();\n    atTextRange.setStartBefore(nextEl);\n    atTextRange.setEndAfter(nextEl);\n    atTextRange.deleteContents();\n  }\n}\nasync function beforeInput(event) {\n  // event can be InputEvent or ClipboardEvent or CompositionEvent\n  if (event.data === \"@\") {\n    event.preventDefault();\n    if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_3__.getMQ)() === \"sm\") {\n      await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__.tryAtSearchBase)();\n      return;\n    }\n    await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__.tryAtSearchAutoLoc)();\n  } else if (event.data === \" \" || event.inputType === \"insertParagraph\") {\n    tryReplaceHttpToNodeLink();\n  }\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/eventHandle/keyEvent.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   beforeInput: function() { return /* binding */ beforeInput; },\n/* harmony export */   onKeyup: function() { return /* binding */ onKeyup; },\n/* harmony export */   recordRange: function() { return /* binding */ recordRange; }\n/* harmony export */ });\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/editor/atTag */ \"./src/utils/app/editor/atTag.ts\");\n/* harmony import */ var _utils_mq__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/mq */ \"./src/utils/mq.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/atSearch */ \"./src/utils/app/editor/eventHandle/atSearch.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\n\nconst HTTPRegex = /(^|\\s)(https?:\\/\\/[^\\s]+)/g;\nfunction tryReplaceHttpToNodeLink() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value || !_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value) return;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__.getRange)(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor);\n  if (!sel || !range) return;\n  const startContainer = range.startContainer;\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor.element.contains(startContainer)) return;\n  const text = startContainer.textContent;\n  if (text === null) return;\n  const textBeforeCursor = text.slice(0, range.startOffset);\n  const match = HTTPRegex.exec(textBeforeCursor);\n  if (!match) return;\n  const start = match.index;\n  if (start === undefined) return;\n  const url = match[2].trim();\n  const urlStart = start + match[1].length;\n  const urlEnd = urlStart + match[2].length;\n  let linkNode = null;\n  if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n    linkNode = document.createElement(\"a\");\n    linkNode.href = url;\n    linkNode.textContent = url;\n  } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n    linkNode = document.createElement(\"span\");\n    linkNode.setAttribute(\"data-type\", \"a\");\n    linkNode.className = \"vditor-ir__node\";\n    const span1 = document.createElement(\"span\");\n    span1.className = \"vditor-ir__marker vditor-ir__marker--bracket\";\n    span1.textContent = \"[\";\n    linkNode.appendChild(span1);\n    const span2 = document.createElement(\"span\");\n    span2.className = \"vditor-ir__link\";\n    span2.textContent = url;\n    linkNode.appendChild(span2);\n    const span3 = document.createElement(\"span\");\n    span3.className = \"vditor-ir__marker vditor-ir__marker--bracket\";\n    span3.textContent = \"]\";\n    linkNode.appendChild(span3);\n    const span4 = document.createElement(\"span\");\n    span4.className = \"vditor-ir__marker vditor-ir__marker--paren\";\n    span4.textContent = \"(\";\n    linkNode.appendChild(span4);\n    const span5 = document.createElement(\"span\");\n    span5.className = \"vditor-ir__marker vditor-ir__marker--link\";\n    span5.textContent = url;\n    linkNode.appendChild(span5);\n    const span6 = document.createElement(\"span\");\n    span6.className = \"vditor-ir__marker vditor-ir__marker--paren\";\n    span6.textContent = \")\";\n    linkNode.appendChild(span6);\n  } else {\n    return;\n  }\n  range.setStart(startContainer, urlStart);\n  range.setEnd(startContainer, urlEnd);\n  range.deleteContents();\n  range.insertNode(linkNode);\n  range.setStartAfter(linkNode);\n  sel.removeAllRanges();\n  sel.addRange(range);\n  sel.collapseToEnd();\n}\nasync function onKeyup(event) {\n  if (!_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value) return;\n  if ([\"ArrowLeft\", \"ArrowRight\"].includes(event.key)) {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    const {\n      isIn,\n      range,\n      anchorElement\n    } = (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInNodeLink)(vditor);\n    if (!isIn) {\n      // await tryAtSearch()\n      return;\n    }\n    if (!isIn || !range || !anchorElement || !anchorElement.textContent) return;\n    if (event.key === \"ArrowLeft\") {\n      range.setStartBefore(anchorElement);\n      range.collapse(true);\n    } else {\n      range.setEndAfter(anchorElement);\n      range.collapse(false);\n    }\n  } else if ([\"ArrowDown\", \"ArrowUp\"].includes(event.key)) {\n    (0,_utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.moveCursorOutATag)();\n  } else if (event.key === \"Backspace\") {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    let func = null;\n    if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n      func = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInNodeLink;\n    } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n      func = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isCursorInSpanLink;\n    } else {\n      return;\n    }\n    const {\n      isIn,\n      range,\n      anchorElement\n    } = func(vditor);\n    // fix vditor bug\n    if (range && _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.cursorQueryText.value === \"\" && (!range.endContainer.nextSibling || range.endContainer.nextSibling?.textContent === \"\")) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.isAtSearch.value = false;\n    }\n    if (!isIn || !range || !anchorElement || !anchorElement.textContent) return;\n    const atTextRange = document.createRange();\n    atTextRange.setStartBefore(anchorElement);\n    atTextRange.setEndAfter(anchorElement);\n    atTextRange.deleteContents();\n  } else if (event.key === \"Delete\") {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n    const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n    const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__.getRange)(vditor);\n    if (!sel || !range) return;\n    // fix vditor bug\n    if (_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.cursorQueryText.value === \"\" && (!range.endContainer.nextSibling || range.endContainer.nextSibling?.textContent === \"\")) {\n      _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.isAtSearch.value = false;\n    }\n    const firstNode = range.endContainer.firstChild;\n    let check = null;\n    if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"wysiwyg\") {\n      check = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isNodeAnchorEl;\n    } else if (_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorMode === \"ir\") {\n      check = _utils_app_editor_atTag__WEBPACK_IMPORTED_MODULE_2__.isNodeSpanEl;\n    } else {\n      return;\n    }\n    if (firstNode && check(firstNode)) {\n      event.preventDefault();\n      const atTextRange = document.createRange();\n      atTextRange.setStartBefore(firstNode);\n      atTextRange.setEndAfter(firstNode);\n      atTextRange.deleteContents();\n      return;\n    }\n    const isCursorAtEnd = range.endOffset === range.endContainer.textContent?.length;\n    if (!isCursorAtEnd) return;\n    const nextEl = range.endContainer.nextSibling;\n    if (!nextEl) return;\n    if (![\"A\", \"SPAN\"].includes(nextEl.tagName)) return;\n    if (!check(nextEl)) return;\n    event.preventDefault();\n    const atTextRange = document.createRange();\n    atTextRange.setStartBefore(nextEl);\n    atTextRange.setEndAfter(nextEl);\n    atTextRange.deleteContents();\n  }\n}\nasync function beforeInput(event) {\n  // event can be InputEvent or ClipboardEvent or CompositionEvent\n  if (event.data === \"@\") {\n    event.preventDefault();\n    if ((0,_utils_mq__WEBPACK_IMPORTED_MODULE_3__.getMQ)() === \"sm\") {\n      await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__.tryAtSearchBase)();\n      return;\n    }\n    await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_4__.tryAtSearchAutoLoc)();\n  } else if (event.data === \" \" || event.inputType === \"insertParagraph\") {\n    tryReplaceHttpToNodeLink();\n  }\n}\nfunction recordRange() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value) return;\n  const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.editor.value.vditor;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_1__.getRange)(vditor);\n  if (!sel || !range) return;\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_0__.cacheRange.value = range;\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/eventHandle/keyEvent.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/editor/eventHandle/updateOutline.ts":
             /*!***********************************************************!*\
@@ -2578,15 +2604,15 @@
         "./src/utils/app/editor/recommend.ts":
             /*!*******************************************!*\
   !*** ./src/utils/app/editor/recommend.ts ***!
   \*******************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   insertAtNode: function() { return /* binding */ insertAtNode; },\n/* harmony export */   resetRecommend: function() { return /* binding */ resetRecommend; }\n/* harmony export */ });\n/* harmony import */ var axios__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! axios */ \"./node_modules/axios/lib/axios.js\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_requestId__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/requestId */ \"./src/utils/requestId.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_msgBox__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/msgBox */ \"./src/utils/msgBox.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/atSearch */ \"./src/utils/app/editor/eventHandle/atSearch.ts\");\n\n\n\n\n\n\n\n\nlet lastTime = 0;\nasync function recommend(nid, content) {\n  const defaultRes = [];\n  const maxLen = 200;\n  // if the content is too short, do not call\n  if (content.length <= 3) return defaultRes;else if (content.length > maxLen) {\n    content = content.slice(content.length - maxLen, content.length);\n  }\n  try {\n    const resp = await axios__WEBPACK_IMPORTED_MODULE_7__[\"default\"].post(`${_utils_configs__WEBPACK_IMPORTED_MODULE_0__[\"default\"].apiUrl}/api/search/recommend`, {\n      nidExclude: [nid],\n      requestId: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_1__[\"default\"])(),\n      content: content\n    }, {\n      headers: {\n        ContentType: 'application/json',\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_2__.getToken)()\n      }\n    });\n    if (resp.data.code !== 0) {\n      (0,_utils_msgBox__WEBPACK_IMPORTED_MODULE_3__.showErrorMsgBox)(resp.data.message);\n      return defaultRes;\n    }\n    return resp.data.nodes;\n  } catch (err) {\n    console.log(err);\n  }\n  return defaultRes;\n}\nfunction getCursorParagraph() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value) return null;\n  const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value.vditor;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_5__.getRange)(vditor);\n  if (!sel || !range) return null;\n  const startContainer = range.startContainer;\n  if (!vditor.element.contains(startContainer)) return null;\n  // parent element\n  const parent = startContainer.parentElement;\n  if (!parent) return null;\n  // check if the parent is a paragraph\n  if (![\"P\", \"LI\"].includes(parent.tagName)) return null;\n  // get the parent's textContent but without a tag's textContent from the parent\n  const aTag = parent.querySelectorAll(\"a\");\n  if (aTag.length === 0) return parent.textContent;\n  let returnText = parent.textContent;\n  // is null\n  if (returnText === null) return null;\n  // remove a tag's textContent from the parent\n  for (let i = 0; i < aTag.length; i++) {\n    const aTagText = aTag[i].textContent;\n    if (aTagText === null || !aTagText.startsWith(\"@\")) continue;\n    returnText = returnText.replace(aTagText, \"\");\n  }\n  // get text from the parent\n  return returnText.trim();\n}\nasync function resetRecommend(nid) {\n  // if the time interval is less than 5 seconds, do not call\n  if (Date.now() - lastTime < 5000) return;\n  lastTime = Date.now();\n  const paragraph = getCursorParagraph();\n  if (!paragraph) return;\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.recommendNodes.value = await recommend(nid, paragraph);\n}\nasync function insertAtNode(nid, toNid, title) {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value) return;\n  const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value.vditor;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_5__.getRange)(vditor);\n  if (!range) return;\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value = range;\n  const blank = document.createTextNode(\" \");\n  range.insertNode(blank);\n  range.setStartAfter(blank);\n  await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_6__.addAtNode)(nid, toNid, title);\n  // set the cursor to the end of the inserted node\n  if (!sel) return;\n  sel.removeAllRanges();\n  sel.addRange(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value);\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/recommend.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   insertAtNode: function() { return /* binding */ insertAtNode; },\n/* harmony export */   resetRecommend: function() { return /* binding */ resetRecommend; }\n/* harmony export */ });\n/* harmony import */ var axios__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! axios */ \"./node_modules/axios/lib/axios.js\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var _utils_requestId__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/requestId */ \"./src/utils/requestId.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_msgBox__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/msgBox */ \"./src/utils/msgBox.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/editor/utils */ \"./src/utils/app/editor/utils.ts\");\n/* harmony import */ var _utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/editor/eventHandle/atSearch */ \"./src/utils/app/editor/eventHandle/atSearch.ts\");\n\n\n\n\n\n\n\n\nlet lastTime = 0;\nasync function recommend(nid, content) {\n  const defaultRes = [];\n  const maxLen = 200;\n  // if the content is too short, do not call\n  if (content.length <= 3) return defaultRes;else if (content.length > maxLen) {\n    content = content.slice(content.length - maxLen, content.length);\n  }\n  try {\n    const resp = await axios__WEBPACK_IMPORTED_MODULE_7__[\"default\"].post(`${_utils_configs__WEBPACK_IMPORTED_MODULE_0__[\"default\"].apiUrl}/api/search/recommend`, {\n      nidExclude: [nid],\n      requestId: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_1__[\"default\"])(),\n      content: content\n    }, {\n      headers: {\n        ContentType: 'application/json',\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_2__.getToken)()\n      }\n    });\n    if (resp.data.code !== 0) {\n      (0,_utils_msgBox__WEBPACK_IMPORTED_MODULE_3__.showErrorMsgBox)(resp.data.message);\n      return defaultRes;\n    }\n    return resp.data.nodes;\n  } catch (err) {\n    console.log(err);\n  }\n  return defaultRes;\n}\nfunction getCursorParagraph() {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value) return null;\n  const vditor = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value.vditor;\n  const [sel, range] = (0,_utils_app_editor_utils__WEBPACK_IMPORTED_MODULE_5__.getRange)(vditor);\n  if (!sel || !range) return null;\n  const startContainer = range.startContainer;\n  if (!vditor.element.contains(startContainer)) return null;\n  // parent element\n  const parent = startContainer.parentElement;\n  if (!parent) return null;\n  // check if the parent is a paragraph\n  if (![\"P\", \"LI\"].includes(parent.tagName)) return null;\n  // get the parent's textContent but without a tag's textContent from the parent\n  const aTag = parent.querySelectorAll(\"a\");\n  if (aTag.length === 0) return parent.textContent;\n  let returnText = parent.textContent;\n  // is null\n  if (returnText === null) return null;\n  // remove a tag's textContent from the parent\n  for (let i = 0; i < aTag.length; i++) {\n    const aTagText = aTag[i].textContent;\n    if (aTagText === null || !aTagText.startsWith(\"@\")) continue;\n    returnText = returnText.replace(aTagText, \"\");\n  }\n  // get text from the parent\n  return returnText.trim();\n}\nasync function resetRecommend(nid) {\n  // if the time interval is less than 5 seconds, do not call\n  if (Date.now() - lastTime < 5000) return;\n  lastTime = Date.now();\n  const paragraph = getCursorParagraph();\n  if (!paragraph) return;\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.recommendNodes.value = await recommend(nid, paragraph);\n}\nasync function insertAtNode(nid, toNid, title) {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.editor.value || !_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value) return;\n  const sel = window.getSelection();\n  const blank = document.createTextNode(\" \");\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value.insertNode(blank);\n  _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value.setStartAfter(blank);\n  await (0,_utils_app_editor_eventHandle_atSearch__WEBPACK_IMPORTED_MODULE_6__.addAtNode)(nid, toNid, title);\n  // set the cursor to the end of the inserted node\n  if (!sel) return;\n  sel.removeAllRanges();\n  sel.addRange(_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_4__.cacheRange.value);\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/recommend.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/editor/refs.ts":
             /*!**************************************!*\
@@ -2610,22 +2636,35 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   renderNid: function() { return /* binding */ renderNid; }\n/* harmony export */ });\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.array.push.js */ \"./node_modules/core-js/modules/es.array.push.js\");\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var _utils_app_node__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/app/node */ \"./src/utils/app/node.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n/* harmony import */ var _router__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/router */ \"./src/router/index.ts\");\n\n\n\n\nasync function renderNid(nid) {\n  if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_2__.editor.value) return \"\";\n  const node = await (0,_utils_app_node__WEBPACK_IMPORTED_MODULE_1__.getNode)(nid);\n  if (!node) {\n    return \"\";\n  }\n  const htmlString = _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_2__.editor.value.vditor.lute.Md2HTML(node.md);\n  // highlight code blocks in the html string\n  const parser = new DOMParser();\n  const he = parser.parseFromString(htmlString, \"text/html\").body;\n  Array.from(he.getElementsByTagName(\"pre\")).forEach(preTag => {\n    hljs.highlightBlock(preTag);\n  });\n  Array.from(he.getElementsByTagName(\"a\")).forEach(aTag => {\n    if (aTag.pathname.startsWith(\"/n/\")) {\n      // change the color of the node link\n      aTag.classList.add(\"node-link\");\n      aTag.addEventListener(\"click\", e => {\n        e.preventDefault();\n        e.stopPropagation();\n        _router__WEBPACK_IMPORTED_MODULE_3__[\"default\"].push({\n          name: \"node\",\n          params: {\n            id: aTag.pathname.split(\"/\")[2]\n          }\n        });\n      });\n    }\n  });\n  return he.innerHTML;\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/renderMd.ts?");
 
                 /***/
             }),
 
         /***/
+        "./src/utils/app/editor/sidebar/historyEditions.ts":
+            /*!*********************************************************!*\
+  !*** ./src/utils/app/editor/sidebar/historyEditions.ts ***!
+  \*********************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   useHistEditions: function() { return /* binding */ useHistEditions; }\n/* harmony export */ });\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _utils_configs__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/configs */ \"./src/utils/configs.ts\");\n/* harmony import */ var axios__WEBPACK_IMPORTED_MODULE_7__ = __webpack_require__(/*! axios */ \"./node_modules/axios/lib/axios.js\");\n/* harmony import */ var _utils_msgBox__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/utils/msgBox */ \"./src/utils/msgBox.ts\");\n/* harmony import */ var _utils_requestId__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/requestId */ \"./src/utils/requestId.ts\");\n/* harmony import */ var _utils_account_token__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/account/token */ \"./src/utils/account/token.ts\");\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n/* harmony import */ var _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_6__ = __webpack_require__(/*! @/utils/app/editor/refs */ \"./src/utils/app/editor/refs.ts\");\n\n\n\n\n\n\n\n\nasync function getHistEditions(nid) {\n  try {\n    const resp = await axios__WEBPACK_IMPORTED_MODULE_7__[\"default\"].post(`${_utils_configs__WEBPACK_IMPORTED_MODULE_1__[\"default\"].apiUrl}/api/node/hist`, {\n      nid: nid,\n      requestId: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_3__[\"default\"])()\n    }, {\n      headers: {\n        ContentType: 'application/json',\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_4__.getToken)()\n      }\n    });\n    if (resp.data.code !== 0) {\n      console.log(resp.data.message);\n      return [];\n    }\n    return resp.data.versions;\n  } catch (err) {\n    console.log(err);\n  }\n  return [];\n}\nasync function getHistEditionMd(nid, version) {\n  try {\n    const resp = await axios__WEBPACK_IMPORTED_MODULE_7__[\"default\"].post(`${_utils_configs__WEBPACK_IMPORTED_MODULE_1__[\"default\"].apiUrl}/api/node/hist/md`, {\n      nid: nid,\n      version: version,\n      requestId: (0,_utils_requestId__WEBPACK_IMPORTED_MODULE_3__[\"default\"])()\n    }, {\n      headers: {\n        ContentType: 'application/json',\n        token: (0,_utils_account_token__WEBPACK_IMPORTED_MODULE_4__.getToken)()\n      }\n    });\n    if (resp.data.code !== 0) {\n      console.log(resp.data.message);\n      return \"\";\n    }\n    return resp.data.md;\n  } catch (err) {\n    console.log(err);\n  }\n  return \"\";\n}\nfunction useHistEditions(nid) {\n  const versions = (0,vue__WEBPACK_IMPORTED_MODULE_0__.ref)([]);\n  (0,vue__WEBPACK_IMPORTED_MODULE_0__.onMounted)(async () => {\n    versions.value = await getHistEditions(nid);\n  });\n  async function onClickRestore(version) {\n    if (!_utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_6__.editor.value) return;\n    const confirmRestore = await (0,_utils_msgBox__WEBPACK_IMPORTED_MODULE_2__.showConfirmMsgBox)(_utils_multiLang__WEBPACK_IMPORTED_MODULE_5__[\"default\"].get(\"editorHistMdRestoreConfirm\"));\n    if (!confirmRestore) return;\n    const md = await getHistEditionMd(nid, version);\n    _utils_app_editor_refs__WEBPACK_IMPORTED_MODULE_6__.editor.value.setValue(md);\n  }\n  return {\n    versions,\n    onClickRestore\n  };\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/sidebar/historyEditions.ts?");
+
+                /***/
+            }),
+
+        /***/
         "./src/utils/app/editor/sidebar/index.ts":
             /*!***********************************************!*\
   !*** ./src/utils/app/editor/sidebar/index.ts ***!
   \***********************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   sideActivatedItem: function() { return /* binding */ sideActivatedItem; },\n/* harmony export */   useSidebar: function() { return /* binding */ useSidebar; },\n/* harmony export */   useSidebarItemView: function() { return /* binding */ useSidebarItemView; }\n/* harmony export */ });\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.array.push.js */ \"./node_modules/core-js/modules/es.array.push.js\");\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _assets_images_icons_node_svg__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/assets/images/icons/node.svg */ \"./src/assets/images/icons/node.svg\");\n/* harmony import */ var _utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/utils/app/plugin/request */ \"./src/utils/app/plugin/request.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\nconst sideActivatedItem = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)(\"linkedNodes\");\nconst sideIframe = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)(null);\nasync function refreshPlugin() {\n  if (sideActivatedItem.value === \"linkedNodes\" || sideActivatedItem.value === null || !sideIframe.value) return;\n  const html = await (0,_utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_3__.renderPluginEditorSide)(sideActivatedItem.value);\n  const iframeWindow = sideIframe.value.contentWindow;\n  if (!iframeWindow) return;\n  iframeWindow.document.open();\n  iframeWindow.document.write(html);\n  iframeWindow.document.close();\n}\nfunction useSidebar() {\n  const plugins = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)([{\n    id: \"linkedNodes\",\n    name: \"linkedNodes\",\n    description: \"linkedNodes\",\n    author: \"morvanzhou\",\n    version: \"1.0.0\",\n    iconSrc: _assets_images_icons_node_svg__WEBPACK_IMPORTED_MODULE_2__\n  }]);\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onMounted)(async () => {\n    if (!_utils_app_user__WEBPACK_IMPORTED_MODULE_4__.user.value) return;\n    sideActivatedItem.value = _utils_app_user__WEBPACK_IMPORTED_MODULE_4__.user.value.settings.editorSideCurrentToolId;\n    if (sideActivatedItem.value === \"\") {\n      sideActivatedItem.value = null;\n    }\n    plugins.value.push(...(await (0,_utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_3__.getPluginsWithRenderEditorSide)()));\n    await refreshPlugin();\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onUnmounted)(() => {\n    plugins.value = [plugins.value[0]];\n  });\n  return {\n    sideActivatedItem,\n    plugins,\n    refreshPlugin\n  };\n}\nfunction useSidebarItemView() {\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onMounted)(async () => {\n    await refreshPlugin();\n  });\n  return {\n    sideActivatedItem,\n    sideIframe\n  };\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/sidebar/index.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   sideActivatedItem: function() { return /* binding */ sideActivatedItem; },\n/* harmony export */   useSidebar: function() { return /* binding */ useSidebar; },\n/* harmony export */   useSidebarItemView: function() { return /* binding */ useSidebarItemView; }\n/* harmony export */ });\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! core-js/modules/es.array.push.js */ \"./node_modules/core-js/modules/es.array.push.js\");\n/* harmony import */ var core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0___default = /*#__PURE__*/__webpack_require__.n(core_js_modules_es_array_push_js__WEBPACK_IMPORTED_MODULE_0__);\n/* harmony import */ var vue__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! vue */ \"./node_modules/vue/dist/vue.runtime.esm-bundler.js\");\n/* harmony import */ var _assets_images_icons_node_svg__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! @/assets/images/icons/node.svg */ \"./src/assets/images/icons/node.svg\");\n/* harmony import */ var _assets_images_icons_restore_svg__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! @/assets/images/icons/restore.svg */ \"./src/assets/images/icons/restore.svg\");\n/* harmony import */ var _utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_4__ = __webpack_require__(/*! @/utils/app/plugin/request */ \"./src/utils/app/plugin/request.ts\");\n/* harmony import */ var _utils_app_user__WEBPACK_IMPORTED_MODULE_5__ = __webpack_require__(/*! @/utils/app/user */ \"./src/utils/app/user.ts\");\n\n\n\n\n\n\nconst sideActivatedItem = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)(\"linkedNodes\");\nconst sideIframe = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)(null);\nconst fixedPluginIds = [];\nasync function refreshPlugin() {\n  if (sideActivatedItem.value === null || fixedPluginIds.includes(sideActivatedItem.value) || !sideIframe.value) return;\n  const html = await (0,_utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_4__.renderPluginEditorSide)(sideActivatedItem.value);\n  const iframeWindow = sideIframe.value.contentWindow;\n  if (!iframeWindow) return;\n  iframeWindow.document.open();\n  iframeWindow.document.write(html);\n  iframeWindow.document.close();\n}\nfunction useSidebar() {\n  const plugins = (0,vue__WEBPACK_IMPORTED_MODULE_1__.ref)([{\n    id: \"linkedNodes\",\n    name: \"Linked Nodes\",\n    description: \"linkedNodes\",\n    author: \"morvanzhou\",\n    version: \"1.0.0\",\n    iconSrc: _assets_images_icons_node_svg__WEBPACK_IMPORTED_MODULE_2__\n  }, {\n    id: \"histRestore\",\n    name: \"Versions\",\n    description: \"versions\",\n    author: \"morvanzhou\",\n    version: \"1.0.0\",\n    iconSrc: _assets_images_icons_restore_svg__WEBPACK_IMPORTED_MODULE_3__\n  }]);\n  fixedPluginIds.push(...plugins.value.map(plugin => plugin.id));\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onMounted)(async () => {\n    if (!_utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value) return;\n    sideActivatedItem.value = _utils_app_user__WEBPACK_IMPORTED_MODULE_5__.user.value.settings.editorSideCurrentToolId;\n    if (sideActivatedItem.value === \"\") {\n      sideActivatedItem.value = null;\n    }\n    plugins.value.push(...(await (0,_utils_app_plugin_request__WEBPACK_IMPORTED_MODULE_4__.getPluginsWithRenderEditorSide)()));\n    await refreshPlugin();\n  });\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onUnmounted)(() => {\n    plugins.value = [plugins.value[0]];\n  });\n  return {\n    sideActivatedItem,\n    plugins,\n    refreshPlugin\n  };\n}\nfunction useSidebarItemView() {\n  (0,vue__WEBPACK_IMPORTED_MODULE_1__.onMounted)(async () => {\n    await refreshPlugin();\n  });\n  return {\n    sideActivatedItem,\n    sideIframe\n  };\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/editor/sidebar/index.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/editor/sidebar/linkedNodes.ts":
             /*!*****************************************************!*\
@@ -2773,15 +2812,15 @@
         "./src/utils/app/textOps.ts":
             /*!**********************************!*\
   !*** ./src/utils/app/textOps.ts ***!
   \**********************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   clipText: function() { return /* binding */ clipText; },\n/* harmony export */   fileSizeStr: function() { return /* binding */ fileSizeStr; },\n/* harmony export */   getBodyFromMd: function() { return /* binding */ getBodyFromMd; },\n/* harmony export */   replace1EnterTo2: function() { return /* binding */ replace1EnterTo2; },\n/* harmony export */   stripMdTitle: function() { return /* binding */ stripMdTitle; },\n/* harmony export */   utc2local: function() { return /* binding */ utc2local; }\n/* harmony export */ });\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n\nfunction clipText(text, n) {\n  text = text.trim();\n  if (text.length > n) {\n    text = text.slice(0, n) + \"...\";\n  }\n  return text;\n}\nfunction stripMdTitle(text, n = 20) {\n  if (text.startsWith(\"#\")) {\n    text = text.slice(1);\n    return stripMdTitle(text, n);\n  }\n  text = clipText(text, n);\n  if (text.length === 0) {\n    text = _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"emptyNodeTitle\");\n  }\n  return text;\n}\nconst utc2local = utcDateStr => {\n  // var utcDate = \"2022-03-19T20:15:50.000Z\";\n  const utcDate = new Date(utcDateStr);\n  const now = new Date();\n  // just now, less than 5 minutes\n  if (now.getTime() - utcDate.getTime() < 10 * 1000 * 60) {\n    return _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeJustNow\");\n  }\n  const year = utcDate.getFullYear();\n  const month = `0${utcDate.getMonth() + 1}`.slice(-2);\n  const day = `0${utcDate.getDate()}`.slice(-2);\n  const hour = `0${utcDate.getHours()}`.slice(-2);\n  const minute = `0${utcDate.getMinutes()}`.slice(-2);\n  const today = new Date(now.getFullYear(), now.getMonth(), now.getDate());\n  const dayDelta = (today.getTime() - utcDate.getTime()) / 1000 / 60 / 60 / 24;\n  if (dayDelta >= 365) {\n    // >= 1 year\n    return `${year}-${month}-${day}`;\n  } else if (dayDelta >= 1) {\n    // >= 2 days\n    return `${month}-${day}`;\n  } else if (dayDelta >= 0) {\n    // yesterday\n    return `${_utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeYesterdayPrefix\")} ${hour}:${minute}`;\n  } else {\n    // today\n    return `${_utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeTodayPrefix\")} ${hour}:${minute}`;\n  }\n};\nfunction getBodyFromMd(md) {\n  // split by the first \\n\n  const index = md.indexOf(\"\\n\");\n  if (index === -1) {\n    return \"\";\n  }\n  return md.slice(index + 1);\n}\nfunction replace1EnterTo2(text) {\n  // replace every single enter to double enters\n  // skip if there are more than 1 enters\n  return text.replace(/([^\\n])(\\n)([^\\n])/g, \"$1$2\\n$3\");\n}\nfunction fileSizeStr(size) {\n  if (size < 1024) {\n    return `${size} B`;\n  } else if (size < 1024 * 1024) {\n    return `${Math.floor(size / 1024)} KB`;\n  } else if (size < 1024 * 1024 * 1024) {\n    const mb = size / 1024 / 1024;\n    if (mb % 1 !== 0) {\n      return `${mb.toFixed(1)} MB`;\n    }\n    return `${mb} MB`;\n  } else {\n    const gb = size / 1024 / 1024 / 1024;\n    if (gb % 1 !== 0) {\n      return `${gb.toFixed(1)} GB`;\n    }\n    return `${gb} GB`;\n  }\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/textOps.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   clipText: function() { return /* binding */ clipText; },\n/* harmony export */   fileSizeStr: function() { return /* binding */ fileSizeStr; },\n/* harmony export */   getBodyFromMd: function() { return /* binding */ getBodyFromMd; },\n/* harmony export */   replace1EnterTo2: function() { return /* binding */ replace1EnterTo2; },\n/* harmony export */   stripMdTitle: function() { return /* binding */ stripMdTitle; },\n/* harmony export */   utc2localApproximate: function() { return /* binding */ utc2localApproximate; },\n/* harmony export */   utc2localFull: function() { return /* binding */ utc2localFull; }\n/* harmony export */ });\n/* harmony import */ var _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! @/utils/multiLang */ \"./src/utils/multiLang.ts\");\n\nfunction clipText(text, n) {\n  text = text.trim();\n  if (text.length > n) {\n    text = text.slice(0, n) + \"...\";\n  }\n  return text;\n}\nfunction stripMdTitle(text, n = 20) {\n  if (text.startsWith(\"#\")) {\n    text = text.slice(1);\n    return stripMdTitle(text, n);\n  }\n  text = clipText(text, n);\n  if (text.length === 0) {\n    text = _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"emptyNodeTitle\");\n  }\n  return text;\n}\nconst utc2localApproximate = utcDateStr => {\n  const [[year, month, day, hour, minute], utcDate] = getTime(utcDateStr);\n  const now = new Date();\n  // just now, less than 10 minutes\n  if (now.getTime() - utcDate.getTime() < 10 * 1000 * 60) {\n    return _utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeJustNow\");\n  }\n  const today = new Date(now.getFullYear(), now.getMonth(), now.getDate());\n  const dayDelta = (today.getTime() - utcDate.getTime()) / 1000 / 60 / 60 / 24;\n  if (dayDelta >= 365) {\n    // >= 1 year\n    return `${year}-${month}-${day}`;\n  } else if (dayDelta >= 1) {\n    // >= 2 days\n    return `${month}-${day}`;\n  } else if (dayDelta >= 0) {\n    // yesterday\n    return `${_utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeYesterdayPrefix\")} ${hour}:${minute}`;\n  } else {\n    // today\n    return `${_utils_multiLang__WEBPACK_IMPORTED_MODULE_0__[\"default\"].get(\"nodeTimeTodayPrefix\")} ${hour}:${minute}`;\n  }\n};\nfunction utc2localFull(utcDateStr) {\n  const [[year, month, day, hour, minute], _] = getTime(utcDateStr);\n  return `${year}-${month}-${day} ${hour}:${minute}`;\n}\nfunction getTime(utcDateStr) {\n  // var utcDate = \"2022-03-19T20:15:50.000Z\";\n  const utcDate = new Date(utcDateStr);\n  const year = utcDate.getFullYear().toString();\n  const month = `0${utcDate.getMonth() + 1}`.slice(-2);\n  const day = `0${utcDate.getDate()}`.slice(-2);\n  const hour = `0${utcDate.getHours()}`.slice(-2);\n  const minute = `0${utcDate.getMinutes()}`.slice(-2);\n  return [[year, month, day, hour, minute], utcDate];\n}\nfunction getBodyFromMd(md) {\n  // split by the first \\n\n  const index = md.indexOf(\"\\n\");\n  if (index === -1) {\n    return \"\";\n  }\n  return md.slice(index + 1);\n}\nfunction replace1EnterTo2(text) {\n  // replace every single enter to double enters\n  // skip if there are more than 1 enters\n  return text.replace(/([^\\n])(\\n)([^\\n])/g, \"$1$2\\n$3\");\n}\nfunction fileSizeStr(size) {\n  if (size < 1024) {\n    return `${size} B`;\n  } else if (size < 1024 * 1024) {\n    return `${Math.floor(size / 1024)} KB`;\n  } else if (size < 1024 * 1024 * 1024) {\n    const mb = size / 1024 / 1024;\n    if (mb % 1 !== 0) {\n      return `${mb.toFixed(1)} MB`;\n    }\n    return `${mb} MB`;\n  } else {\n    const gb = size / 1024 / 1024 / 1024;\n    if (gb % 1 !== 0) {\n      return `${gb.toFixed(1)} GB`;\n    }\n    return `${gb} GB`;\n  }\n}\n\n\n//# sourceURL=webpack://rethink/./src/utils/app/textOps.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/app/user.ts":
             /*!*******************************!*\
@@ -2890,15 +2929,15 @@
         "./src/utils/multiLang.ts":
             /*!********************************!*\
   !*** ./src/utils/multiLang.ts ***!
   \********************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
-                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! ./node_modules/@babel/runtime/helpers/esm/defineProperty.js */ \"./node_modules/@babel/runtime/helpers/esm/defineProperty.js\");\n/* harmony import */ var _utils_msgBox__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/msgBox */ \"./src/utils/msgBox.ts\");\n\n\nclass MultiLang {\n  constructor(data) {\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"langData\", void 0);\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"availableLangCodes\", [\"zh\", \"en\"]);\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"langCodeMap\", {\n      zh: \"中文\",\n      en: \"English\"\n    });\n    this.langData = data;\n  }\n  get(key) {\n    const l = this.langData[key];\n    if (!l) {\n      (0,_utils_msgBox__WEBPACK_IMPORTED_MODULE_1__.showErrorMsgBox)(`Lang key ${key} not found`);\n      return \"\";\n    }\n    return this.getGlobalLang() === \"zh\" ? l.zh : l.en;\n  }\n  setGlobalLang(lang) {\n    localStorage.setItem(\"rethinkLang\", lang);\n  }\n  getGlobalLang() {\n    return localStorage.getItem(\"rethinkLang\") || \"en\";\n  }\n}\nconst mLang = new MultiLang({\n  navbarHome: {\n    zh: \"首页\",\n    en: \"Home\"\n  },\n  navbarAbout: {\n    zh: \"关于\",\n    en: \"About\"\n  },\n  navbarLogin: {\n    zh: \"登录\",\n    en: \"Login\"\n  },\n  navbarStart: {\n    zh: \"开始\",\n    en: \"Start\"\n  },\n  goBackIcon: {\n    zh: \"返回\",\n    en: \"Back\"\n  },\n  sideBarHome: {\n    zh: \"首页\",\n    en: \"Home\"\n  },\n  importDataH1: {\n    zh: \"导入数据\",\n    en: \"Import Data\"\n  },\n  sideBarTrash: {\n    zh: \"回收站\",\n    en: \"Trash\"\n  },\n  sideBarImport: {\n    zh: \"导入数据\",\n    en: \"Import Data\"\n  },\n  sideBarPlugins: {\n    zh: \"插件\",\n    en: \"Plugins\"\n  },\n  arrangeNodeList: {\n    zh: \"列表\",\n    en: \"List\"\n  },\n  arrangeNodeGrid: {\n    zh: \"网格\",\n    en: \"Grid\"\n  },\n  sortNodeByTime: {\n    zh: \"时间\",\n    en: \"Time\"\n  },\n  sortNodeByCreatedAt: {\n    zh: \"最新\",\n    en: \"Create\"\n  },\n  sortNodeByModifiedAt: {\n    zh: \"最后修改\",\n    en: \"Update\"\n  },\n  sortNodeByTitle: {\n    zh: \"名称\",\n    en: \"Title\"\n  },\n  node2Trash: {\n    zh: \"移至回收桶\",\n    en: \"Move To Trash\"\n  },\n  nodeDelete: {\n    zh: \"删除\",\n    en: \"Delete\"\n  },\n  nodeDeleteConfirmation: {\n    zh: \"确认删除\",\n    en: \"Delete this thought\"\n  },\n  nodeRestoreFromTrash: {\n    zh: \"恢复\",\n    en: \"Restore\"\n  },\n  searchBarPlaceholder: {\n    zh: \"搜想法...\",\n    en: \"Search...\"\n  },\n  searchWindowSMSubmit: {\n    zh: \"搜索\",\n    en: \"Search\"\n  },\n  searchWindowSMCollapse: {\n    zh: \"收起\",\n    en: \"Collapse\"\n  },\n  noSearchResult: {\n    zh: \"没有搜索结果\",\n    en: \"No search result\"\n  },\n  search: {\n    zh: \"搜索\",\n    en: \"Search\"\n  },\n  headerBarNewThink: {\n    zh: \"新想法\",\n    en: \"New Thought\"\n  },\n  nodeTimeJustNow: {\n    zh: \"刚刚\",\n    en: \"Just now\"\n  },\n  nodeTimeYesterdayPrefix: {\n    zh: \"昨天\",\n    en: \"Yesterday\"\n  },\n  nodeTimeTodayPrefix: {\n    zh: \"今天\",\n    en: \"Today\"\n  },\n  nodeViewHeaderTitle: {\n    zh: \"标题\",\n    en: \"Title\"\n  },\n  nodeViewHeaderSnippet: {\n    zh: \"内容\",\n    en: \"Content\"\n  },\n  nodeViewHeaderTime: {\n    zh: \"时间\",\n    en: \"Time\"\n  },\n  sortNodeBySimilarity: {\n    zh: \"相似度\",\n    en: \"Similarity\"\n  },\n  cursorSearchDropdownSearchResult: {\n    zh: \"Rethink\",\n    en: \"Rethink\"\n  },\n  cursorSearchDropdownSearchRecent: {\n    zh: \"最近链接的想法\",\n    en: \"Recent linked thoughts\"\n  },\n  cursorSearchDropdownCreateNew: {\n    zh: \"新建\",\n    en: \"Create new\"\n  },\n  cursorSearchDropdownTitle: {\n    zh: \"选择连接的想法\",\n    en: \"Select a thought to link\"\n  },\n  emptyNodeTitle: {\n    zh: \"无标题\",\n    en: \"Untitled\"\n  },\n  settingsViewHeading: {\n    zh: \"设置\",\n    en: \"Settings\"\n  },\n  settingsViewGlobal: {\n    zh: \"全局设置\",\n    en: \"Global Settings\"\n  },\n  settingsLanguage: {\n    zh: \"语言\",\n    en: \"Language\"\n  },\n  settingsTheme: {\n    zh: \"主题\",\n    en: \"Theme\"\n  },\n  settingsViewEditor: {\n    zh: \"编辑器\",\n    en: \"Editor\"\n  },\n  settingsEditorMode: {\n    zh: \"模式\",\n    en: \"Mode\"\n  },\n  settingsEditorFontSize: {\n    zh: \"字体大小\",\n    en: \"Font Size\"\n  },\n  settingsEditorCodeTheme: {\n    zh: \"代码主题\",\n    en: \"Code Theme\"\n  },\n  settingsChangePwd: {\n    zh: \"修改密码\",\n    en: \"Change Password\"\n  },\n  settingsOldPwd: {\n    zh: \"旧密码\",\n    en: \"Old Password\"\n  },\n  settingsNewPwd: {\n    zh: \"新密码\",\n    en: \"New Password\"\n  },\n  settingsNewPwdConfirm: {\n    zh: \"确认新密码\",\n    en: \"Confirm New Password\"\n  },\n  settingsUpdatePwd: {\n    zh: \"更新密码\",\n    en: \"Update Password\"\n  },\n  settingsPwdNotMatch: {\n    zh: \"新密码与确认新密码不一致\",\n    en: \"New Password not match\"\n  },\n  settingsChangePwdHint: {\n    zh: \"修改密码\",\n    en: \"Change Password\"\n  },\n  settingsPwdUpdated: {\n    zh: \"密码已更新，请重新登陆\",\n    en: \"Password updated, please login again\"\n  },\n  settingsPwdSameAsOld: {\n    zh: \"新密码与旧密码相同\",\n    en: \"New password is the same as the old one\"\n  },\n  settingsIForgetMyPwd: {\n    zh: \"我忘记了我的密码\",\n    en: \"I forgot my password\"\n  },\n  userViewProfilePage: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  userProfileMeta: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  userViewName: {\n    zh: \"名字\",\n    en: \"Name\"\n  },\n  userViewEmail: {\n    zh: \"邮箱\",\n    en: \"Email\"\n  },\n  userViewAvatar: {\n    zh: \"头像\",\n    en: \"Picture\"\n  },\n  userProfileStats: {\n    zh: \"统计\",\n    en: \"Stats\"\n  },\n  userViewStorageUsage: {\n    zh: \"已使用:\",\n    en: \"Used Space:\"\n  },\n  loginViewHeading: {\n    zh: \"登录\",\n    en: \"Login\"\n  },\n  loginViewHeadingSignup: {\n    zh: \"新用户注册\",\n    en: \"New User Register\"\n  },\n  loginViewAccountLabel: {\n    zh: \"账号\",\n    en: \"Account\"\n  },\n  loginViewAccountPlaceholder: {\n    zh: \"邮箱\",\n    en: \"email\"\n  },\n  loginViewAccountInputTitle: {\n    zh: \"请输入正确的邮箱\",\n    en: \"Please input a valid email\"\n  },\n  loginViewPasswordLabel: {\n    zh: \"密码\",\n    en: \"Password\"\n  },\n  loginViewNoUserOrPassword: {\n    zh: \"账号或密码错误\",\n    en: \"Account or password error\"\n  },\n  loginViewAccountPasswordEmpty: {\n    zh: \"账号或密码不能为空\",\n    en: \"Account or password can not be empty\"\n  },\n  loginViewPasswordInputTitle: {\n    zh: \"必须包含至少 1 位数字和 1 位字母，且至少 6 个字符以上，最多 20 字符以下\",\n    en: \"Must contain at least one number and one letter, and at least 6 and less than 20 characters\"\n  },\n  loginViewConfirmPasswordLabel: {\n    zh: \"确认密码\",\n    en: \"Confirm password\"\n  },\n  loginViewConfirmPasswordNotMatch: {\n    zh: \"两次密码不一致\",\n    en: \"Confirm password not match\"\n  },\n  loginViewLoginButton: {\n    zh: \"登录\",\n    en: \"Log In\"\n  },\n  loginViewSignupButton: {\n    zh: \"注册\",\n    en: \"Create new account\"\n  },\n  loginViewSignupHasAccount: {\n    zh: \"已有账号？\",\n    en: \"Already have an account?\"\n  },\n  loginViewForgetPassword: {\n    zh: \"忘记密码\",\n    en: \"Forget password\"\n  },\n  loginViewWrongPasswordLength: {\n    zh: \"密码长度不正确，密码应在 6-20 字符之间\",\n    en: \"Password length is not correct, should be 6-20 characters\"\n  },\n  loginViewOAuthLogin: {\n    zh: \"其他方式登录\",\n    en: \"Other Login\"\n  },\n  notValidEmail: {\n    zh: \"邮箱格式不正确\",\n    en: \"Email format is not correct\"\n  },\n  registerCaptchaLabel: {\n    zh: \"验证码\",\n    en: \"Verification code\"\n  },\n  loginViewCaptchaEmpty: {\n    zh: \"验证码不能为空\",\n    en: \"Verification code can not be empty\"\n  },\n  forgetPasswordH1: {\n    zh: \"忘记密码\",\n    en: \"Forget password\"\n  },\n  forgetPasswordNewLabel: {\n    zh: \"新密码\",\n    en: \"New password\"\n  },\n  sendVerificationCode: {\n    zh: \"发送验证码\",\n    en: \"Send verification code\"\n  },\n  noCaptcha: {\n    zh: \"请先完成验证码\",\n    en: \"Please complete the verification code first\"\n  },\n  \"6digitalCode\": {\n    zh: \"6位数字验证码\",\n    en: \"6 digital code\"\n  },\n  resendVerificationCode: {\n    zh: \"重新发送验证码\",\n    en: \"Resend code\"\n  },\n  verificationCodeLabel: {\n    zh: \"验证码\",\n    en: \"Verification code\"\n  },\n  resetPasswordFailed: {\n    zh: \"重置密码失败\",\n    en: \"Reset password failed\"\n  },\n  headerMenuLogout: {\n    zh: \"登出\",\n    en: \"Logout\"\n  },\n  headerMenuProfile: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  headerMenuSettings: {\n    zh: \"设置\",\n    en: \"Settings\"\n  },\n  oauthPageHeading: {\n    zh: \"账号正在验证中...\",\n    en: \"Verifying your account...\"\n  },\n  msgBoxConfirmButton: {\n    zh: \"确定\",\n    en: \"OK\"\n  },\n  msgBoxCancelButton: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  modificationSuccessful: {\n    zh: \"修改成功\",\n    en: \"Modification successful\"\n  },\n  cancel: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  submit: {\n    zh: \"提交\",\n    en: \"Submit\"\n  },\n  next: {\n    zh: \"下一步\",\n    en: \"Next\"\n  },\n  recentSearchedTitle: {\n    zh: \"最近搜索\",\n    en: \"Recent Queries\"\n  },\n  editorContentPlaceholder: {\n    zh: \"记录我的新想法...\",\n    en: \"Record my new thought...\"\n  },\n  editorSyncStatusSaved: {\n    zh: \"已自动保存\",\n    en: \"Auto saved\"\n  },\n  editorSyncStatusLastSaved: {\n    zh: \"最近保存 \",\n    en: \"Last saved \"\n  },\n  quickPostPanelPlaceholder: {\n    zh: \"速记想法 / 链接 ...\",\n    en: \"Quick thought / link ...\"\n  },\n  quickPostBtn: {\n    zh: \"记下\",\n    en: \"Send\"\n  },\n  quickPostTooLong: {\n    zh: \"用编辑器记长想法 >\",\n    en: \"Use editor for long thought >\"\n  },\n  quickPostEditInNodePage: {\n    zh: \"在新页面编辑\",\n    en: \"Edit in new page\"\n  },\n  quickPostBtnTitle: {\n    zh: \"快速记录\",\n    en: \"Quick post\"\n  },\n  tryRestoreFromTrash: {\n    zh: \"此想法被放在回收站中，是否要从回收站恢复？\",\n    en: \"This thought is in trash, do you want to restore it?\"\n  },\n  nodeIsDeleted: {\n    zh: \"此想法已被您删除\",\n    en: \"This thought is deleted\"\n  },\n  noLinkedNode: {\n    zh: \"还没有链接到任何想法，尝试 @ 一些吧\",\n    en: \"No linked thought yet, try @ some\"\n  },\n  batchFileOpsShare: {\n    zh: \"分享\",\n    en: \"Share\"\n  },\n  batchFileOpsDelete: {\n    zh: \"删除\",\n    en: \"Delete\"\n  },\n  batchFileOpsTrash: {\n    zh: \"回收\",\n    en: \"To Trash\"\n  },\n  batchFileOpsCancel: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  batchFileOpsDownload: {\n    zh: \"下载\",\n    en: \"Download\"\n  },\n  batchFileOpsRestore: {\n    zh: \"恢复\",\n    en: \"Restore\"\n  },\n  batchDeleteConfirmPre: {\n    zh: \"确认删除\",\n    en: \"Confirm to delete\"\n  },\n  batchDeleteConfirmPost: {\n    zh: \"个想法？\",\n    en: \"thoughts?\"\n  },\n  nodeNeedRestoreToView: {\n    zh: \"需要恢复后才能查看，确认恢复并查看？\",\n    en: \"Need restore to be viewed, confirm restore?\"\n  },\n  uploadFilesLabel: {\n    zh: \"上传文件\",\n    en: \"Upload files\"\n  },\n  uploadFilesEmptyTask: {\n    zh: \"无任务\",\n    en: \"No Task\"\n  },\n  fileDropIsDragging: {\n    zh: \"放入文件\",\n    en: \"Release to drop files here.\"\n  },\n  fileDropNotDraggingPre: {\n    zh: \"拖拽文件到此处或\",\n    en: \"Drag and drop files here, or \"\n  },\n  fileDropNotDraggingClick: {\n    zh: \"点此\",\n    en: \"click here\"\n  },\n  fileDropNotDraggingPost: {\n    zh: \" 上传\",\n    en: \" to upload\"\n  },\n  fileDropInvalidFile: {\n    zh: \"文件格式错误\",\n    en: \"Invalid file format\"\n  },\n  fileDropTooLarge: {\n    zh: \"文件过大\",\n    en: \"File too large\"\n  },\n  fileDropTooManyPre: {\n    zh: \"文件个数超过上限: \",\n    en: \"File count exceeds limit: \"\n  },\n  fileDropTooManyPost: {\n    zh: \"，请分批上传\",\n    en: \", please upload in batches\"\n  },\n  filesSubmitBtn: {\n    zh: \"上传\",\n    en: \"Upload\"\n  },\n  fileDropPreviewFileCount: {\n    zh: \"已加载文件数：\",\n    en: \"Loaded file count: \"\n  },\n  uploadFilesTaskNotFinished: {\n    zh: \"任务未完成: \",\n    en: \"Task not finished: \"\n  },\n  newJobProgress: {\n    zh: \"最新任务进度\",\n    en: \"The latest job progress\"\n  },\n  autoRecommendation: {\n    zh: \"自动展示相关想法...\",\n    en: \"Auto show related thoughts...\"\n  },\n  editorExternalLinkConfirm: {\n    zh: \"点击确定将会去往外部链接：\",\n    en: \"Click OK to go to external link: \"\n  },\n  pluginPanelDescription: {\n    zh: \"插件是一种括展能力，可以基于你的想法库，延伸不同的功能。当前仅可以在私有化部署的版本中，开发、体验自己的插件。\",\n    en: \"Plugin is an extension capability, which can extend different functions based on your own data. \" + \"Currently, you can only develop and view your own plugins in the self-hosted version.\"\n  },\n  pluginPageTitle: {\n    zh: \"插件页\",\n    en: \"Plugin page\"\n  }\n});\n/* harmony default export */ __webpack_exports__[\"default\"] = (mLang);\n\n//# sourceURL=webpack://rethink/./src/utils/multiLang.ts?");
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! ./node_modules/@babel/runtime/helpers/esm/defineProperty.js */ \"./node_modules/@babel/runtime/helpers/esm/defineProperty.js\");\n/* harmony import */ var _utils_msgBox__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! @/utils/msgBox */ \"./src/utils/msgBox.ts\");\n\n\nclass MultiLang {\n  constructor(data) {\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"langData\", void 0);\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"availableLangCodes\", [\"zh\", \"en\"]);\n    (0,_Users_morvanzhou_Documents_repo_rethink_frontend_node_modules_babel_runtime_helpers_esm_defineProperty_js__WEBPACK_IMPORTED_MODULE_0__[\"default\"])(this, \"langCodeMap\", {\n      zh: \"中文\",\n      en: \"English\"\n    });\n    this.langData = data;\n  }\n  get(key) {\n    const l = this.langData[key];\n    if (!l) {\n      (0,_utils_msgBox__WEBPACK_IMPORTED_MODULE_1__.showErrorMsgBox)(`Lang key ${key} not found`);\n      return \"\";\n    }\n    return this.getGlobalLang() === \"zh\" ? l.zh : l.en;\n  }\n  setGlobalLang(lang) {\n    localStorage.setItem(\"rethinkLang\", lang);\n  }\n  getGlobalLang() {\n    return localStorage.getItem(\"rethinkLang\") || \"en\";\n  }\n}\nconst mLang = new MultiLang({\n  navbarHome: {\n    zh: \"首页\",\n    en: \"Home\"\n  },\n  navbarAbout: {\n    zh: \"关于\",\n    en: \"About\"\n  },\n  navbarLogin: {\n    zh: \"登录\",\n    en: \"Login\"\n  },\n  navbarStart: {\n    zh: \"开始\",\n    en: \"Start\"\n  },\n  goBackIcon: {\n    zh: \"返回\",\n    en: \"Back\"\n  },\n  sideBarHome: {\n    zh: \"首页\",\n    en: \"Home\"\n  },\n  importDataH1: {\n    zh: \"导入数据\",\n    en: \"Import Data\"\n  },\n  sideBarTrash: {\n    zh: \"回收站\",\n    en: \"Trash\"\n  },\n  sideBarImport: {\n    zh: \"导入数据\",\n    en: \"Import Data\"\n  },\n  sideBarPlugins: {\n    zh: \"插件\",\n    en: \"Plugins\"\n  },\n  arrangeNodeList: {\n    zh: \"列表\",\n    en: \"List\"\n  },\n  arrangeNodeGrid: {\n    zh: \"网格\",\n    en: \"Grid\"\n  },\n  sortNodeByTime: {\n    zh: \"时间\",\n    en: \"Time\"\n  },\n  sortNodeByCreatedAt: {\n    zh: \"最新\",\n    en: \"Create\"\n  },\n  sortNodeByModifiedAt: {\n    zh: \"最后修改\",\n    en: \"Update\"\n  },\n  sortNodeByTitle: {\n    zh: \"名称\",\n    en: \"Title\"\n  },\n  node2Trash: {\n    zh: \"移至回收桶\",\n    en: \"Move To Trash\"\n  },\n  nodeDelete: {\n    zh: \"删除\",\n    en: \"Delete\"\n  },\n  nodeDeleteConfirmation: {\n    zh: \"确认删除\",\n    en: \"Delete this thought\"\n  },\n  nodeRestoreFromTrash: {\n    zh: \"恢复\",\n    en: \"Restore\"\n  },\n  searchBarPlaceholder: {\n    zh: \"搜想法...\",\n    en: \"Search...\"\n  },\n  searchWindowSMSubmit: {\n    zh: \"搜索\",\n    en: \"Search\"\n  },\n  searchWindowSMCollapse: {\n    zh: \"收起\",\n    en: \"Collapse\"\n  },\n  noSearchResult: {\n    zh: \"没有搜索结果\",\n    en: \"No search result\"\n  },\n  search: {\n    zh: \"搜索\",\n    en: \"Search\"\n  },\n  headerBarNewThink: {\n    zh: \"新想法\",\n    en: \"New Thought\"\n  },\n  nodeTimeJustNow: {\n    zh: \"刚刚\",\n    en: \"Just now\"\n  },\n  nodeTimeYesterdayPrefix: {\n    zh: \"昨天\",\n    en: \"Yesterday\"\n  },\n  nodeTimeTodayPrefix: {\n    zh: \"今天\",\n    en: \"Today\"\n  },\n  nodeViewHeaderTitle: {\n    zh: \"标题\",\n    en: \"Title\"\n  },\n  nodeViewHeaderSnippet: {\n    zh: \"内容\",\n    en: \"Content\"\n  },\n  nodeViewHeaderTime: {\n    zh: \"时间\",\n    en: \"Time\"\n  },\n  sortNodeBySimilarity: {\n    zh: \"相似度\",\n    en: \"Similarity\"\n  },\n  cursorSearchDropdownSearchResult: {\n    zh: \"Rethink\",\n    en: \"Rethink\"\n  },\n  cursorSearchDropdownSearchRecent: {\n    zh: \"最近链接的想法\",\n    en: \"Recent linked thoughts\"\n  },\n  cursorSearchDropdownCreateNew: {\n    zh: \"新建\",\n    en: \"Create new\"\n  },\n  cursorSearchDropdownTitle: {\n    zh: \"选择连接的想法\",\n    en: \"Select a thought to link\"\n  },\n  emptyNodeTitle: {\n    zh: \"无标题\",\n    en: \"Untitled\"\n  },\n  settingsViewHeading: {\n    zh: \"设置\",\n    en: \"Settings\"\n  },\n  settingsViewGlobal: {\n    zh: \"全局设置\",\n    en: \"Global Settings\"\n  },\n  settingsLanguage: {\n    zh: \"语言\",\n    en: \"Language\"\n  },\n  settingsTheme: {\n    zh: \"主题\",\n    en: \"Theme\"\n  },\n  settingsViewEditor: {\n    zh: \"编辑器\",\n    en: \"Editor\"\n  },\n  settingsEditorMode: {\n    zh: \"模式\",\n    en: \"Mode\"\n  },\n  settingsEditorFontSize: {\n    zh: \"字体大小\",\n    en: \"Font Size\"\n  },\n  settingsEditorCodeTheme: {\n    zh: \"代码主题\",\n    en: \"Code Theme\"\n  },\n  settingsChangePwd: {\n    zh: \"修改密码\",\n    en: \"Change Password\"\n  },\n  settingsOldPwd: {\n    zh: \"旧密码\",\n    en: \"Old Password\"\n  },\n  settingsNewPwd: {\n    zh: \"新密码\",\n    en: \"New Password\"\n  },\n  settingsNewPwdConfirm: {\n    zh: \"确认新密码\",\n    en: \"Confirm New Password\"\n  },\n  settingsUpdatePwd: {\n    zh: \"更新密码\",\n    en: \"Update Password\"\n  },\n  settingsPwdNotMatch: {\n    zh: \"新密码与确认新密码不一致\",\n    en: \"New Password not match\"\n  },\n  settingsChangePwdHint: {\n    zh: \"修改密码\",\n    en: \"Change Password\"\n  },\n  settingsPwdUpdated: {\n    zh: \"密码已更新，请重新登陆\",\n    en: \"Password updated, please login again\"\n  },\n  settingsPwdSameAsOld: {\n    zh: \"新密码与旧密码相同\",\n    en: \"New password is the same as the old one\"\n  },\n  settingsIForgetMyPwd: {\n    zh: \"我忘记了我的密码\",\n    en: \"I forgot my password\"\n  },\n  userViewProfilePage: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  userProfileMeta: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  userViewName: {\n    zh: \"名字\",\n    en: \"Name\"\n  },\n  userViewEmail: {\n    zh: \"邮箱\",\n    en: \"Email\"\n  },\n  userViewAvatar: {\n    zh: \"头像\",\n    en: \"Picture\"\n  },\n  userProfileStats: {\n    zh: \"统计\",\n    en: \"Stats\"\n  },\n  userViewStorageUsage: {\n    zh: \"已使用:\",\n    en: \"Used Space:\"\n  },\n  loginViewHeading: {\n    zh: \"登录\",\n    en: \"Login\"\n  },\n  loginViewHeadingSignup: {\n    zh: \"新用户注册\",\n    en: \"New User Register\"\n  },\n  loginViewAccountLabel: {\n    zh: \"账号\",\n    en: \"Account\"\n  },\n  loginViewAccountPlaceholder: {\n    zh: \"邮箱\",\n    en: \"email\"\n  },\n  loginViewAccountInputTitle: {\n    zh: \"请输入正确的邮箱\",\n    en: \"Please input a valid email\"\n  },\n  loginViewPasswordLabel: {\n    zh: \"密码\",\n    en: \"Password\"\n  },\n  loginViewNoUserOrPassword: {\n    zh: \"账号或密码错误\",\n    en: \"Account or password error\"\n  },\n  loginViewAccountPasswordEmpty: {\n    zh: \"账号或密码不能为空\",\n    en: \"Account or password can not be empty\"\n  },\n  loginViewPasswordInputTitle: {\n    zh: \"必须包含至少 1 位数字和 1 位字母，且至少 6 个字符以上，最多 20 字符以下\",\n    en: \"Must contain at least one number and one letter, and at least 6 and less than 20 characters\"\n  },\n  loginViewConfirmPasswordLabel: {\n    zh: \"确认密码\",\n    en: \"Confirm password\"\n  },\n  loginViewConfirmPasswordNotMatch: {\n    zh: \"两次密码不一致\",\n    en: \"Confirm password not match\"\n  },\n  loginViewLoginButton: {\n    zh: \"登录\",\n    en: \"Log In\"\n  },\n  loginViewSignupButton: {\n    zh: \"注册\",\n    en: \"Create new account\"\n  },\n  loginViewSignupHasAccount: {\n    zh: \"已有账号？\",\n    en: \"Already have an account?\"\n  },\n  loginViewForgetPassword: {\n    zh: \"忘记密码\",\n    en: \"Forget password\"\n  },\n  loginViewWrongPasswordLength: {\n    zh: \"密码长度不正确，密码应在 6-20 字符之间\",\n    en: \"Password length is not correct, should be 6-20 characters\"\n  },\n  loginViewOAuthLogin: {\n    zh: \"其他方式登录\",\n    en: \"Other Login\"\n  },\n  notValidEmail: {\n    zh: \"邮箱格式不正确\",\n    en: \"Email format is not correct\"\n  },\n  registerCaptchaLabel: {\n    zh: \"验证码\",\n    en: \"Verification code\"\n  },\n  loginViewCaptchaEmpty: {\n    zh: \"验证码不能为空\",\n    en: \"Verification code can not be empty\"\n  },\n  forgetPasswordH1: {\n    zh: \"忘记密码\",\n    en: \"Forget password\"\n  },\n  forgetPasswordNewLabel: {\n    zh: \"新密码\",\n    en: \"New password\"\n  },\n  sendVerificationCode: {\n    zh: \"发送验证码\",\n    en: \"Send verification code\"\n  },\n  noCaptcha: {\n    zh: \"请先完成验证码\",\n    en: \"Please complete the verification code first\"\n  },\n  \"6digitalCode\": {\n    zh: \"6位数字验证码\",\n    en: \"6 digital code\"\n  },\n  resendVerificationCode: {\n    zh: \"重新发送验证码\",\n    en: \"Resend code\"\n  },\n  verificationCodeLabel: {\n    zh: \"验证码\",\n    en: \"Verification code\"\n  },\n  resetPasswordFailed: {\n    zh: \"重置密码失败\",\n    en: \"Reset password failed\"\n  },\n  headerMenuLogout: {\n    zh: \"登出\",\n    en: \"Logout\"\n  },\n  headerMenuProfile: {\n    zh: \"个人信息\",\n    en: \"Profile\"\n  },\n  headerMenuSettings: {\n    zh: \"设置\",\n    en: \"Settings\"\n  },\n  oauthPageHeading: {\n    zh: \"账号正在验证中...\",\n    en: \"Verifying your account...\"\n  },\n  msgBoxConfirmButton: {\n    zh: \"确定\",\n    en: \"OK\"\n  },\n  msgBoxCancelButton: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  modificationSuccessful: {\n    zh: \"修改成功\",\n    en: \"Modification successful\"\n  },\n  cancel: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  submit: {\n    zh: \"提交\",\n    en: \"Submit\"\n  },\n  next: {\n    zh: \"下一步\",\n    en: \"Next\"\n  },\n  recentSearchedTitle: {\n    zh: \"最近搜索\",\n    en: \"Recent Queries\"\n  },\n  editorContentPlaceholder: {\n    zh: \"记录我的新想法...\",\n    en: \"Record my new thought...\"\n  },\n  editorSyncStatusSaved: {\n    zh: \"已自动保存\",\n    en: \"Auto saved\"\n  },\n  editorSyncStatusLastSaved: {\n    zh: \"最近保存 \",\n    en: \"Last saved \"\n  },\n  editorHistMdRestoreConfirm: {\n    zh: \"确认恢复至该版本吗？\",\n    en: \"Confirm to restore this version?\"\n  },\n  editorExternalLinkConfirm: {\n    zh: \"点击确定将会去往外部链接：\",\n    en: \"Click OK to go to external link: \"\n  },\n  nodeHistEditionRestoreNoVersions: {\n    zh: \"没有历史版本\",\n    en: \"No history versions\"\n  },\n  nodeHistEditionRestoreHeading: {\n    zh: \"历史版本\",\n    en: \"History Versions\"\n  },\n  nodeHistEditionRestoreNotice: {\n    zh: \"恢复\",\n    en: \"Restore\"\n  },\n  quickPostPanelPlaceholder: {\n    zh: \"速记想法 / 链接 ...\",\n    en: \"Quick thought / link ...\"\n  },\n  quickPostBtn: {\n    zh: \"记下\",\n    en: \"Send\"\n  },\n  quickPostTooLong: {\n    zh: \"用编辑器记长想法 >\",\n    en: \"Use editor for long thought >\"\n  },\n  quickPostEditInNodePage: {\n    zh: \"在新页面编辑\",\n    en: \"Edit in new page\"\n  },\n  quickPostBtnTitle: {\n    zh: \"快速记录\",\n    en: \"Quick post\"\n  },\n  tryRestoreFromTrash: {\n    zh: \"此想法被放在回收站中，是否要从回收站恢复？\",\n    en: \"This thought is in trash, do you want to restore it?\"\n  },\n  nodeIsDeleted: {\n    zh: \"此想法已被您删除\",\n    en: \"This thought is deleted\"\n  },\n  noLinkedNode: {\n    zh: \"还没有链接到任何想法，尝试 @ 一些吧\",\n    en: \"No linked thought yet, try @ some\"\n  },\n  batchFileOpsShare: {\n    zh: \"分享\",\n    en: \"Share\"\n  },\n  batchFileOpsDelete: {\n    zh: \"删除\",\n    en: \"Delete\"\n  },\n  batchFileOpsTrash: {\n    zh: \"回收\",\n    en: \"To Trash\"\n  },\n  batchFileOpsCancel: {\n    zh: \"取消\",\n    en: \"Cancel\"\n  },\n  batchFileOpsDownload: {\n    zh: \"下载\",\n    en: \"Download\"\n  },\n  batchFileOpsRestore: {\n    zh: \"恢复\",\n    en: \"Restore\"\n  },\n  batchDeleteConfirmPre: {\n    zh: \"确认删除\",\n    en: \"Confirm to delete\"\n  },\n  batchDeleteConfirmPost: {\n    zh: \"个想法？\",\n    en: \"thoughts?\"\n  },\n  nodeNeedRestoreToView: {\n    zh: \"需要恢复后才能查看，确认恢复并查看？\",\n    en: \"Need restore to be viewed, confirm restore?\"\n  },\n  uploadFilesLabel: {\n    zh: \"上传文件\",\n    en: \"Upload files\"\n  },\n  uploadFilesEmptyTask: {\n    zh: \"无任务\",\n    en: \"No Task\"\n  },\n  fileDropIsDragging: {\n    zh: \"放入文件\",\n    en: \"Release to drop files here.\"\n  },\n  fileDropNotDraggingPre: {\n    zh: \"拖拽文件到此处或\",\n    en: \"Drag and drop files here, or \"\n  },\n  fileDropNotDraggingClick: {\n    zh: \"点此\",\n    en: \"click here\"\n  },\n  fileDropNotDraggingPost: {\n    zh: \" 上传\",\n    en: \" to upload\"\n  },\n  fileDropInvalidFile: {\n    zh: \"文件格式错误\",\n    en: \"Invalid file format\"\n  },\n  fileDropTooLarge: {\n    zh: \"文件过大\",\n    en: \"File too large\"\n  },\n  fileDropTooManyPre: {\n    zh: \"文件个数超过上限: \",\n    en: \"File count exceeds limit: \"\n  },\n  fileDropTooManyPost: {\n    zh: \"，请分批上传\",\n    en: \", please upload in batches\"\n  },\n  filesSubmitBtn: {\n    zh: \"上传\",\n    en: \"Upload\"\n  },\n  fileDropPreviewFileCount: {\n    zh: \"已加载文件数：\",\n    en: \"Loaded file count: \"\n  },\n  uploadFilesTaskNotFinished: {\n    zh: \"任务未完成: \",\n    en: \"Task not finished: \"\n  },\n  newJobProgress: {\n    zh: \"最新任务进度\",\n    en: \"The latest job progress\"\n  },\n  autoRecommendation: {\n    zh: \"自动展示相关想法...\",\n    en: \"Auto show related thoughts...\"\n  },\n  pluginPanelDescription: {\n    zh: \"插件是一种括展能力，可以基于你的想法库，延伸不同的功能。当前仅可以在私有化部署的版本中，开发、体验自己的插件。\",\n    en: \"Plugin is an extension capability, which can extend different functions based on your own data. \" + \"Currently, you can only develop and view your own plugins in the self-hosted version.\"\n  },\n  pluginPageTitle: {\n    zh: \"插件页\",\n    en: \"Plugin page\"\n  }\n});\n/* harmony default export */ __webpack_exports__[\"default\"] = (mLang);\n\n//# sourceURL=webpack://rethink/./src/utils/multiLang.ts?");
 
                 /***/
             }),
 
         /***/
         "./src/utils/requestId.ts":
             /*!********************************!*\
@@ -3169,14 +3208,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n// extracted by mini-css-extract-plugin\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use%5B0%5D!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use%5B1%5D!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use%5B2%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
 
                 /***/
             }),
 
         /***/
+        "./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css":
+            /*!*************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
+  !*** ./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css ***!
+  \*************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n// extracted by mini-css-extract-plugin\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use%5B0%5D!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use%5B1%5D!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use%5B2%5D!./node_modules/vue-loader/dist/index.js??ruleSet%5B0%5D.use%5B0%5D");
+
+                /***/
+            }),
+
+        /***/
         "./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=style&index=0&id=404f2c61&scoped=true&lang=css":
             /*!*************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************!*\
   !*** ./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=style&index=0&id=404f2c61&scoped=true&lang=css ***!
   \*************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -4157,14 +4209,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _RecommendPopupWindow_vue_vue_type_template_id_68a8b995_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! ./RecommendPopupWindow.vue?vue&type=template&id=68a8b995&scoped=true&ts=true */ \"./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=template&id=68a8b995&scoped=true&ts=true\");\n/* harmony import */ var _RecommendPopupWindow_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./RecommendPopupWindow.vue?vue&type=script&lang=ts&setup=true */ \"./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=script&lang=ts&setup=true\");\n/* harmony import */ var _RecommendPopupWindow_vue_vue_type_style_index_0_id_68a8b995_scoped_true_lang_css__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./RecommendPopupWindow.vue?vue&type=style&index=0&id=68a8b995&scoped=true&lang=css */ \"./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=style&index=0&id=68a8b995&scoped=true&lang=css\");\n/* harmony import */ var _node_modules_vue_loader_dist_exportHelper_js__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ../../../../../node_modules/vue-loader/dist/exportHelper.js */ \"./node_modules/vue-loader/dist/exportHelper.js\");\n\n\n\n\n\n\n\nconst __exports__ = /*#__PURE__*/(0,_node_modules_vue_loader_dist_exportHelper_js__WEBPACK_IMPORTED_MODULE_3__[\"default\"])(_RecommendPopupWindow_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_1__[\"default\"], [['render',_RecommendPopupWindow_vue_vue_type_template_id_68a8b995_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__.render],['__scopeId',\"data-v-68a8b995\"],['__file',\"src/components/app/editor/recom/RecommendPopupWindow.vue\"]])\n/* hot reload */\nif (false) {}\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (__exports__);\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?");
 
                 /***/
             }),
 
         /***/
+        "./src/components/app/editor/sidebar/HistRestore.vue":
+            /*!***********************************************************!*\
+  !*** ./src/components/app/editor/sidebar/HistRestore.vue ***!
+  \***********************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _HistRestore_vue_vue_type_template_id_7e97cf55_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! ./HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true */ \"./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true\");\n/* harmony import */ var _HistRestore_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_1__ = __webpack_require__(/*! ./HistRestore.vue?vue&type=script&lang=ts&setup=true */ \"./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true\");\n/* harmony import */ var _HistRestore_vue_vue_type_style_index_0_id_7e97cf55_scoped_true_lang_css__WEBPACK_IMPORTED_MODULE_2__ = __webpack_require__(/*! ./HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css */ \"./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css\");\n/* harmony import */ var _node_modules_vue_loader_dist_exportHelper_js__WEBPACK_IMPORTED_MODULE_3__ = __webpack_require__(/*! ../../../../../node_modules/vue-loader/dist/exportHelper.js */ \"./node_modules/vue-loader/dist/exportHelper.js\");\n\n\n\n\n\n\n\nconst __exports__ = /*#__PURE__*/(0,_node_modules_vue_loader_dist_exportHelper_js__WEBPACK_IMPORTED_MODULE_3__[\"default\"])(_HistRestore_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_1__[\"default\"], [['render',_HistRestore_vue_vue_type_template_id_7e97cf55_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__.render],['__scopeId',\"data-v-7e97cf55\"],['__file',\"src/components/app/editor/sidebar/HistRestore.vue\"]])\n/* hot reload */\nif (false) {}\n\n\n/* harmony default export */ __webpack_exports__[\"default\"] = (__exports__);\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?");
+
+                /***/
+            }),
+
+        /***/
         "./src/components/app/editor/sidebar/LinkedNodes.vue":
             /*!***********************************************************!*\
   !*** ./src/components/app/editor/sidebar/LinkedNodes.vue ***!
   \***********************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -5288,14 +5353,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"default\": function() { return /* reexport safe */ _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_RecommendPopupWindow_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_0__[\"default\"]; }\n/* harmony export */ });\n/* harmony import */ var _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_RecommendPopupWindow_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/babel-loader/lib/index.js!../../../../../node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./RecommendPopupWindow.vue?vue&type=script&lang=ts&setup=true */ \"./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=script&lang=ts&setup=true\");\n \n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?");
 
                 /***/
             }),
 
         /***/
+        "./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true":
+            /*!**********************************************************************************************!*\
+  !*** ./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true ***!
+  \**********************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   \"default\": function() { return /* reexport safe */ _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_HistRestore_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_0__[\"default\"]; }\n/* harmony export */ });\n/* harmony import */ var _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_HistRestore_vue_vue_type_script_lang_ts_setup_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/babel-loader/lib/index.js!../../../../../node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./HistRestore.vue?vue&type=script&lang=ts&setup=true */ \"./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=script&lang=ts&setup=true\");\n \n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?");
+
+                /***/
+            }),
+
+        /***/
         "./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=script&lang=ts&setup=true":
             /*!**********************************************************************************************!*\
   !*** ./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=script&lang=ts&setup=true ***!
   \**********************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -6419,14 +6497,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* reexport safe */ _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_templateLoader_js_ruleSet_1_rules_4_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_RecommendPopupWindow_vue_vue_type_template_id_68a8b995_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__.render; }\n/* harmony export */ });\n/* harmony import */ var _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_templateLoader_js_ruleSet_1_rules_4_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_RecommendPopupWindow_vue_vue_type_template_id_68a8b995_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/babel-loader/lib/index.js!../../../../../node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!../../../../../node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./RecommendPopupWindow.vue?vue&type=template&id=68a8b995&scoped=true&ts=true */ \"./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=template&id=68a8b995&scoped=true&ts=true\");\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?");
 
                 /***/
             }),
 
         /***/
+        "./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true":
+            /*!*************************************************************************************************************!*\
+  !*** ./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true ***!
+  \*************************************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony export */ __webpack_require__.d(__webpack_exports__, {\n/* harmony export */   render: function() { return /* reexport safe */ _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_templateLoader_js_ruleSet_1_rules_4_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_HistRestore_vue_vue_type_template_id_7e97cf55_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__.render; }\n/* harmony export */ });\n/* harmony import */ var _node_modules_babel_loader_lib_index_js_node_modules_ts_loader_index_js_clonedRuleSet_41_use_1_node_modules_vue_loader_dist_templateLoader_js_ruleSet_1_rules_4_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_HistRestore_vue_vue_type_template_id_7e97cf55_scoped_true_ts_true__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/babel-loader/lib/index.js!../../../../../node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!../../../../../node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true */ \"./node_modules/babel-loader/lib/index.js!./node_modules/ts-loader/index.js??clonedRuleSet-41.use[1]!./node_modules/vue-loader/dist/templateLoader.js??ruleSet[1].rules[4]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=template&id=7e97cf55&scoped=true&ts=true\");\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?");
+
+                /***/
+            }),
+
+        /***/
         "./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=template&id=404f2c61&scoped=true&ts=true":
             /*!*************************************************************************************************************!*\
   !*** ./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=template&id=404f2c61&scoped=true&ts=true ***!
   \*************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -7537,14 +7628,27 @@
 
                 eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _node_modules_mini_css_extract_plugin_dist_loader_js_clonedRuleSet_12_use_0_node_modules_css_loader_dist_cjs_js_clonedRuleSet_12_use_1_node_modules_vue_loader_dist_stylePostLoader_js_node_modules_postcss_loader_dist_cjs_js_clonedRuleSet_12_use_2_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_RecommendPopupWindow_vue_vue_type_style_index_0_id_68a8b995_scoped_true_lang_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!../../../../../node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!../../../../../node_modules/vue-loader/dist/stylePostLoader.js!../../../../../node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./RecommendPopupWindow.vue?vue&type=style&index=0&id=68a8b995&scoped=true&lang=css */ \"./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/recom/RecommendPopupWindow.vue?vue&type=style&index=0&id=68a8b995&scoped=true&lang=css\");\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/recom/RecommendPopupWindow.vue?");
 
                 /***/
             }),
 
         /***/
+        "./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css":
+            /*!*******************************************************************************************************************!*\
+  !*** ./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css ***!
+  \*******************************************************************************************************************/
+            /***/
+            (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
+
+                eval("__webpack_require__.r(__webpack_exports__);\n/* harmony import */ var _node_modules_mini_css_extract_plugin_dist_loader_js_clonedRuleSet_12_use_0_node_modules_css_loader_dist_cjs_js_clonedRuleSet_12_use_1_node_modules_vue_loader_dist_stylePostLoader_js_node_modules_postcss_loader_dist_cjs_js_clonedRuleSet_12_use_2_node_modules_vue_loader_dist_index_js_ruleSet_0_use_0_HistRestore_vue_vue_type_style_index_0_id_7e97cf55_scoped_true_lang_css__WEBPACK_IMPORTED_MODULE_0__ = __webpack_require__(/*! -!../../../../../node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!../../../../../node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!../../../../../node_modules/vue-loader/dist/stylePostLoader.js!../../../../../node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!../../../../../node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css */ \"./node_modules/mini-css-extract-plugin/dist/loader.js??clonedRuleSet-12.use[0]!./node_modules/css-loader/dist/cjs.js??clonedRuleSet-12.use[1]!./node_modules/vue-loader/dist/stylePostLoader.js!./node_modules/postcss-loader/dist/cjs.js??clonedRuleSet-12.use[2]!./node_modules/vue-loader/dist/index.js??ruleSet[0].use[0]!./src/components/app/editor/sidebar/HistRestore.vue?vue&type=style&index=0&id=7e97cf55&scoped=true&lang=css\");\n\n\n//# sourceURL=webpack://rethink/./src/components/app/editor/sidebar/HistRestore.vue?");
+
+                /***/
+            }),
+
+        /***/
         "./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=style&index=0&id=404f2c61&scoped=true&lang=css":
             /*!*******************************************************************************************************************!*\
   !*** ./src/components/app/editor/sidebar/LinkedNodes.vue?vue&type=style&index=0&id=404f2c61&scoped=true&lang=css ***!
   \*******************************************************************************************************************/
             /***/
             (function(__unused_webpack_module, __webpack_exports__, __webpack_require__) {
 
@@ -8525,14 +8629,27 @@
 
                 eval("module.exports = __webpack_require__.p + \"img/recentoutline.svg\";\n\n//# sourceURL=webpack://rethink/./src/assets/images/icons/recentoutline.svg?");
 
                 /***/
             }),
 
         /***/
+        "./src/assets/images/icons/restore.svg":
+            /*!*********************************************!*\
+  !*** ./src/assets/images/icons/restore.svg ***!
+  \*********************************************/
+            /***/
+            (function(module, __unused_webpack_exports, __webpack_require__) {
+
+                eval("module.exports = __webpack_require__.p + \"img/restore.svg\";\n\n//# sourceURL=webpack://rethink/./src/assets/images/icons/restore.svg?");
+
+                /***/
+            }),
+
+        /***/
         "./src/assets/images/icons/return-arrow.svg":
             /*!**************************************************!*\
   !*** ./src/assets/images/icons/return-arrow.svg ***!
   \**************************************************/
             /***/
             (function(module, __unused_webpack_exports, __webpack_require__) {
```

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/js/chunk-vendors.js` & `rethink-note-0.2.4/src/rethink/dist-local/js/chunk-vendors.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/js/highlight.min.js` & `rethink-note-0.2.4/src/rethink/dist-local/js/highlight.min.js`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/dist-local/media/demo.mp4` & `rethink-note-0.2.4/src/rethink/dist-local/media/demo.mp4`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/logger.py` & `rethink-note-0.2.4/src/rethink/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 log_date_format = "%Y-%m-%d %H:%M:%S"
 logging.basicConfig(
     level=logging.ERROR,
     format=log_format,
     datefmt=log_date_format,
 )
 logger = logging.getLogger("rethink")
-logger.setLevel(logging.INFO)
+logger.setLevel(logging.ERROR)
 
 
 # add rotating file handler
 def add_rotating_file_handler(log_dir: str, max_bytes: int, backup_count: int):
     if not os.path.exists(log_dir):
         os.mkdir(log_dir)
     file_handler = RotatingFileHandler(
```

### Comparing `rethink-note-0.2.3/src/rethink/models/client.py` & `rethink-note-0.2.4/src/rethink/models/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import calendar
 import datetime
-import json
 import os
 import struct
 from typing import Optional, Union
 
 from bson import ObjectId
 from bson.tz_util import utc
 
-from rethink import config, const, utils
+from rethink import config, const, utils, version_manager
 from rethink.depend.mongita import MongitaClientDisk
 from rethink.logger import logger
 from rethink.models.search_engine.engine import BaseEngine, SearchDoc, RestoreSearchDoc
 from rethink.models.search_engine.engine_local import LocalSearcher
 from .coll import Collections
 from .indexing import remote_try_build_index
 from .tps import UserFile, ImportData, UserMeta, Node
@@ -84,55 +83,39 @@
             await self.search.drop()
         if self.mongo is not None:
             if isinstance(self.mongo, MongitaClientDisk):
                 await self.mongo.close()
             await self.mongo.drop_database(config.get_settings().DB_NAME)
 
     async def local_try_add_default_user(self):
-        dot_rethink_path = config.get_settings().LOCAL_STORAGE_PATH / ".data" / ".rethink.json"
-        u_insertion = {
-            "_id": ObjectId(),
-            "id": utils.short_uuid(),
-            "email": const.DEFAULT_USER["email"],
-            "nickname": const.DEFAULT_USER["nickname"],
-            "avatar": const.DEFAULT_USER["avatar"],
-            "account": const.DEFAULT_USER["email"],
-            "settings": {
-                "language": os.getenv("VUE_APP_LANGUAGE", const.Language.EN.value),
-                "theme": const.AppTheme.LIGHT.value,
-                "editorMode": const.EditorMode.WYSIWYG.value,
-                "editorFontSize": 15,
-                "editorCodeTheme": const.EditorCodeTheme.GITHUB.value,
-            }
-        }
-        with open(dot_rethink_path, "w", encoding="utf-8") as f:
-            out = u_insertion.copy()
-            out["_id"] = str(out["_id"])
-            json.dump(out, f, indent=2, ensure_ascii=False)
+        _v = version_manager.recover.dump_dot_rethink(
+            path=config.get_settings().LOCAL_STORAGE_PATH / ".data" / ".rethink.json"
+        )
 
         logger.info("running at the first time, a user with initial data will be created")
-        ns = const.NEW_USER_DEFAULT_NODES[u_insertion["settings"]["language"]]
+        ns = const.NEW_USER_DEFAULT_NODES[_v["settings"]["language"]]
         search_docs = []
 
         async def create_node(md: str, to_nid: Optional[str] = None):
             title_, body_, snippet_ = utils.preprocess_md(md)
             n: Node = {
                 "_id": ObjectId(),
                 "id": utils.short_uuid(),
-                "uid": u_insertion["id"],
+                "uid": _v["id"],
                 "title": title_,
                 "snippet": snippet_,
                 "md": md,
                 "type": const.NodeType.MARKDOWN.value,
                 "disabled": False,
                 "inTrash": False,
                 "modifiedAt": datetime.datetime.now(tz=utc),
                 "inTrashAt": None,
                 "fromNodeIds": [],
                 "toNodeIds": [] if to_nid is None else [to_nid],
+                "history": [],
             }
             res = await self.coll.nodes.insert_one(n)
             if not res.acknowledged:
                 raise ValueError("cannot insert default node")
             search_docs.append(
                 SearchDoc(
                     nid=n["id"],
@@ -147,46 +130,47 @@
             return n
 
         n0 = await create_node(ns[0])
         _md = ns[1].format(n0["id"])
         n1 = await create_node(_md, to_nid=n0["id"])
 
         u: UserMeta = {
-            "_id": ObjectId(u_insertion["_id"]),
-            "id": u_insertion["id"],
-            "email": u_insertion["email"],
-            "nickname": u_insertion["nickname"],
-            "avatar": u_insertion["avatar"],
-            "account": u_insertion["email"],
+            "_id": ObjectId(_v["_id"]),
+            "id": _v["id"],
+            "email": _v["email"],
+            "nickname": _v["nickname"],
+            "avatar": _v["avatar"],
+            "account": _v["email"],
 
             "source": const.UserSource.LOCAL.value,
             "hashed": "",
             "disabled": False,
             "modifiedAt": datetime.datetime.now(tz=utc),
             "usedSpace": 0,
             "type": const.USER_TYPE.NORMAL.id,
             "lastState": {
                 "recentCursorSearchSelectedNIds": [n0["id"], n1["id"]],
                 "recentSearch": [],
                 "nodeDisplayMethod": const.NodeDisplayMethod.CARD.value,
                 "nodeDisplaySortKey": "modifiedAt"
             },
-            "settings": u_insertion["settings"],
+            "settings": _v["settings"],
         }
         _ = await self.coll.users.insert_one(u)
 
         await self.search.add_batch(
             uid=u["id"],
             docs=search_docs,
         )
 
     async def local_try_create_or_restore(self):  # noqa: C901
         if not config.get_settings().ONE_USER:
             return
 
+        version_manager.migrate.to_latest_version(config.get_settings().LOCAL_STORAGE_PATH)
         # check if field changes
         for c, t in [
             (self.coll.users, UserMeta),
             (self.coll.nodes, Node),
             (self.coll.user_file, UserFile),
             (self.coll.import_data, ImportData),
         ]:
@@ -230,46 +214,48 @@
             return
 
         # no default user, create one
         await self.local_try_add_default_user()
 
     async def _local_restore(self):
         # restore user
-        dot_rethink_path = config.get_settings().LOCAL_STORAGE_PATH / ".data" / ".rethink.json"
-        if not dot_rethink_path.exists():
+        _v = version_manager.recover.load_dot_rethink(
+            path=config.get_settings().LOCAL_STORAGE_PATH / ".data" / ".rethink.json"
+        )
+        if _v is None:
             return
-        with open(dot_rethink_path, "r", encoding="utf-8") as f:
-            u_insertion = json.load(f)
 
         u: UserMeta = {
-            "_id": ObjectId(u_insertion["_id"]),
-            "id": u_insertion["id"],
-            "email": u_insertion["email"],
-            "nickname": u_insertion["nickname"],
-            "avatar": u_insertion["avatar"],
-            "account": u_insertion["email"],
+            "_id": ObjectId(_v["_id"]),
+            "id": _v["id"],
+            "email": _v["email"],
+            "nickname": _v["nickname"],
+            "avatar": _v["avatar"],
+            "account": _v["email"],
 
             "source": const.UserSource.LOCAL.value,
             "hashed": "",
             "disabled": False,
             "modifiedAt": datetime.datetime.now(tz=utc),
             "usedSpace": 0,
             "type": const.USER_TYPE.NORMAL.id,
             "lastState": {
                 "recentCursorSearchSelectedNIds": [],
                 "recentSearch": [],
                 "nodeDisplayMethod": const.NodeDisplayMethod.CARD.value,
                 "nodeDisplaySortKey": "modifiedAt"
             },
-            "settings": u_insertion.get("settings", {
+            "settings": _v.get("settings", {
                 "language": os.getenv("VUE_APP_LANGUAGE", const.Language.EN.value),
                 "theme": const.AppTheme.LIGHT.value,
                 "editorMode": const.EditorMode.WYSIWYG.value,
                 "editorFontSize": 15,
                 "editorCodeTheme": const.EditorCodeTheme.GITHUB.value,
+                "editorSepRightWidth": 200,
+                "editorSideCurrentToolId": "",
             }),
         }
         _ = await self.coll.users.insert_one(u)
 
         # restore nodes
         md_dir = config.get_settings().LOCAL_STORAGE_PATH / ".data" / "md"
         if not md_dir.exists():
@@ -281,62 +267,63 @@
             created_time = datetime.datetime.fromtimestamp(md_path.stat().st_ctime, tz=utc)
             modified_time = datetime.datetime.fromtimestamp(md_path.stat().st_mtime, tz=utc)
             title_, body_, snippet_ = utils.preprocess_md(md)
 
             n: Node = {
                 "_id": _oid_from_datetime(created_time),
                 "id": md_path.stem,
-                "uid": u_insertion["id"],
+                "uid": _v["id"],
                 "title": title_,
                 "snippet": snippet_,
                 "md": md,
                 "type": const.NodeType.MARKDOWN.value,
                 "disabled": False,
                 "inTrash": False,
                 "modifiedAt": modified_time,
                 "inTrashAt": None,
                 "fromNodeIds": [],
                 "toNodeIds": [],
+                "history": [],
             }
             ns.append(n)
             search_docs.append(
                 SearchDoc(
                     nid=n["id"],
                     title=title_,
                     body=body_,
                 )
             )
         res = await self.coll.nodes.insert_many(ns)
         if not res.acknowledged:
             raise ValueError("cannot insert default node")
-        logger.info(f"restore nodes count: {len(res.inserted_ids)}")
+        logger.debug(f"restore nodes count: {len(res.inserted_ids)}")
 
         docs = []
         for f in config.get_settings().LOCAL_STORAGE_PATH.glob(".data/files/*"):
             filename = f.name
             fid = filename.split(".")[0]
             created_time = datetime.datetime.fromtimestamp(f.stat().st_ctime, tz=utc)
             docs.append({
                 "_id": _oid_from_datetime(created_time),
-                "uid": u_insertion["id"],
+                "uid": _v["id"],
                 "fid": fid,
                 "filename": filename,
                 "size": f.stat().st_size,
             })
         res = await self.coll.user_file.insert_many(docs)
         if not res.acknowledged:
             raise ValueError("cannot insert default node")
 
         await self.search.drop()
         await self.search.init()
         await self.search.add_batch(
             uid=u["id"],
             docs=search_docs,
         )
-        logger.info(f"restore files count: {len(res.inserted_ids)}")
+        logger.debug(f"restore files count: {len(res.inserted_ids)}")
 
     async def try_restore_search(self):
         count_mongo = await self.coll.nodes.count_documents({})
         count_search = await self.search.count_all()
         if count_mongo == count_search:
             return
         await self.search.drop()
@@ -361,15 +348,15 @@
         for uid, docs in search_docs.items():
             code = await self.search.batch_restore_docs(
                 uid=uid,
                 docs=docs,
             )
             if code != const.Code.OK:
                 raise ValueError("cannot restore search index")
-        logger.info(f"restore search index count: {count_mongo}")
+        logger.debug(f"restore search index count: {count_mongo}")
 
 
 def _oid_from_datetime(dt: datetime.datetime) -> ObjectId:
     offset = dt.utcoffset()
     if offset is not None:
         dt = dt - offset
     timestamp = calendar.timegm(dt.timetuple())
```

### Comparing `rethink-note-0.2.3/src/rethink/models/db_ops.py` & `rethink-note-0.2.4/src/rethink/models/db_ops.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/indexing.py` & `rethink-note-0.2.4/src/rethink/models/indexing.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/search_engine/baidu_stopwords.txt` & `rethink-note-0.2.4/src/rethink/models/search_engine/baidu_stopwords.txt`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/search_engine/cn_stopwords.txt` & `rethink-note-0.2.4/src/rethink/models/search_engine/cn_stopwords.txt`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/search_engine/engine.py` & `rethink-note-0.2.4/src/rethink/models/search_engine/engine.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/search_engine/engine_es.py` & `rethink-note-0.2.4/src/rethink/models/search_engine/engine_es.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         if resp.meta.status != 200:
             raise RuntimeError(f"reindex failed, resp: {resp}")
         resp = await self.es.indices.delete(index=self.index)
         if resp.meta.status != 200:
             raise RuntimeError(f"reindex failed, resp: {resp}")
 
         self.index = new_index
-        logger.info(f"elasticsearch reindex finished, new index: {self.index}")
+        logger.debug(f"elasticsearch reindex finished, new index: {self.index}")
 
     async def drop(self):
         await self.connect()
         if self.index != "" and await self.es.indices.exists(index=self.index):
             await self.es.indices.delete(index=self.index)
         self.index = ""
         await self.es.close()
```

### Comparing `rethink-note-0.2.3/src/rethink/models/search_engine/engine_local.py` & `rethink-note-0.2.4/src/rethink/models/search_engine/engine_local.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/models/tps.py` & `rethink-note-0.2.4/src/rethink/models/tps.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     type: int  # const.NodeType.MARKDOWN.value
     disabled: bool
     inTrash: bool
     modifiedAt: datetime.datetime
     inTrashAt: Optional[datetime.datetime]
     fromNodeIds: List[str]
     toNodeIds: List[str]
+    history: List[str]
 
 
 class _LastState(TypedDict):
     nodeDisplayMethod: int
     nodeDisplaySortKey: str
     recentSearch: List[str]
     recentCursorSearchSelectedNIds: List[str]
```

### Comparing `rethink-note-0.2.3/src/rethink/plugins/base.py` & `rethink-note-0.2.4/src/rethink/plugins/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,17 +150,18 @@
         in your template html, you can pass this url to your javascript code to connect self.handle_api_call() method.
 
         Returns:
             str: the api call url
         """
         try:
             port = os.environ["VUE_APP_API_PORT"]
+            host = os.environ['RETHINK_HOSTNAME']
         except KeyError:
-            raise ValueError("the port number is not set in the environment variable VUE_APP_API_PORT.")
-        return f"http://localhost:{port}/api/plugin/call"
+            raise ValueError("the host or port number is not set in the environment.")
+        return f"http://{host}:{port}/api/plugin/call"
 
 
 event_plugin_map: Dict[str, List[Plugin]] = {
     "on_node_added": [],
     "before_node_updated": [],
     "on_node_updated": [],
     "on_schedule": [],
```

### Comparing `rethink-note-0.2.3/src/rethink/plugins/handler.py` & `rethink-note-0.2.4/src/rethink/plugins/handler.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/_static/logo.svg` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/main.py` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/main.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/templates/home.html` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/home.html`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/favorites/templates/side.html` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/favorites/templates/side.html`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/_static/image/logo.svg` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/_static/image/logo.svg`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/main.py` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/main.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/templates/home.html` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/templates/home.html`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/official_plugins/summary/templates/side.html` & `rethink-note-0.2.4/src/rethink/plugins/official_plugins/summary/templates/side.html`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/plugins/schedule/timing.py` & `rethink-note-0.2.4/src/rethink/plugins/schedule/timing.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/regex.py` & `rethink-note-0.2.4/src/rethink/regex.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/email.py` & `rethink-note-0.2.4/src/rethink/routes/email.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/files.py` & `rethink-note-0.2.4/src/rethink/routes/files.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/node.py` & `rethink-note-0.2.4/src/rethink/routes/node.py`

 * *Files 10% similar despite different names*

```diff
@@ -87,7 +87,37 @@
         req: schemas.node.CoreNodesRequest,
         token_decode: Annotated[TokenDecode, Depends(token2uid)]
 ) -> schemas.node.CoreNodesResponse:
     return await node_ops.get_core_nodes(
         td=token_decode,
         req=req,
     )
+
+
+@router.post(
+    path="/node/hist",
+    response_model=schemas.node.HistEditionsResponse,
+)
+@measure_time_spend
+async def get_hist_editions(
+        req: schemas.node.HistEditionsRequest,
+        token_decode: Annotated[TokenDecode, Depends(token2uid)]
+) -> schemas.node.HistEditionsResponse:
+    return await node_ops.get_hist_editions(
+        td=token_decode,
+        req=req,
+    )
+
+
+@router.post(
+    path="/node/hist/md",
+    response_model=schemas.node.HistEditionMdResponse,
+)
+@measure_time_spend
+async def get_hist_md(
+        req: schemas.node.HistEditionMdRequest,
+        token_decode: Annotated[TokenDecode, Depends(token2uid)]
+) -> schemas.node.HistEditionMdResponse:
+    return await node_ops.get_hist_edition_md(
+        td=token_decode,
+        req=req,
+    )
```

### Comparing `rethink-note-0.2.3/src/rethink/routes/oauth.py` & `rethink-note-0.2.4/src/rethink/routes/oauth.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/plugin.py` & `rethink-note-0.2.4/src/rethink/routes/plugin.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/search.py` & `rethink-note-0.2.4/src/rethink/routes/search.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/trash.py` & `rethink-note-0.2.4/src/rethink/routes/trash.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/routes/user.py` & `rethink-note-0.2.4/src/rethink/routes/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 
 @router.post(
     path="/user/password/update",
     response_model=schemas.base.AcknowledgeResponse,
 )
 @measure_time_spend
-async def update_user(
+async def update_user_password(
         req: schemas.user.UpdatePasswordRequest,
         token_decode: Annotated[TokenDecode, Depends(token2uid)],
         referer: Optional[str] = Depends(verify_referer),
 ) -> schemas.base.AcknowledgeResponse:
     return await password.update(
         td=token_decode,
         req=req,
```

### Comparing `rethink-note-0.2.3/src/rethink/routes/utils.py` & `rethink-note-0.2.4/src/rethink/routes/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,23 @@
         uid = ""
         code = ""
         if "token_decode" in kwargs:
             uid = kwargs["token_decode"].uid
             code = kwargs["token_decode"].code
         req_s = req_s[:200] + "..." if len(req_s) > 200 else req_s
         if func.__name__ not in ["login", "reset_password", "register"]:
-            logger.info(f"REQ: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | code='{code}' | {req_s}")
+            logger.debug(f"REQ: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | code='{code}' | {req_s}")
 
         resp = await func(*args, **kwargs)
         t1 = time.perf_counter()
         try:
             req_id = resp.requestId
         except AttributeError:
             req_id = ""
-        logger.info(f"RESP: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | spend={t1 - t0:.4f}s")
+        logger.debug(f"RESP: reqId='{req_id}' | uid='{uid}' | api='{func.__name__}' | spend={t1 - t0:.4f}s")
         return resp
 
     return wrapper
 
 
 def verify_referer(referer: Optional[str] = Header(None)):
     if config.get_settings().VERIFY_REFERER and not referer.startswith(REFERER_PREFIX):
```

### Comparing `rethink-note-0.2.3/src/rethink/routes/verification.py` & `rethink-note-0.2.4/src/rethink/routes/verification.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/src/rethink/run.py` & `rethink-note-0.2.4/src/rethink/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,31 +56,33 @@
     td = threading.Thread(target=scheduler.run)
     td.start()
     return td
 
 
 def run(
         path: Union[str, Path] = None,
-        host="127.0.0.1",
-        port=8000,
+        host: str = "127.0.0.1",
+        port: int = 8000,
         language: Literal["en", "zh"] = "en",
+        headless: bool = False,
+        debug: bool = False,
 ):
     """
     Run the server.
 
     Args:
         path (str): the database path for text and file data.
-         Rethink will create .data folder in this path, default is current working directory.
+            Rethink will create .data folder in this path, default is current working directory.
         host (str): server host, default is the localhost.
         port (int): server port, default is 8000.
         language (str): website language, default is English.
-         Possible values are "en" and "zh".
-
-    Returns:
-        None
+            Possible values are "en" and "zh".
+        headless (bool): run the server in headless mode. if False, it will open a browser after startup.
+            default is False.
+        debug (bool): run the server in debug mode. default is False.
 
     Raises:
         FileNotFoundError: if the path not exists.
         NotADirectoryError: if the path is not a directory.
     """
     if path is None:
         path = os.getcwd()
@@ -90,19 +92,23 @@
         raise FileNotFoundError(f"Path not exists: {path}")
     if not path.is_dir():
         raise NotADirectoryError(f"Path is not a directory: {path}")
     os.environ["LOCAL_STORAGE_PATH"] = str(path)
     os.environ["VUE_APP_API_PORT"] = str(port)
     os.environ["VUE_APP_MODE"] = "local"
     os.environ["VUE_APP_LANGUAGE"] = language
+    os.environ["RETHINK_HEADLESS"] = "1" if headless else "0"
+    os.environ["RETHINK_HOSTNAME"] = host
+    os.environ["DEBUG"] = "true" if debug else "false"
 
     td = _start_on_schedule_plugins()
 
     uvicorn.run(
         "rethink.application:app",
         host=host,
         port=port,
         reload=False,
         workers=1,
+        log_level="error",
         env_file=os.path.join(os.path.abspath(os.path.dirname(__file__)), ".env.local"),
     )
     td.join()
```

### Comparing `rethink-note-0.2.3/src/rethink/utils.py` & `rethink-note-0.2.4/src/rethink/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         no_title = "No title found"
         no_description = "No description found"
     else:
         no_title = "No title found"
         no_description = "No description found"
 
     if count > 2:
-        logger.info(f"too many 30X code, failed to get {url}")
+        logger.debug(f"too many 30X code, failed to get {url}")
         return no_title, no_description
 
     # SSRF protection
     if ssrf_check(url):
         return no_title, no_description
     # end of SSRF protection
 
@@ -249,15 +249,15 @@
         except (
                 httpx.ConnectTimeout,
                 RuntimeError,
                 httpx.ConnectError,
                 httpx.ReadTimeout,
                 httpx.HTTPError
         ) as e:
-            logger.info(f"failed to get {url}: {e}")
+            logger.debug(f"failed to get {url}: {e}")
             return no_title, no_description
         if response.status_code in (301, 302):
             return await get_title_description_from_link(
                 url=response.headers["Location"],
                 language=language,
                 count=count + 1,
             )
```

### Comparing `rethink-note-0.2.3/src/rethink_note.egg-info/PKG-INFO` & `rethink-note-0.2.4/src/rethink_note.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rethink-note
-Version: 0.2.3
+Version: 0.2.4
 Summary: note taking app
 Home-page: https://github.com/MorvanZhou/rethink
 Author: MorvanZhou
 Author-email: morvanzhou@hotmail.com
 Project-URL: Bug Tracker, https://github.com/MorvanZhou/rethink/issues
 Project-URL: Source, https://github.com/MorvanZhou/rethink
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rethink-note Version: 0.2.3 Summary: note taking
+Metadata-Version: 2.1 Name: rethink-note Version: 0.2.4 Summary: note taking
 app Home-page: https://github.com/MorvanZhou/rethink Author: MorvanZhou Author-
 email: morvanzhou@hotmail.com Project-URL: Bug Tracker, https://github.com/
 MorvanZhou/rethink/issues Project-URL: Source, https://github.com/MorvanZhou/
 rethink Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `rethink-note-0.2.3/src/rethink_note.egg-info/SOURCES.txt` & `rethink-note-0.2.4/src/rethink_note.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/rethink/.env.local
 src/rethink/__init__.py
+src/rethink/_version.py
 src/rethink/application.py
 src/rethink/config.py
 src/rethink/const.py
 src/rethink/logger.py
 src/rethink/regex.py
 src/rethink/run.py
 src/rethink/utils.py
@@ -34,15 +35,14 @@
 src/rethink/controllers/search/node_search.py
 src/rethink/controllers/user/__init__.py
 src/rethink/controllers/user/password.py
 src/rethink/controllers/user/user_ops.py
 src/rethink/controllers/verify/__init__.py
 src/rethink/controllers/verify/v_captcha.py
 src/rethink/core/__init__.py
-src/rethink/core/node.py
 src/rethink/core/search.py
 src/rethink/core/user.py
 src/rethink/core/files/__init__.py
 src/rethink/core/files/get.py
 src/rethink/core/files/saver.py
 src/rethink/core/files/upload.py
 src/rethink/core/files/importing/__init__.py
@@ -51,14 +51,18 @@
 src/rethink/core/files/importing/async_tasks/obsidian/__init__.py
 src/rethink/core/files/importing/async_tasks/obsidian/ops.py
 src/rethink/core/files/importing/async_tasks/obsidian/task.py
 src/rethink/core/files/importing/async_tasks/text/__init__.py
 src/rethink/core/files/importing/async_tasks/text/task.py
 src/rethink/core/files/importing/sync_tasks/__init__.py
 src/rethink/core/files/importing/sync_tasks/editor.py
+src/rethink/core/node/__init__.py
+src/rethink/core/node/backup.py
+src/rethink/core/node/node.py
+src/rethink/core/node/node_utils.py
 src/rethink/core/verify/__init__.py
 src/rethink/core/verify/email.py
 src/rethink/core/verify/verification.py
 src/rethink/depend/__init__.py
 src/rethink/depend/mongita/__init__.py
 src/rethink/depend/mongita/collection.py
 src/rethink/depend/mongita/command_cursor.py
@@ -302,14 +306,15 @@
 src/rethink/dist-local/img/loading.gif
 src/rethink/dist-local/img/menu.svg
 src/rethink/dist-local/img/morvanQR.png
 src/rethink/dist-local/img/node.svg
 src/rethink/dist-local/img/plugin.svg
 src/rethink/dist-local/img/plus.svg
 src/rethink/dist-local/img/recentoutline.svg
+src/rethink/dist-local/img/restore.svg
 src/rethink/dist-local/img/return-arrow.svg
 src/rethink/dist-local/img/search.svg
 src/rethink/dist-local/img/sort.svg
 src/rethink/dist-local/img/tab.svg
 src/rethink/dist-local/img/text.svg
 src/rethink/dist-local/img/three-dots-vertical.svg
 src/rethink/dist-local/img/tick.svg
@@ -355,14 +360,17 @@
 src/rethink/routes/oauth.py
 src/rethink/routes/plugin.py
 src/rethink/routes/search.py
 src/rethink/routes/trash.py
 src/rethink/routes/user.py
 src/rethink/routes/utils.py
 src/rethink/routes/verification.py
+src/rethink/version_manager/__init__.py
+src/rethink/version_manager/migrate.py
+src/rethink/version_manager/recover.py
 src/rethink_note.egg-info/PKG-INFO
 src/rethink_note.egg-info/SOURCES.txt
 src/rethink_note.egg-info/dependency_links.txt
 src/rethink_note.egg-info/requires.txt
 src/rethink_note.egg-info/top_level.txt
 tests/test_api.py
 tests/test_auth.py
@@ -372,8 +380,9 @@
 tests/test_data_restore.py
 tests/test_plugins.py
 tests/test_run.py
 tests/test_search_es.py
 tests/test_search_local.py
 tests/test_sso.py
 tests/test_utils.py
-tests/test_verification.py
+tests/test_verification.py
+tests/test_version_manager.py
```

### Comparing `rethink-note-0.2.3/tests/test_api.py` & `rethink-note-0.2.4/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_auth.py` & `rethink-note-0.2.4/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_core_files_obsidian.py` & `rethink-note-0.2.4/tests/test_core_files_obsidian.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_core_local.py` & `rethink-note-0.2.4/tests/test_core_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import shutil
+import time
 import unittest
 from io import BytesIO
 from pathlib import Path
 from textwrap import dedent
 from unittest.mock import patch
 
 import httpx
@@ -131,15 +132,14 @@
         )
 
         self.assertEqual(const.Code.OK, code)
         self.assertEqual("createdAt", u["lastState"]["nodeDisplaySortKey"])
         used_space = u["usedSpace"]
         n, _, code = await core.node.update(uid=self.uid, nid=node["id"], md="title2\nbody2")
         self.assertEqual(const.Code.OK, code)
-        self.assertEqual(const.Code.OK, code)
         self.assertEqual("title2", n["title"])
         self.assertEqual("title2\nbody2", n["md"])
         self.assertEqual(const.NodeType.MARKDOWN.value, n["type"])
 
         u, code = await core.user.get(self.uid)
         self.assertEqual(const.Code.OK, code)
         self.assertEqual(used_space + (
@@ -460,7 +460,28 @@
             u, code = await core.user.get(self.uid)
             self.assertEqual(const.Code.OK, code)
             now = u["usedSpace"] - base_used_space
             if now < 0:
                 now = 0
                 base_used_space = 0
             self.assertAlmostEqual(value, now, msg=f"delta: {delta}, value: {value}")
+
+    async def test_node_version(self):
+        node, code = await core.node.add(
+            uid=self.uid, md="[title](/qqq)\nbody", type_=const.NodeType.MARKDOWN.value
+        )
+        self.assertEqual(const.Code.OK, code)
+        md_path = Path(__file__).parent / "tmp" / ".data" / "md" / (node["id"] + ".md")
+        self.assertTrue(md_path.exists())
+
+        time.sleep(1)
+
+        n, _, code = await core.node.update(uid=self.uid, nid=node["id"], md="title2\nbody2")
+        self.assertEqual(const.Code.OK, code)
+        hist_dir = Path(__file__).parent / "tmp" / ".data" / "md" / "hist" / node["id"]
+        self.assertEqual(1, len(list(hist_dir.glob("*.md"))))
+
+        time.sleep(1)
+
+        n, _, code = await core.node.update(uid=self.uid, nid=node["id"], md="title2\nbody3")
+        self.assertEqual(const.Code.OK, code)
+        self.assertEqual(2, len(list(hist_dir.glob("*.md"))))
```

### Comparing `rethink-note-0.2.3/tests/test_core_remote.py` & `rethink-note-0.2.4/tests/test_core_remote.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import unittest
 from textwrap import dedent
+from unittest.mock import patch
 
 import elastic_transport
 import pymongo.errors
 from bson import ObjectId
 
 from rethink import const, config, core
 from rethink.controllers.auth import register_user
@@ -148,15 +149,30 @@
         code = await core.user.disable(uid="ssaa")
         self.assertEqual(const.Code.OPERATION_FAILED, code)
 
         code = await core.user.delete(uid=_id)
         self.assertEqual(const.Code.OK, code)
 
     @utils.skip_no_connect
-    async def test_node(self):
+    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("rethink.core.node.backup.__remove_md_from_cos")
+    @patch("rethink.core.node.backup.__get_md_from_cos")
+    @patch("rethink.core.node.backup.__save_md_to_cos")
+    async def test_node(
+            self,
+            mock_save_md_to_cos,
+            mock_get_md_from_cos,
+            mock_remove_md_from_cos,
+            mock_remove_md_all_versions_from_cos,
+    ):
+        mock_save_md_to_cos.return_value = const.Code.OK
+        mock_get_md_from_cos.return_value = ("", const.Code.OK)
+        mock_remove_md_from_cos.return_value = const.Code.OK
+        mock_remove_md_all_versions_from_cos.return_value = const.Code.OK
+
         u, code = await core.user.get(self.uid)
         self.assertEqual(const.Code.OK, code)
         used_space = u["usedSpace"]
         node, code = await core.node.add(
             uid=self.uid, md="title\ntext", type_=const.NodeType.MARKDOWN.value
         )
         self.assertEqual(const.Code.OK, code)
@@ -209,15 +225,30 @@
         self.assertEqual(used_space - len(node["md"].encode("utf-8")), u["usedSpace"])
 
         nodes, total = await core.node.core_nodes(self.uid, 0, 10)
         self.assertEqual(2, len(nodes))
         self.assertEqual(2, total)
 
     @utils.skip_no_connect
-    async def test_parse_at(self):
+    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("rethink.core.node.backup.__remove_md_from_cos")
+    @patch("rethink.core.node.backup.__get_md_from_cos")
+    @patch("rethink.core.node.backup.__save_md_to_cos")
+    async def test_parse_at(
+            self,
+            mock_save_md_to_cos,
+            mock_get_md_from_cos,
+            mock_remove_md_from_cos,
+            mock_remove_md_all_versions_from_cos,
+    ):
+        mock_save_md_to_cos.return_value = const.Code.OK
+        mock_get_md_from_cos.return_value = ("", const.Code.OK)
+        mock_remove_md_from_cos.return_value = const.Code.OK
+        mock_remove_md_all_versions_from_cos.return_value = const.Code.OK
+
         nid1, _ = await core.node.add(
             uid=self.uid, md="c", type_=const.NodeType.MARKDOWN.value,
         )
         nid2, _ = await core.node.add(
             uid=self.uid, md="我133", type_=const.NodeType.MARKDOWN.value,
         )
         md = dedent(
@@ -311,15 +342,29 @@
 
         await client.search.refresh()
         nodes, total = await client.search.search(self.uid)
         self.assertEqual(4, len(nodes))
         self.assertEqual(4, total)
 
     @utils.skip_no_connect
-    async def test_batch(self):
+    @patch("rethink.core.node.backup.__remove_md_all_versions_from_cos")
+    @patch("rethink.core.node.backup.__remove_md_from_cos")
+    @patch("rethink.core.node.backup.__get_md_from_cos")
+    @patch("rethink.core.node.backup.__save_md_to_cos")
+    async def test_batch(
+            self,
+            mock_save_md_to_cos,
+            mock_get_md_from_cos,
+            mock_remove_md_from_cos,
+            mock_remove_md_all_versions_from_cos,
+    ):
+        mock_save_md_to_cos.return_value = const.Code.OK
+        mock_get_md_from_cos.return_value = ("", const.Code.OK)
+        mock_remove_md_from_cos.return_value = const.Code.OK
+        mock_remove_md_all_versions_from_cos.return_value = const.Code.OK
         ns = []
         for i in range(10):
             n, code = await core.node.add(
                 uid=self.uid, md=f"title{i}\ntext", type_=const.NodeType.MARKDOWN.value
             )
             self.assertEqual(const.Code.OK, code)
             ns.append(n)
```

### Comparing `rethink-note-0.2.3/tests/test_data_restore.py` & `rethink-note-0.2.4/tests/test_data_restore.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_plugins.py` & `rethink-note-0.2.4/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_run.py` & `rethink-note-0.2.4/tests/test_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,18 @@
         shutil.rmtree(str(cls.path), ignore_errors=True)
         config.get_settings.cache_clear()
 
     def test_run(self):
         port = 8001
 
         for _ in range(2):
-            p = multiprocessing.Process(target=rethink.run, kwargs={"path": self.path, "port": port, "language": "zh"})
+            p = multiprocessing.Process(target=rethink.run, kwargs={
+                "path": self.path, "port": port, "language": "zh", "headless": True,
+                "debug": False,
+            })
             p.start()
             # p.join()
             while True:
                 sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 sock.settimeout(2)
                 result = sock.connect_ex(('127.0.0.1', port))
                 sock.close()
```

### Comparing `rethink-note-0.2.3/tests/test_search_es.py` & `rethink-note-0.2.4/tests/test_search_es.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_search_local.py` & `rethink-note-0.2.4/tests/test_search_local.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_sso.py` & `rethink-note-0.2.4/tests/test_sso.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_utils.py` & `rethink-note-0.2.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rethink-note-0.2.3/tests/test_verification.py` & `rethink-note-0.2.4/tests/test_verification.py`

 * *Files identical despite different names*

