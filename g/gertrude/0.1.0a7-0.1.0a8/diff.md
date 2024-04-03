# Comparing `tmp/gertrude-0.1.0a7.tar.gz` & `tmp/gertrude-0.1.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gertrude-0.1.0a7.tar", max compression
+gzip compressed data, was "gertrude-0.1.0a8.tar", max compression
```

## Comparing `gertrude-0.1.0a7.tar` & `gertrude-0.1.0a8.tar`

### file list

```diff
@@ -1,100 +1,100 @@
--rw-r--r--   0        0        0      848 2023-11-17 07:54:27.301099 gertrude-0.1.0a7/gertrude/__init__.py
--rw-r--r--   0        0        0      747 2023-10-31 11:12:22.117447 gertrude-0.1.0a7/gertrude/application/__init__.py
--rw-r--r--   0        0        0     3521 2023-11-24 06:54:06.819760 gertrude-0.1.0a7/gertrude/application/projectors.py
--rw-r--r--   0        0        0      753 2023-10-11 06:51:22.846029 gertrude-0.1.0a7/gertrude/application/use_cases/__init__.py
--rw-r--r--   0        0        0     3460 2023-11-17 17:20:01.478255 gertrude-0.1.0a7/gertrude/application/use_cases/assign_task.py
--rw-r--r--   0        0        0     4163 2023-11-08 17:38:51.165279 gertrude-0.1.0a7/gertrude/application/use_cases/capture_task.py
--rw-r--r--   0        0        0     3164 2023-11-17 13:36:48.242411 gertrude-0.1.0a7/gertrude/application/use_cases/create_project.py
--rw-r--r--   0        0        0     2912 2023-11-21 16:15:46.893257 gertrude-0.1.0a7/gertrude/application/use_cases/delegate_task.py
--rw-r--r--   0        0        0     2299 2023-11-17 13:39:36.304274 gertrude-0.1.0a7/gertrude/application/use_cases/display_project.py
--rw-r--r--   0        0        0     2498 2023-11-08 12:30:54.734050 gertrude-0.1.0a7/gertrude/application/use_cases/do_task.py
--rw-r--r--   0        0        0     2527 2023-11-08 12:30:54.774050 gertrude-0.1.0a7/gertrude/application/use_cases/eliminate_task.py
--rw-r--r--   0        0        0     2513 2023-11-08 12:30:54.766050 gertrude-0.1.0a7/gertrude/application/use_cases/file_task.py
--rw-r--r--   0        0        0     2510 2023-11-08 12:30:54.766050 gertrude-0.1.0a7/gertrude/application/use_cases/incubate_task.py
--rw-r--r--   0        0        0     1252 2023-11-14 06:54:49.917520 gertrude-0.1.0a7/gertrude/application/use_cases/list_projects.py
--rw-r--r--   0        0        0     1735 2023-11-14 06:54:49.917520 gertrude-0.1.0a7/gertrude/application/use_cases/list_tasks.py
--rw-r--r--   0        0        0     2532 2023-11-08 12:30:54.750050 gertrude-0.1.0a7/gertrude/application/use_cases/postpone_task.py
--rw-r--r--   0        0        0     2525 2023-11-21 16:47:19.916863 gertrude-0.1.0a7/gertrude/application/use_cases/reclaim_task.py
--rw-r--r--   0        0        0     3111 2023-11-17 06:32:24.930899 gertrude-0.1.0a7/gertrude/application/use_cases/schedule_task.py
--rw-r--r--   0        0        0     2844 2023-11-24 06:54:06.819760 gertrude-0.1.0a7/gertrude/application/use_cases/update_task.py
--rw-r--r--   0        0        0      977 2023-11-03 15:10:36.959717 gertrude-0.1.0a7/gertrude/configuration/__init__.py
--rw-r--r--   0        0        0     1105 2023-11-03 15:10:36.959717 gertrude-0.1.0a7/gertrude/configuration/cli.py
--rw-r--r--   0        0        0     1035 2023-11-03 15:10:36.991717 gertrude-0.1.0a7/gertrude/configuration/wsgi.py
--rw-r--r--   0        0        0      753 2023-10-11 06:51:22.806029 gertrude-0.1.0a7/gertrude/domain/__init__.py
--rw-r--r--   0        0        0      747 2023-10-31 10:17:24.097292 gertrude-0.1.0a7/gertrude/domain/project_management/__init__.py
--rw-r--r--   0        0        0      913 2023-11-17 10:12:46.893906 gertrude-0.1.0a7/gertrude/domain/project_management/entities.py
--rw-r--r--   0        0        0     1140 2023-11-17 13:22:30.105315 gertrude-0.1.0a7/gertrude/domain/project_management/repositories.py
--rw-r--r--   0        0        0     1204 2023-11-17 10:12:46.893906 gertrude-0.1.0a7/gertrude/domain/project_management/value_objects.py
--rw-r--r--   0        0        0      753 2023-10-11 06:51:22.806029 gertrude-0.1.0a7/gertrude/domain/task_management/__init__.py
--rw-r--r--   0        0        0     1050 2023-10-31 16:42:33.175971 gertrude-0.1.0a7/gertrude/domain/task_management/dto.py
--rw-r--r--   0        0        0     9550 2023-11-24 06:54:06.819760 gertrude-0.1.0a7/gertrude/domain/task_management/entities.py
--rw-r--r--   0        0        0     1004 2023-11-22 07:26:17.415262 gertrude-0.1.0a7/gertrude/domain/task_management/enums.py
--rw-r--r--   0        0        0     1836 2023-11-24 06:54:06.819760 gertrude-0.1.0a7/gertrude/domain/task_management/events.py
--rw-r--r--   0        0        0     1190 2023-11-17 06:32:24.930899 gertrude-0.1.0a7/gertrude/domain/task_management/exceptions.py
--rw-r--r--   0        0        0     1041 2023-11-14 06:54:49.921520 gertrude-0.1.0a7/gertrude/domain/task_management/projections.py
--rw-r--r--   0        0        0     1500 2023-11-14 06:54:49.921520 gertrude-0.1.0a7/gertrude/domain/task_management/repositories.py
--rw-r--r--   0        0        0     1213 2023-11-17 06:32:24.930899 gertrude-0.1.0a7/gertrude/domain/task_management/services.py
--rw-r--r--   0        0        0     1392 2023-11-21 14:57:52.177916 gertrude-0.1.0a7/gertrude/domain/task_management/value_objects.py
--rw-r--r--   0        0        0      753 2023-10-11 06:51:22.814029 gertrude-0.1.0a7/gertrude/infrastructure/__init__.py
--rw-r--r--   0        0        0     3133 2023-11-17 07:54:27.305099 gertrude-0.1.0a7/gertrude/infrastructure/click/__init__.py
--rw-r--r--   0        0        0     2995 2023-11-24 07:52:26.674003 gertrude-0.1.0a7/gertrude/infrastructure/flask/__init__.py
--rw-r--r--   0        0        0     1087 2023-10-30 12:03:53.411816 gertrude-0.1.0a7/gertrude/infrastructure/flask/aliases/__init__.py
--rw-r--r--   0        0        0     2040 2023-11-15 12:25:11.103410 gertrude-0.1.0a7/gertrude/infrastructure/flask/auth/__init__.py
--rw-r--r--   0        0        0     1642 2023-11-03 15:10:36.991717 gertrude-0.1.0a7/gertrude/infrastructure/flask/ip/__init__.py
--rw-r--r--   0        0        0     7265 2023-11-24 12:40:27.566932 gertrude-0.1.0a7/gertrude/infrastructure/flask/presenters.py
--rw-r--r--   0        0        0     2293 2023-11-24 12:47:39.177634 gertrude-0.1.0a7/gertrude/infrastructure/flask/projects/__init__.py
--rw-r--r--   0        0        0     3270 2023-11-17 06:32:24.930899 gertrude-0.1.0a7/gertrude/infrastructure/flask/services.py
--rw-r--r--   0        0        0    73117 2023-10-30 12:03:53.411816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/font-awesome@5.14.0.css
--rw-r--r--   0        0        0   150303 2023-11-21 17:26:29.578518 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/styles.css
--rw-r--r--   0        0        0   204232 2023-11-21 17:26:29.578518 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/styles.css.map
--rw-r--r--   0        0        0    46044 1985-10-26 08:15:00.000000 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/js/htmx@1.9.6.min.js
--rw-r--r--   0        0        0   100369 1985-10-26 08:15:00.000000 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/js/hyperscript@0.9.12.min.js
--rw-r--r--   0        0        0   186112 2023-10-30 12:03:53.415816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   107460 2023-10-30 12:03:53.415816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    62048 2023-10-30 12:03:53.415816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25096 2023-10-30 12:03:53.419816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   397728 2023-10-30 12:03:53.423816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   150472 2023-10-30 12:03:53.423816 gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0     7646 2023-11-24 12:47:39.177634 gertrude-0.1.0a7/gertrude/infrastructure/flask/tasks/__init__.py
--rw-r--r--   0        0        0     2078 2023-11-21 13:18:23.707722 gertrude-0.1.0a7/gertrude/infrastructure/flask/utils.py
--rw-r--r--   0        0        0     1735 2023-11-24 07:52:26.678003 gertrude-0.1.0a7/gertrude/infrastructure/settings.py
--rw-r--r--   0        0        0      747 2023-10-11 06:51:22.838029 gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     5194 2023-11-24 06:54:06.823760 gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/projections.py
--rw-r--r--   0        0        0     2180 2023-11-17 13:23:12.036789 gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/repositories.py
--rw-r--r--   0        0        0      753 2023-10-11 06:51:22.838029 gertrude-0.1.0a7/gertrude/interfaces/__init__.py
--rw-r--r--   0        0        0     5630 2023-11-24 06:54:06.823760 gertrude-0.1.0a7/gertrude/interfaces/from_base_types.py
--rw-r--r--   0        0        0     1716 2023-10-30 12:03:53.423816 gertrude-0.1.0a7/gertrude/interfaces/l10n/__init__.py
--rw-r--r--   0        0        0    11497 2023-11-24 10:35:32.359133 gertrude-0.1.0a7/gertrude/interfaces/l10n/en-GB/main.ftl
--rw-r--r--   0        0        0    12384 2023-11-24 06:54:06.823760 gertrude-0.1.0a7/gertrude/interfaces/l10n/fr-FR/main.ftl
--rw-r--r--   0        0        0     1806 2023-11-21 13:18:23.711722 gertrude-0.1.0a7/gertrude/interfaces/to_http/__init__.py
--rw-r--r--   0        0        0     4547 2023-11-24 07:52:26.678003 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/__init__.py
--rw-r--r--   0        0        0     4789 2023-11-24 10:35:32.403132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/fragment.py
--rw-r--r--   0        0        0     5425 2023-11-24 07:52:26.678003 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/page.py
--rw-r--r--   0        0        0     3860 2023-11-24 12:40:27.566932 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/page_or_fragment.py
--rw-r--r--   0        0        0     1399 2023-11-24 06:54:06.827760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/auth/login.pug
--rw-r--r--   0        0        0      952 2023-11-24 06:54:06.827760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/error.pug
--rw-r--r--   0        0        0     1782 2023-11-24 12:40:27.566932 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/layout.pug
--rw-r--r--   0        0        0     3762 2023-11-24 11:47:22.362280 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/actions.pug
--rw-r--r--   0        0        0     1116 2023-10-31 07:20:21.878690 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
--rw-r--r--   0        0        0     2492 2023-11-24 11:47:22.362280 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/list_of_tasks.pug
--rw-r--r--   0        0        0     4439 2023-11-24 12:47:39.177634 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/navbar.pug
--rw-r--r--   0        0        0     2188 2023-11-24 06:54:06.827760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/create.pug
--rw-r--r--   0        0        0     2070 2023-11-24 06:54:06.827760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/display.pug
--rw-r--r--   0        0        0     1762 2023-11-24 06:54:06.827760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/list.pug
--rw-r--r--   0        0        0     2709 2023-11-24 10:35:32.371132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/assign.pug
--rw-r--r--   0        0        0     4031 2023-11-24 10:35:32.383132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/capture.pug
--rw-r--r--   0        0        0     2532 2023-11-24 10:35:32.375132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/delegate.pug
--rw-r--r--   0        0        0     4651 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/display.pug
--rw-r--r--   0        0        0     1306 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/inbox.pug
--rw-r--r--   0        0        0     1943 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/index.pug
--rw-r--r--   0        0        0     1387 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/next.pug
--rw-r--r--   0        0        0     1280 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/organize.pug
--rw-r--r--   0        0        0     2426 2023-11-24 10:35:32.375132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/schedule.pug
--rw-r--r--   0        0        0     1192 2023-11-24 10:35:32.403132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/scheduled.pug
--rw-r--r--   0        0        0     1185 2023-11-24 10:35:32.403132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/someday.pug
--rw-r--r--   0        0        0     3386 2023-11-24 10:35:32.375132 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/update.pug
--rw-r--r--   0        0        0     1467 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/waiting.pug
--rw-r--r--   0        0        0    20860 2023-11-24 06:54:06.831760 gertrude-0.1.0a7/gertrude/interfaces/to_http/presenters.py
--rw-r--r--   0        0        0        0 2022-11-30 09:37:09.781149 gertrude-0.1.0a7/gertrude/py.typed
--rw-r--r--   0        0        0     1645 2023-11-24 16:42:17.752409 gertrude-0.1.0a7/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 gertrude-0.1.0a7/PKG-INFO
+-rw-r--r--   0        0        0      848 2023-11-17 07:54:27.301099 gertrude-0.1.0a8/gertrude/__init__.py
+-rw-r--r--   0        0        0      747 2023-10-31 11:12:22.117447 gertrude-0.1.0a8/gertrude/application/__init__.py
+-rw-r--r--   0        0        0     3521 2023-11-24 06:54:06.819760 gertrude-0.1.0a8/gertrude/application/projectors.py
+-rw-r--r--   0        0        0      753 2023-10-11 06:51:22.846029 gertrude-0.1.0a8/gertrude/application/use_cases/__init__.py
+-rw-r--r--   0        0        0     3460 2023-11-17 17:20:01.478255 gertrude-0.1.0a8/gertrude/application/use_cases/assign_task.py
+-rw-r--r--   0        0        0     4163 2023-11-08 17:38:51.165279 gertrude-0.1.0a8/gertrude/application/use_cases/capture_task.py
+-rw-r--r--   0        0        0     3164 2023-11-17 13:36:48.242411 gertrude-0.1.0a8/gertrude/application/use_cases/create_project.py
+-rw-r--r--   0        0        0     2912 2023-11-21 16:15:46.893257 gertrude-0.1.0a8/gertrude/application/use_cases/delegate_task.py
+-rw-r--r--   0        0        0     2299 2023-11-17 13:39:36.304274 gertrude-0.1.0a8/gertrude/application/use_cases/display_project.py
+-rw-r--r--   0        0        0     2498 2023-11-08 12:30:54.734050 gertrude-0.1.0a8/gertrude/application/use_cases/do_task.py
+-rw-r--r--   0        0        0     2527 2023-11-08 12:30:54.774050 gertrude-0.1.0a8/gertrude/application/use_cases/eliminate_task.py
+-rw-r--r--   0        0        0     2513 2023-11-08 12:30:54.766050 gertrude-0.1.0a8/gertrude/application/use_cases/file_task.py
+-rw-r--r--   0        0        0     2510 2023-11-08 12:30:54.766050 gertrude-0.1.0a8/gertrude/application/use_cases/incubate_task.py
+-rw-r--r--   0        0        0     1252 2023-11-14 06:54:49.917520 gertrude-0.1.0a8/gertrude/application/use_cases/list_projects.py
+-rw-r--r--   0        0        0     1735 2023-11-14 06:54:49.917520 gertrude-0.1.0a8/gertrude/application/use_cases/list_tasks.py
+-rw-r--r--   0        0        0     2532 2023-11-08 12:30:54.750050 gertrude-0.1.0a8/gertrude/application/use_cases/postpone_task.py
+-rw-r--r--   0        0        0     2525 2023-11-21 16:47:19.916863 gertrude-0.1.0a8/gertrude/application/use_cases/reclaim_task.py
+-rw-r--r--   0        0        0     3111 2023-11-17 06:32:24.930899 gertrude-0.1.0a8/gertrude/application/use_cases/schedule_task.py
+-rw-r--r--   0        0        0     2844 2023-11-24 06:54:06.819760 gertrude-0.1.0a8/gertrude/application/use_cases/update_task.py
+-rw-r--r--   0        0        0      977 2023-11-03 15:10:36.959717 gertrude-0.1.0a8/gertrude/configuration/__init__.py
+-rw-r--r--   0        0        0     1105 2023-11-03 15:10:36.959717 gertrude-0.1.0a8/gertrude/configuration/cli.py
+-rw-r--r--   0        0        0     1035 2023-11-03 15:10:36.991717 gertrude-0.1.0a8/gertrude/configuration/wsgi.py
+-rw-r--r--   0        0        0      753 2023-10-11 06:51:22.806029 gertrude-0.1.0a8/gertrude/domain/__init__.py
+-rw-r--r--   0        0        0      747 2023-10-31 10:17:24.097292 gertrude-0.1.0a8/gertrude/domain/project_management/__init__.py
+-rw-r--r--   0        0        0      913 2023-11-17 10:12:46.893906 gertrude-0.1.0a8/gertrude/domain/project_management/entities.py
+-rw-r--r--   0        0        0     1140 2023-11-17 13:22:30.105315 gertrude-0.1.0a8/gertrude/domain/project_management/repositories.py
+-rw-r--r--   0        0        0     1204 2023-11-17 10:12:46.893906 gertrude-0.1.0a8/gertrude/domain/project_management/value_objects.py
+-rw-r--r--   0        0        0      753 2023-10-11 06:51:22.806029 gertrude-0.1.0a8/gertrude/domain/task_management/__init__.py
+-rw-r--r--   0        0        0     1050 2023-10-31 16:42:33.175971 gertrude-0.1.0a8/gertrude/domain/task_management/dto.py
+-rw-r--r--   0        0        0     9550 2023-11-24 06:54:06.819760 gertrude-0.1.0a8/gertrude/domain/task_management/entities.py
+-rw-r--r--   0        0        0     1004 2023-11-22 07:26:17.415262 gertrude-0.1.0a8/gertrude/domain/task_management/enums.py
+-rw-r--r--   0        0        0     1836 2023-11-24 06:54:06.819760 gertrude-0.1.0a8/gertrude/domain/task_management/events.py
+-rw-r--r--   0        0        0     1190 2023-11-17 06:32:24.930899 gertrude-0.1.0a8/gertrude/domain/task_management/exceptions.py
+-rw-r--r--   0        0        0     1041 2023-11-14 06:54:49.921520 gertrude-0.1.0a8/gertrude/domain/task_management/projections.py
+-rw-r--r--   0        0        0     1500 2023-11-14 06:54:49.921520 gertrude-0.1.0a8/gertrude/domain/task_management/repositories.py
+-rw-r--r--   0        0        0     1213 2023-11-17 06:32:24.930899 gertrude-0.1.0a8/gertrude/domain/task_management/services.py
+-rw-r--r--   0        0        0     1392 2023-11-21 14:57:52.177916 gertrude-0.1.0a8/gertrude/domain/task_management/value_objects.py
+-rw-r--r--   0        0        0      753 2023-10-11 06:51:22.814029 gertrude-0.1.0a8/gertrude/infrastructure/__init__.py
+-rw-r--r--   0        0        0     3133 2023-11-17 07:54:27.305099 gertrude-0.1.0a8/gertrude/infrastructure/click/__init__.py
+-rw-r--r--   0        0        0     2995 2023-11-24 07:52:26.674003 gertrude-0.1.0a8/gertrude/infrastructure/flask/__init__.py
+-rw-r--r--   0        0        0     1087 2023-10-30 12:03:53.411816 gertrude-0.1.0a8/gertrude/infrastructure/flask/aliases/__init__.py
+-rw-r--r--   0        0        0     2040 2023-11-15 12:25:11.103410 gertrude-0.1.0a8/gertrude/infrastructure/flask/auth/__init__.py
+-rw-r--r--   0        0        0     1642 2023-11-03 15:10:36.991717 gertrude-0.1.0a8/gertrude/infrastructure/flask/ip/__init__.py
+-rw-r--r--   0        0        0     7265 2023-11-24 12:40:27.566932 gertrude-0.1.0a8/gertrude/infrastructure/flask/presenters.py
+-rw-r--r--   0        0        0     2293 2023-11-24 12:47:39.177634 gertrude-0.1.0a8/gertrude/infrastructure/flask/projects/__init__.py
+-rw-r--r--   0        0        0     3270 2023-11-17 06:32:24.930899 gertrude-0.1.0a8/gertrude/infrastructure/flask/services.py
+-rw-r--r--   0        0        0    73117 2023-10-30 12:03:53.411816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/font-awesome@5.14.0.css
+-rw-r--r--   0        0        0   150303 2023-11-21 17:26:29.578518 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/styles.css
+-rw-r--r--   0        0        0   204232 2023-11-21 17:26:29.578518 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/styles.css.map
+-rw-r--r--   0        0        0    46044 1985-10-26 08:15:00.000000 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/js/htmx@1.9.6.min.js
+-rw-r--r--   0        0        0   100369 1985-10-26 08:15:00.000000 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/js/hyperscript@0.9.12.min.js
+-rw-r--r--   0        0        0   186112 2023-10-30 12:03:53.415816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   107460 2023-10-30 12:03:53.415816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    62048 2023-10-30 12:03:53.415816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25096 2023-10-30 12:03:53.419816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   397728 2023-10-30 12:03:53.423816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   150472 2023-10-30 12:03:53.423816 gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0     7646 2023-11-24 12:47:39.177634 gertrude-0.1.0a8/gertrude/infrastructure/flask/tasks/__init__.py
+-rw-r--r--   0        0        0     2078 2023-11-21 13:18:23.707722 gertrude-0.1.0a8/gertrude/infrastructure/flask/utils.py
+-rw-r--r--   0        0        0     1735 2023-11-24 07:52:26.678003 gertrude-0.1.0a8/gertrude/infrastructure/settings.py
+-rw-r--r--   0        0        0      747 2023-10-11 06:51:22.838029 gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     5194 2023-11-24 06:54:06.823760 gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/projections.py
+-rw-r--r--   0        0        0     2180 2023-11-17 13:23:12.036789 gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/repositories.py
+-rw-r--r--   0        0        0      753 2023-10-11 06:51:22.838029 gertrude-0.1.0a8/gertrude/interfaces/__init__.py
+-rw-r--r--   0        0        0     5630 2023-11-24 06:54:06.823760 gertrude-0.1.0a8/gertrude/interfaces/from_base_types.py
+-rw-r--r--   0        0        0     1716 2023-10-30 12:03:53.423816 gertrude-0.1.0a8/gertrude/interfaces/l10n/__init__.py
+-rw-r--r--   0        0        0    11475 2023-11-24 16:57:03.981420 gertrude-0.1.0a8/gertrude/interfaces/l10n/en-GB/main.ftl
+-rw-r--r--   0        0        0    12362 2023-11-24 16:56:57.925496 gertrude-0.1.0a8/gertrude/interfaces/l10n/fr-FR/main.ftl
+-rw-r--r--   0        0        0     1806 2023-11-21 13:18:23.711722 gertrude-0.1.0a8/gertrude/interfaces/to_http/__init__.py
+-rw-r--r--   0        0        0     4547 2023-11-24 07:52:26.678003 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/__init__.py
+-rw-r--r--   0        0        0     4789 2023-11-24 10:35:32.403132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/fragment.py
+-rw-r--r--   0        0        0     5425 2023-11-24 07:52:26.678003 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/page.py
+-rw-r--r--   0        0        0     3860 2023-11-24 12:40:27.566932 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/page_or_fragment.py
+-rw-r--r--   0        0        0     1399 2023-11-24 06:54:06.827760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/auth/login.pug
+-rw-r--r--   0        0        0      952 2023-11-24 06:54:06.827760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/error.pug
+-rw-r--r--   0        0        0     1782 2023-11-24 12:40:27.566932 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/layout.pug
+-rw-r--r--   0        0        0     3762 2023-11-24 11:47:22.362280 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/actions.pug
+-rw-r--r--   0        0        0     1116 2023-10-31 07:20:21.878690 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/flash_messages.pug
+-rw-r--r--   0        0        0     2492 2023-11-24 11:47:22.362280 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/list_of_tasks.pug
+-rw-r--r--   0        0        0     4439 2023-11-24 12:47:39.177634 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/navbar.pug
+-rw-r--r--   0        0        0     2188 2023-11-24 06:54:06.827760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/create.pug
+-rw-r--r--   0        0        0     2070 2023-11-24 06:54:06.827760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/display.pug
+-rw-r--r--   0        0        0     1762 2023-11-24 06:54:06.827760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/list.pug
+-rw-r--r--   0        0        0     2709 2023-11-24 10:35:32.371132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/assign.pug
+-rw-r--r--   0        0        0     4031 2023-11-24 10:35:32.383132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/capture.pug
+-rw-r--r--   0        0        0     2532 2023-11-24 10:35:32.375132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/delegate.pug
+-rw-r--r--   0        0        0     4651 2023-11-24 06:54:06.831760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/display.pug
+-rw-r--r--   0        0        0     1307 2023-11-24 16:55:11.126824 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/inbox.pug
+-rw-r--r--   0        0        0     1943 2023-11-24 06:54:06.831760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/index.pug
+-rw-r--r--   0        0        0     1388 2023-11-24 16:55:17.094750 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/next.pug
+-rw-r--r--   0        0        0     1280 2023-11-24 06:54:06.831760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/organize.pug
+-rw-r--r--   0        0        0     2426 2023-11-24 10:35:32.375132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/schedule.pug
+-rw-r--r--   0        0        0     1192 2023-11-24 10:35:32.403132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/scheduled.pug
+-rw-r--r--   0        0        0     1185 2023-11-24 10:35:32.403132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/someday.pug
+-rw-r--r--   0        0        0     3386 2023-11-24 10:35:32.375132 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/update.pug
+-rw-r--r--   0        0        0     1467 2023-11-24 06:54:06.831760 gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/waiting.pug
+-rw-r--r--   0        0        0    20860 2023-11-24 06:54:06.831760 gertrude-0.1.0a8/gertrude/interfaces/to_http/presenters.py
+-rw-r--r--   0        0        0        0 2022-11-30 09:37:09.781149 gertrude-0.1.0a8/gertrude/py.typed
+-rw-r--r--   0        0        0     1645 2023-11-24 17:01:31.462096 gertrude-0.1.0a8/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 gertrude-0.1.0a8/PKG-INFO
```

### Comparing `gertrude-0.1.0a7/gertrude/__init__.py` & `gertrude-0.1.0a8/gertrude/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/__init__.py` & `gertrude-0.1.0a8/gertrude/application/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/projectors.py` & `gertrude-0.1.0a8/gertrude/application/projectors.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/__init__.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/assign_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/assign_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/capture_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/capture_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/create_project.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/create_project.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/delegate_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/delegate_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/display_project.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/display_project.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/do_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/do_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/eliminate_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/eliminate_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/file_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/file_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/incubate_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/incubate_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/list_projects.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/list_projects.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/list_tasks.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/list_tasks.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/postpone_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/postpone_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/reclaim_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/reclaim_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/schedule_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/schedule_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/application/use_cases/update_task.py` & `gertrude-0.1.0a8/gertrude/application/use_cases/update_task.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/configuration/__init__.py` & `gertrude-0.1.0a8/gertrude/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/configuration/cli.py` & `gertrude-0.1.0a8/gertrude/configuration/cli.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/configuration/wsgi.py` & `gertrude-0.1.0a8/gertrude/configuration/wsgi.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/__init__.py` & `gertrude-0.1.0a8/gertrude/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/project_management/__init__.py` & `gertrude-0.1.0a8/gertrude/domain/project_management/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/project_management/entities.py` & `gertrude-0.1.0a8/gertrude/domain/project_management/entities.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/project_management/repositories.py` & `gertrude-0.1.0a8/gertrude/domain/project_management/repositories.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/project_management/value_objects.py` & `gertrude-0.1.0a8/gertrude/domain/project_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/__init__.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/dto.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/dto.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/entities.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/entities.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/enums.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/enums.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/events.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/events.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/exceptions.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/projections.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/projections.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/repositories.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/repositories.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/services.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/services.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/domain/task_management/value_objects.py` & `gertrude-0.1.0a8/gertrude/domain/task_management/value_objects.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/click/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/click/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/aliases/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/aliases/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/auth/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/ip/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/ip/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/presenters.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/presenters.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/projects/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/services.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/services.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/font-awesome@5.14.0.css` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/font-awesome@5.14.0.css`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/styles.css` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/styles.css`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/css/styles.css.map` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/css/styles.css.map`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/js/htmx@1.9.6.min.js` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/js/htmx@1.9.6.min.js`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/js/hyperscript@0.9.12.min.js` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/js/hyperscript@0.9.12.min.js`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.ttf` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.woff2` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.ttf` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.woff2` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.ttf` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.woff2` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/static/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/tasks/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/flask/utils.py` & `gertrude-0.1.0a8/gertrude/infrastructure/flask/utils.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/settings.py` & `gertrude-0.1.0a8/gertrude/infrastructure/settings.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/__init__.py` & `gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/projections.py` & `gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/projections.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/infrastructure/sqlalchemy/repositories.py` & `gertrude-0.1.0a8/gertrude/infrastructure/sqlalchemy/repositories.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/__init__.py` & `gertrude-0.1.0a8/gertrude/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/from_base_types.py` & `gertrude-0.1.0a8/gertrude/interfaces/from_base_types.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/l10n/__init__.py` & `gertrude-0.1.0a8/gertrude/interfaces/l10n/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/l10n/en-GB/main.ftl` & `gertrude-0.1.0a8/gertrude/interfaces/l10n/en-GB/main.ftl`

 * *Files 1% similar despite different names*

```diff
@@ -170,20 +170,19 @@
 
 pages-tasks-inbox-title = Inbox
 pages-tasks-inbox-empty-html =
     <p>
         Your inbox is empty!
         <br />
         Find the next tasks to do on
-        <a href={ $link_next }>
+        <a href="{ $link_next }">
             <span>the next page</span>
                 <span class="icon-text">
                     <span class="icon">
-                        <span class="fas fa-chevron-circle-right>
-                        </span>
+                        <span class="fas fa-chevron-circle-right"></span>
                     </span>
                 </span>
             </span>
         </a>
     </p>
 
 pages-tasks-incubate-success = Task incubated!
```

#### html2text {}

```diff
@@ -90,17 +90,43 @@
 you want to do it somedayâ¦ pages-tasks-display-conditions-file = If you want
 to keep it for referenceâ¦ pages-tasks-display-conditions-eliminate = Elseâ¦
 pages-tasks-display-no-action = Nothing more can be done with this task! pages-
 tasks-do-success = Task marked as done! pages-tasks-eliminate-success = Task
 eliminated! pages-tasks-file-success = Task filed! pages-tasks-inbox-title =
 Inbox pages-tasks-inbox-empty-html =
 Your inbox is empty!
-Find the next tasks to do on link_next }> the next page $url_waiting }">
-waiting
-, _s_c_h_e_d_u_l_e_d_ and _s_o_m_e_d_a_y_ lists to find out what to do next.
+Find the next tasks to do on _t_h_e_ _n_e_x_t_ _p_a_g_e
+pages-tasks-incubate-success = Task incubated! pages-tasks-index-title =
+Welcome to { -project-name }! pages-tasks-index-subtitle = A task-management
+system. pages-tasks-index-introduction-html = The heartbeat of GTD is ffiivvee
+ssiimmppllee sstteeppss that apply order to chaos and provide you the space and structure
+to be more creative, strategic and focused. pages-tasks-index-capture-title =
+Capture â collect what has your attention pages-tasks-index-capture-
+description-html = Use an in-tray, notepad, digital list or voice recorder to
+capture everything that has your attention.
+Little, big, personal and professional â all your to-do's, projects, things
+to handle or finish. pages-tasks-index-clarify-title = Clarify â process what
+it means pages-tasks-index-clarify-description-html = Take everything that you
+capture and ask; is it actionable?
+If no, then trash it, incubate it, or file it as reference.
+If yes, decide the very next action required. If it will take less than two
+minutes, do it now. If not, delegate it if you can; or put it on a list to do
+when you can. pages-tasks-index-organize-title = Organize â put it where it
+belongs pages-tasks-index-organize-description-html = Put action reminders on
+the right lists. For example, create lists for the apropriate categories â
+calls to make, errands to run, emails to send, etc. pages-tasks-index-reflect-
+title = Reflect â review frequently pages-tasks-index-reflect-description-
+html = Look over your lists as often as necessary to trust your choices about
+what to do next. Do a weekly review to get clear, get current and creative.
+pages-tasks-index-engage-title = Engage â simply do pages-tasks-index-engage-
+description-html = Use your system to take appropriate actions with confidence.
+pages-tasks-next-title = Next pages-tasks-next-empty-html =
+Congratulations! Your list of things to do is empty!
+Reflect and review all your _w_a_i_t_i_n_g_ , _s_c_h_e_d_u_l_e_d_ and _s_o_m_e_d_a_y_ lists to find out
+what to do next.
 pages-tasks-postpone-success = Task postponed! pages-tasks-organize-title =
 Organize pages-tasks-organize-empty = No task to display. Change the filter or
 capture new ones! pages-tasks-reclaim-success = Task reclaimed! pages-tasks-
 schedule-title = Schedule task on a later date pages-tasks-schedule-date-label
 = Date pages-tasks-schedule-date-help = Date on which the task is scheduled to
 be done. pages-tasks-schedule-submit = Schedule pages-tasks-schedule-cancel =
 Cancel pages-tasks-schedule-success = Task scheduled! pages-tasks-scheduled-
```

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/l10n/fr-FR/main.ftl` & `gertrude-0.1.0a8/gertrude/interfaces/l10n/fr-FR/main.ftl`

 * *Files 0% similar despite different names*

```diff
@@ -170,20 +170,19 @@
 
 pages-tasks-inbox-title = { categories-inbox }
 pages-tasks-inbox-empty-html =
     <p>
         Votre boite de réception est vide !
         <br />
         Trouver la prochaine sur
-        <a href={ $link_next }>
+        <a href="{ $link_next }">
             <span>la page des tâches à réaliser</span>
                 <span class="icon-text">
                     <span class="icon">
-                        <span class="fas fa-chevron-circle-right>
-                        </span>
+                        <span class="fas fa-chevron-circle-right"></span>
                     </span>
                 </span>
             </span>
         </a>
     </p>
 
 pages-tasks-incubate-success = Tâche incubée !
```

#### html2text {}

```diff
@@ -97,17 +97,43 @@
 pages-tasks-display-conditions-file = Si vous voulez juste le garder pour
 rÃ©fÃ©renceâ¦ pages-tasks-display-conditions-eliminate = Sinonâ¦ pages-tasks-
 display-no-action = Il n'y a rien Ã  faire de plus pour cette tÃ¢cheÂ ! pages-
 tasks-do-success = TÃ¢che marquÃ©e comme rÃ©alisÃ©eÂ ! pages-tasks-eliminate-
 success = TÃ¢che Ã©liminÃ©eÂ ! pages-tasks-file-success = TÃ¢che classÃ©eÂ !
 pages-tasks-inbox-title = { categories-inbox } pages-tasks-inbox-empty-html =
 Votre boite de rÃ©ception est videÂ !
-Trouver la prochaine sur link_next }> la page des tÃ¢ches Ã  rÃ©aliser
-$url_waiting }"> dÃ©lÃ©guÃ©es
-, _p_r_o_g_r_a_m_m_Ã_©_e_s_ et _r_e_p_o_u_s_s_Ã_©_e_s_ pour trouver quoi faire ensuite.
+Trouver la prochaine sur _l_a_ _p_a_g_e_ _d_e_s_ _t_Ã_¢_c_h_e_s_ _Ã_ _ _r_Ã_©_a_l_i_s_e_r
+pages-tasks-incubate-success = TÃ¢che incubÃ©eÂ ! pages-tasks-index-title =
+Bienvenue sur { -project-name }Â ! pages-tasks-index-subtitle = Un systÃ¨me de
+gestion de tÃ¢ches. pages-tasks-index-introduction-html = The heartbeat of GTD
+is ffiivvee ssiimmppllee sstteeppss that apply order to chaos and provide you the space and
+structure to be more creative, strategic and focused. pages-tasks-index-
+capture-title = Capture â collect what has your attention pages-tasks-index-
+capture-description-html = Use an in-tray, notepad, digital list or voice
+recorder to capture everything that has your attention.
+Little, big, personal and professional â all your to-do's, projects, things
+to handle or finish. pages-tasks-index-clarify-title = Clarify â process what
+it means pages-tasks-index-clarify-description-html = Take everything that you
+capture and ask; is it actionable?
+If no, then trash it, incubate it, or file it as reference.
+If yes, decide the very next action required. If it will take less than two
+minutes, do it now. If not, delegate it if you can; or put it on a list to do
+when you can. pages-tasks-index-organize-title = Organize â put it where it
+belongs pages-tasks-index-organize-description-html = Put action reminders on
+the right lists. For example, create lists for the apropriate categories â
+calls to make, errands to run, emails to send, etc. pages-tasks-index-reflect-
+title = Reflect â review frequently pages-tasks-index-reflect-description-
+html = Look over your lists as often as necessary to trust your choices about
+what to do next. Do a weekly review to get clear, get current and creative.
+pages-tasks-index-engage-title = Engage â simply do pages-tasks-index-engage-
+description-html = Use your system to take appropriate actions with confidence.
+pages-tasks-next-title = Next pages-tasks-next-empty-html =
+FÃ©licitationsÂ ! Votre liste des choses Ã  faire est videÂ !
+RÃ©flÃ©chisser Ã  et passer en revue vos listes de tÃ¢ches _d_Ã_©_l_Ã_©_g_u_Ã_©_e_s_ ,
+_p_r_o_g_r_a_m_m_Ã_©_e_s_ et _r_e_p_o_u_s_s_Ã_©_e_s_ pour trouver quoi faire ensuite.
 pages-tasks-postpone-success = TÃ¢che marquÃ©e comme actionnable. pages-tasks-
 organize-title = Organiser pages-tasks-organize-empty = Il n'y a aucune tÃ¢che
 Ã  afficher. Changer les filtres ou capturez en de nouvelles. pages-tasks-
 reclaim-success = TÃ¢che rÃ©cupÃ©rÃ©eÂ ! pages-tasks-schedule-title =
 Programmer une tÃ¢che pour une date pages-tasks-schedule-date-label = Date
 pages-tasks-schedule-date-help = Date Ã  laquelle la tÃ¢che doit Ãªtre
 rÃ©alisÃ©e. pages-tasks-schedule-submit = Programmer pages-tasks-schedule-
```

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/__init__.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/__init__.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/__init__.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/fragment.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/fragment.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/page.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/page.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/page_or_fragment.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/page_or_fragment.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/auth/login.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/auth/login.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/error.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/error.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/layout.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/layout.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/actions.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/actions.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/flash_messages.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/flash_messages.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/mixins/list_of_tasks.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/mixins/list_of_tasks.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/navbar.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/navbar.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/create.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/create.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/display.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/display.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/projects/list.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/projects/list.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/assign.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/assign.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/capture.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/capture.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/delegate.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/delegate.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/display.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/display.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/inbox.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/inbox.pug`

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,8 @@
       )
         block tasks
           if tasks
             include mixins/list_of_tasks
             +list_of_tasks(tasks)
           else
             article.message.is-success
-              .message-body= _("pages-tasks-inbox-empty-html", link_next=url_for("tasks.next"))
+              .message-body!= _("pages-tasks-inbox-empty-html", link_next=url_for("tasks.next"))
```

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/index.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/index.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/next.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/next.pug`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
       )
         block tasks
           if tasks
             include mixins/list_of_tasks
             +list_of_tasks(tasks)
           else
             article.message.is-success
-              .message-body= _("pages-tasks-next-empty-html", url_waiting=url_for("tasks.waiting"), url_scheduled=url_for("tasks.scheduled"), url_someday=url_for("tasks.someday"))
+              .message-body!= _("pages-tasks-next-empty-html", url_waiting=url_for("tasks.waiting"), url_scheduled=url_for("tasks.scheduled"), url_someday=url_for("tasks.someday"))
```

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/organize.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/organize.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/schedule.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/schedule.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/scheduled.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/scheduled.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/someday.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/someday.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/update.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/update.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/as_html/templates/tasks/waiting.pug` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/as_html/templates/tasks/waiting.pug`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/gertrude/interfaces/to_http/presenters.py` & `gertrude-0.1.0a8/gertrude/interfaces/to_http/presenters.py`

 * *Files identical despite different names*

### Comparing `gertrude-0.1.0a7/pyproject.toml` & `gertrude-0.1.0a8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gertrude"
-version = "0.1.0a7"
+version = "0.1.0a8"
 description = "GTD done right"
 authors = ["Tanguy Le Carrour <tanguy@bioneland.org>"]
 license = "AGPL-3.0-or-later"
 
 include = [
     # Generated assets
     "gertrude/**/styles.css*",
```

### Comparing `gertrude-0.1.0a7/PKG-INFO` & `gertrude-0.1.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gertrude
-Version: 0.1.0a7
+Version: 0.1.0a8
 Summary: GTD done right
 License: AGPL-3.0-or-later
 Author: Tanguy Le Carrour
 Author-email: tanguy@bioneland.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
```

