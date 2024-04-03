# Comparing `tmp/aio-scrapy-2.0.8.tar.gz` & `tmp/aio-scrapy-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio-scrapy-2.0.8.tar", last modified: Wed Jan 17 07:14:06 2024, max compression
+gzip compressed data, was "aio-scrapy-2.0.9.tar", last modified: Wed Apr  3 06:32:05 2024, max compression
```

## Comparing `aio-scrapy-2.0.8.tar` & `aio-scrapy-2.0.9.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.323933 aio-scrapy-2.0.8/
--rw-rw-rw-   0        0        0     1088 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/LICENSE
--rw-rw-rw-   0        0        0      182 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6337 2024-01-17 07:14:06.322617 aio-scrapy-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     3855 2023-12-25 01:05:41.000000 aio-scrapy-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.319688 aio-scrapy-2.0.8/aio_scrapy.egg-info/
--rw-rw-rw-   0        0        0     6337 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4366 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      574 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-01-17 07:14:05.000000 aio-scrapy-2.0.8/aio_scrapy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.696017 aio-scrapy-2.0.8/aioscrapy/
--rw-rw-rw-   0        0        0        5 2024-01-17 07:13:53.000000 aio-scrapy-2.0.8/aioscrapy/VERSION
--rw-rw-rw-   0        0        0      858 2023-09-28 01:34:29.000000 aio-scrapy-2.0.8/aioscrapy/__init__.py
--rw-rw-rw-   0        0        0       80 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/__main__.py
--rw-rw-rw-   0        0        0     5159 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/cmdline.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.760279 aio-scrapy-2.0.8/aioscrapy/commands/
--rw-rw-rw-   0        0        0     4769 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/__init__.py
--rw-rw-rw-   0        0        0     1020 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/crawl.py
--rw-rw-rw-   0        0        0     5426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/genspider.py
--rw-rw-rw-   0        0        0      346 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/list.py
--rw-rw-rw-   0        0        0     2067 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/runspider.py
--rw-rw-rw-   0        0        0     1798 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/settings.py
--rw-rw-rw-   0        0        0     4001 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/startproject.py
--rw-rw-rw-   0        0        0      485 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/commands/version.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.775188 aio-scrapy-2.0.8/aioscrapy/core/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.792006 aio-scrapy-2.0.8/aioscrapy/core/downloader/
--rw-rw-rw-   0        0        0     9465 2024-01-15 09:49:33.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.830657 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/
--rw-rw-rw-   0        0        0     3198 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/__init__.py
--rw-rw-rw-   0        0        0     3942 2023-12-25 07:35:12.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/aiohttp.py
--rw-rw-rw-   0        0        0     3041 2023-09-27 08:43:17.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/httpx.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.833586 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/
--rw-rw-rw-   0        0        0     4160 2023-10-12 09:22:48.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/__init__.py
--rw-rw-rw-   0        0        0     1374 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/driverpool.py
--rw-rw-rw-   0        0        0     3530 2023-10-12 09:38:59.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/webdriver.py
--rw-rw-rw-   0        0        0     2228 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/pyhttpx.py
--rw-rw-rw-   0        0        0     1996 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/requests.py
--rw-rw-rw-   0        0        0    10925 2024-01-15 09:37:22.000000 aio-scrapy-2.0.8/aioscrapy/core/engine.py
--rw-rw-rw-   0        0        0     5737 2023-09-27 09:13:11.000000 aio-scrapy-2.0.8/aioscrapy/core/scheduler.py
--rw-rw-rw-   0        0        0    10304 2023-10-12 09:32:46.000000 aio-scrapy-2.0.8/aioscrapy/core/scraper.py
--rw-rw-rw-   0        0        0    10109 2023-12-22 04:04:27.000000 aio-scrapy-2.0.8/aioscrapy/crawler.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.845958 aio-scrapy-2.0.8/aioscrapy/db/
--rw-rw-rw-   0        0        0     2456 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/db/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/db/absmanager.py
--rw-rw-rw-   0        0        0     2745 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/db/aiomongo.py
--rw-rw-rw-   0        0        0     3799 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/db/aiomysql.py
--rw-rw-rw-   0        0        0     3213 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/db/aiopg.py
--rw-rw-rw-   0        0        0     5583 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/db/aiorabbitmq.py
--rw-rw-rw-   0        0        0     2966 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/db/aioredis.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.874426 aio-scrapy-2.0.8/aioscrapy/dupefilters/
--rw-rw-rw-   0        0        0      725 2023-09-13 03:12:08.000000 aio-scrapy-2.0.8/aioscrapy/dupefilters/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/dupefilters/disk.py
--rw-rw-rw-   0        0        0     5160 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/dupefilters/redis.py
--rw-rw-rw-   0        0        0     2027 2024-01-15 09:43:42.000000 aio-scrapy-2.0.8/aioscrapy/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.876482 aio-scrapy-2.0.8/aioscrapy/http/
--rw-rw-rw-   0        0        0      597 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/__init__.py
--rw-rw-rw-   0        0        0     1573 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/headers.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.909802 aio-scrapy-2.0.8/aioscrapy/http/request/
--rw-rw-rw-   0        0        0     7121 2023-09-26 06:37:06.000000 aio-scrapy-2.0.8/aioscrapy/http/request/__init__.py
--rw-rw-rw-   0        0        0     1382 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/request/form.py
--rw-rw-rw-   0        0        0     2051 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/request/json_request.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.944871 aio-scrapy-2.0.8/aioscrapy/http/response/
--rw-rw-rw-   0        0        0     6731 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/response/__init__.py
--rw-rw-rw-   0        0        0      303 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/response/html.py
--rw-rw-rw-   0        0        0     1051 2023-10-12 09:29:08.000000 aio-scrapy-2.0.8/aioscrapy/http/response/playwright.py
--rw-rw-rw-   0        0        0     9844 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/response/text.py
--rw-rw-rw-   0        0        0      300 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/http/response/xml.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.945847 aio-scrapy-2.0.8/aioscrapy/libs/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/libs/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.969621 aio-scrapy-2.0.8/aioscrapy/libs/downloader/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/__init__.py
--rw-rw-rw-   0        0        0      563 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/defaultheaders.py
--rw-rw-rw-   0        0        0      704 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/downloadtimeout.py
--rw-rw-rw-   0        0        0     1058 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/ja3fingerprint.py
--rw-rw-rw-   0        0        0     5082 2024-01-15 09:43:42.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/retry.py
--rw-rw-rw-   0        0        0     1376 2023-09-26 09:41:57.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/stats.py
--rw-rw-rw-   0        0        0      743 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/libs/downloader/useragent.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.030321 aio-scrapy-2.0.8/aioscrapy/libs/extensions/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/__init__.py
--rw-rw-rw-   0        0        0     2734 2023-09-22 10:41:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/closespider.py
--rw-rw-rw-   0        0        0     1820 2023-09-26 08:56:09.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/corestats.py
--rw-rw-rw-   0        0        0     1844 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/logstats.py
--rw-rw-rw-   0        0        0     5479 2023-10-20 01:51:59.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/metric.py
--rw-rw-rw-   0        0        0     3512 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/extensions/throttle.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.068922 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/
--rw-rw-rw-   0        0        0     5709 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/__init__.py
--rw-rw-rw-   0        0        0     2454 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/csv.py
--rw-rw-rw-   0        0        0     6284 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/execl.py
--rw-rw-rw-   0        0        0     2001 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/mongo.py
--rw-rw-rw-   0        0        0     1022 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/mysql.py
--rw-rw-rw-   0        0        0      990 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/pipelines/pg.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.082350 aio-scrapy-2.0.8/aioscrapy/libs/spider/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/__init__.py
--rw-rw-rw-   0        0        0     1938 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/depth.py
--rw-rw-rw-   0        0        0     1857 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/httperror.py
--rw-rw-rw-   0        0        0     2941 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/offsite.py
--rw-rw-rw-   0        0        0    13768 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/referer.py
--rw-rw-rw-   0        0        0     1151 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/libs/spider/urllength.py
--rw-rw-rw-   0        0        0     1867 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/link.py
--rw-rw-rw-   0        0        0     3028 2023-10-12 09:32:03.000000 aio-scrapy-2.0.8/aioscrapy/logformatter.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.090241 aio-scrapy-2.0.8/aioscrapy/middleware/
--rw-rw-rw-   0        0        0      396 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/middleware/__init__.py
--rw-rw-rw-   0        0        0     3410 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/middleware/absmanager.py
--rw-rw-rw-   0        0        0     3199 2023-09-26 06:48:29.000000 aio-scrapy-2.0.8/aioscrapy/middleware/downloader.py
--rw-rw-rw-   0        0        0      420 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/middleware/extension.py
--rw-rw-rw-   0        0        0      674 2023-09-19 03:48:43.000000 aio-scrapy-2.0.8/aioscrapy/middleware/itempipeline.py
--rw-rw-rw-   0        0        0     6361 2023-12-05 08:01:00.000000 aio-scrapy-2.0.8/aioscrapy/middleware/spider.py
--rw-rw-rw-   0        0        0     1603 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/process.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.125396 aio-scrapy-2.0.8/aioscrapy/proxy/
--rw-rw-rw-   0        0        0     1807 2024-01-15 08:08:24.000000 aio-scrapy-2.0.8/aioscrapy/proxy/__init__.py
--rw-rw-rw-   0        0        0     2711 2024-01-15 09:59:00.000000 aio-scrapy-2.0.8/aioscrapy/proxy/redis.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.135025 aio-scrapy-2.0.8/aioscrapy/queue/
--rw-rw-rw-   0        0        0     2037 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/queue/__init__.py
--rw-rw-rw-   0        0        0     3140 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/queue/memory.py
--rw-rw-rw-   0        0        0     2516 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/queue/rabbitmq.py
--rw-rw-rw-   0        0        0     4788 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/queue/redis.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.137054 aio-scrapy-2.0.8/aioscrapy/scrapyd/
--rw-rw-rw-   0        0        0       68 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/scrapyd/__init__.py
--rw-rw-rw-   0        0        0     1777 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/scrapyd/runner.py
--rw-rw-rw-   0        0        0      734 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/serializer.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.152994 aio-scrapy-2.0.8/aioscrapy/settings/
--rw-rw-rw-   0        0        0    15781 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/settings/__init__.py
--rw-rw-rw-   0        0        0     5432 2023-09-27 08:43:18.000000 aio-scrapy-2.0.8/aioscrapy/settings/default_settings.py
--rw-rw-rw-   0        0        0     2402 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/signalmanager.py
--rw-rw-rw-   0        0        0      610 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/signals.py
--rw-rw-rw-   0        0        0     3426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/spiderloader.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.163491 aio-scrapy-2.0.8/aioscrapy/spiders/
--rw-rw-rw-   0        0        0     3934 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/spiders/__init__.py
--rw-rw-rw-   0        0        0     2036 2023-12-05 07:56:11.000000 aio-scrapy-2.0.8/aioscrapy/statscollectors.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:05.560220 aio-scrapy-2.0.8/aioscrapy/templates/
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.164468 aio-scrapy-2.0.8/aioscrapy/templates/project/
--rw-rw-rw-   0        0        0      112 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/aioscrapy.cfg
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.178619 aio-scrapy-2.0.8/aioscrapy/templates/project/module/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/module/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-12-05 07:04:56.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/module/middlewares.py.tmpl
--rw-rw-rw-   0        0        0      164 2023-12-05 07:04:56.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/module/pipelines.py.tmpl
--rw-rw-rw-   0        0        0     1421 2023-12-05 07:11:48.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/module/settings.py.tmpl
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.189757 aio-scrapy-2.0.8/aioscrapy/templates/project/module/spiders/
--rw-rw-rw-   0        0        0      164 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/templates/project/module/spiders/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.191240 aio-scrapy-2.0.8/aioscrapy/templates/spiders/
--rw-rw-rw-   0        0        0      375 2023-12-05 07:11:48.000000 aio-scrapy-2.0.8/aioscrapy/templates/spiders/basic.tmpl
--rw-rw-rw-   0        0        0      942 2023-12-05 07:11:48.000000 aio-scrapy-2.0.8/aioscrapy/templates/spiders/single.tmpl
-drwxrwxrwx   0        0        0        0 2024-01-17 07:14:06.307473 aio-scrapy-2.0.8/aioscrapy/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.8/aioscrapy/utils/__init__.py
--rw-rw-rw-   0        0        0     7208 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/conf.py
--rw-rw-rw-   0        0        0     3295 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/curl.py
--rw-rw-rw-   0        0        0      794 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/decorators.py
--rw-rw-rw-   0        0        0     5467 2023-09-28 01:34:29.000000 aio-scrapy-2.0.8/aioscrapy/utils/deprecate.py
--rw-rw-rw-   0        0        0      708 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/httpobj.py
--rw-rw-rw-   0        0        0     1592 2023-12-06 09:29:44.000000 aio-scrapy-2.0.8/aioscrapy/utils/log.py
--rw-rw-rw-   0        0        0     3509 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/misc.py
--rw-rw-rw-   0        0        0      896 2023-09-26 07:33:08.000000 aio-scrapy-2.0.8/aioscrapy/utils/ossignal.py
--rw-rw-rw-   0        0        0     2905 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/project.py
--rw-rw-rw-   0        0        0     4577 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/python.py
--rw-rw-rw-   0        0        0      487 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/utils/reqser.py
--rw-rw-rw-   0        0        0     2418 2024-01-17 07:10:58.000000 aio-scrapy-2.0.8/aioscrapy/utils/request.py
--rw-rw-rw-   0        0        0     1341 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/response.py
--rw-rw-rw-   0        0        0     2282 2023-09-26 06:57:24.000000 aio-scrapy-2.0.8/aioscrapy/utils/signal.py
--rw-rw-rw-   0        0        0      610 2023-09-26 06:57:24.000000 aio-scrapy-2.0.8/aioscrapy/utils/spider.py
--rw-rw-rw-   0        0        0      833 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/template.py
--rw-rw-rw-   0        0        0     2319 2023-09-22 09:42:23.000000 aio-scrapy-2.0.8/aioscrapy/utils/tools.py
--rw-rw-rw-   0        0        0     2019 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/trackref.py
--rw-rw-rw-   0        0        0     5464 2023-09-21 06:43:51.000000 aio-scrapy-2.0.8/aioscrapy/utils/url.py
--rw-rw-rw-   0        0        0       42 2024-01-17 07:14:06.323933 aio-scrapy-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2444 2023-10-07 03:17:40.000000 aio-scrapy-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.429945 aio-scrapy-2.0.9/
+-rw-rw-rw-   0        0        0     1088 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0      182 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6337 2024-04-03 06:32:05.428956 aio-scrapy-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3855 2023-12-25 01:05:41.000000 aio-scrapy-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.425913 aio-scrapy-2.0.9/aio_scrapy.egg-info/
+-rw-rw-rw-   0        0        0     6337 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4366 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      574 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 06:32:04.000000 aio-scrapy-2.0.9/aio_scrapy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.875668 aio-scrapy-2.0.9/aioscrapy/
+-rw-rw-rw-   0        0        0        5 2024-04-03 06:26:17.000000 aio-scrapy-2.0.9/aioscrapy/VERSION
+-rw-rw-rw-   0        0        0      858 2023-09-28 01:34:29.000000 aio-scrapy-2.0.9/aioscrapy/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/__main__.py
+-rw-rw-rw-   0        0        0     5159 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/cmdline.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.918480 aio-scrapy-2.0.9/aioscrapy/commands/
+-rw-rw-rw-   0        0        0     4769 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/__init__.py
+-rw-rw-rw-   0        0        0     1020 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/crawl.py
+-rw-rw-rw-   0        0        0     5426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/genspider.py
+-rw-rw-rw-   0        0        0      346 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/list.py
+-rw-rw-rw-   0        0        0     2067 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/runspider.py
+-rw-rw-rw-   0        0        0     1798 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/settings.py
+-rw-rw-rw-   0        0        0     4001 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/startproject.py
+-rw-rw-rw-   0        0        0      485 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/commands/version.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.923810 aio-scrapy-2.0.9/aioscrapy/core/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.938965 aio-scrapy-2.0.9/aioscrapy/core/downloader/
+-rw-rw-rw-   0        0        0     9465 2024-01-15 09:49:33.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.995130 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/
+-rw-rw-rw-   0        0        0     3198 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3942 2023-12-25 07:35:12.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/aiohttp.py
+-rw-rw-rw-   0        0        0     3041 2023-09-27 08:43:17.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/httpx.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.006182 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/
+-rw-rw-rw-   0        0        0     4160 2023-10-12 09:22:48.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/__init__.py
+-rw-rw-rw-   0        0        0     1374 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py
+-rw-rw-rw-   0        0        0     3530 2023-10-12 09:38:59.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py
+-rw-rw-rw-   0        0        0     2228 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/pyhttpx.py
+-rw-rw-rw-   0        0        0     1996 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/requests.py
+-rw-rw-rw-   0        0        0    10925 2024-01-15 09:37:22.000000 aio-scrapy-2.0.9/aioscrapy/core/engine.py
+-rw-rw-rw-   0        0        0     5737 2023-09-27 09:13:11.000000 aio-scrapy-2.0.9/aioscrapy/core/scheduler.py
+-rw-rw-rw-   0        0        0    10304 2023-10-12 09:32:46.000000 aio-scrapy-2.0.9/aioscrapy/core/scraper.py
+-rw-rw-rw-   0        0        0    10109 2023-12-22 04:04:27.000000 aio-scrapy-2.0.9/aioscrapy/crawler.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.014768 aio-scrapy-2.0.9/aioscrapy/db/
+-rw-rw-rw-   0        0        0     2456 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/__init__.py
+-rw-rw-rw-   0        0        0     1162 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/db/absmanager.py
+-rw-rw-rw-   0        0        0     2745 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiomongo.py
+-rw-rw-rw-   0        0        0     3799 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiomysql.py
+-rw-rw-rw-   0        0        0     3213 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiopg.py
+-rw-rw-rw-   0        0        0     5583 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/db/aiorabbitmq.py
+-rw-rw-rw-   0        0        0     2966 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/db/aioredis.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.030116 aio-scrapy-2.0.9/aioscrapy/dupefilters/
+-rw-rw-rw-   0        0        0     1498 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/__init__.py
+-rw-rw-rw-   0        0        0     1551 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/disk.py
+-rw-rw-rw-   0        0        0     4723 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/dupefilters/redis.py
+-rw-rw-rw-   0        0        0     2027 2024-01-15 09:43:42.000000 aio-scrapy-2.0.9/aioscrapy/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.033116 aio-scrapy-2.0.9/aioscrapy/http/
+-rw-rw-rw-   0        0        0      597 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/__init__.py
+-rw-rw-rw-   0        0        0     1573 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/headers.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.057981 aio-scrapy-2.0.9/aioscrapy/http/request/
+-rw-rw-rw-   0        0        0     7121 2023-09-26 06:37:06.000000 aio-scrapy-2.0.9/aioscrapy/http/request/__init__.py
+-rw-rw-rw-   0        0        0     1382 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/request/form.py
+-rw-rw-rw-   0        0        0     2051 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/request/json_request.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.091989 aio-scrapy-2.0.9/aioscrapy/http/response/
+-rw-rw-rw-   0        0        0     6731 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/__init__.py
+-rw-rw-rw-   0        0        0      303 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/html.py
+-rw-rw-rw-   0        0        0     1051 2023-10-12 09:29:08.000000 aio-scrapy-2.0.9/aioscrapy/http/response/playwright.py
+-rw-rw-rw-   0        0        0     9844 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/text.py
+-rw-rw-rw-   0        0        0      300 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/http/response/xml.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.092988 aio-scrapy-2.0.9/aioscrapy/libs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.119955 aio-scrapy-2.0.9/aioscrapy/libs/downloader/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/__init__.py
+-rw-rw-rw-   0        0        0      563 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/defaultheaders.py
+-rw-rw-rw-   0        0        0      704 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/downloadtimeout.py
+-rw-rw-rw-   0        0        0     1058 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/ja3fingerprint.py
+-rw-rw-rw-   0        0        0     5191 2024-03-01 06:49:55.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/retry.py
+-rw-rw-rw-   0        0        0     1376 2023-09-26 09:41:57.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/stats.py
+-rw-rw-rw-   0        0        0      743 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/downloader/useragent.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.137091 aio-scrapy-2.0.9/aioscrapy/libs/extensions/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/__init__.py
+-rw-rw-rw-   0        0        0     2734 2023-09-22 10:41:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/closespider.py
+-rw-rw-rw-   0        0        0     1820 2023-09-26 08:56:09.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/corestats.py
+-rw-rw-rw-   0        0        0     1844 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/logstats.py
+-rw-rw-rw-   0        0        0     5479 2023-10-20 01:51:59.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/metric.py
+-rw-rw-rw-   0        0        0     3512 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/extensions/throttle.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.145175 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/
+-rw-rw-rw-   0        0        0     5709 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/__init__.py
+-rw-rw-rw-   0        0        0     2454 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/csv.py
+-rw-rw-rw-   0        0        0     6284 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/execl.py
+-rw-rw-rw-   0        0        0     2001 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mongo.py
+-rw-rw-rw-   0        0        0     1022 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mysql.py
+-rw-rw-rw-   0        0        0      990 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/pipelines/pg.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.163841 aio-scrapy-2.0.9/aioscrapy/libs/spider/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/__init__.py
+-rw-rw-rw-   0        0        0     1938 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/depth.py
+-rw-rw-rw-   0        0        0     1857 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/httperror.py
+-rw-rw-rw-   0        0        0     2941 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/offsite.py
+-rw-rw-rw-   0        0        0    13768 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/referer.py
+-rw-rw-rw-   0        0        0     1151 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/libs/spider/urllength.py
+-rw-rw-rw-   0        0        0     1867 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/link.py
+-rw-rw-rw-   0        0        0     3028 2023-10-12 09:32:03.000000 aio-scrapy-2.0.9/aioscrapy/logformatter.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.170852 aio-scrapy-2.0.9/aioscrapy/middleware/
+-rw-rw-rw-   0        0        0      396 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/middleware/__init__.py
+-rw-rw-rw-   0        0        0     3410 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/middleware/absmanager.py
+-rw-rw-rw-   0        0        0     3199 2023-09-26 06:48:29.000000 aio-scrapy-2.0.9/aioscrapy/middleware/downloader.py
+-rw-rw-rw-   0        0        0      420 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/middleware/extension.py
+-rw-rw-rw-   0        0        0      674 2023-09-19 03:48:43.000000 aio-scrapy-2.0.9/aioscrapy/middleware/itempipeline.py
+-rw-rw-rw-   0        0        0     6361 2023-12-05 08:01:00.000000 aio-scrapy-2.0.9/aioscrapy/middleware/spider.py
+-rw-rw-rw-   0        0        0     1603 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/process.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.199809 aio-scrapy-2.0.9/aioscrapy/proxy/
+-rw-rw-rw-   0        0        0     1807 2024-01-15 08:08:24.000000 aio-scrapy-2.0.9/aioscrapy/proxy/__init__.py
+-rw-rw-rw-   0        0        0     2711 2024-01-15 09:59:00.000000 aio-scrapy-2.0.9/aioscrapy/proxy/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.224959 aio-scrapy-2.0.9/aioscrapy/queue/
+-rw-rw-rw-   0        0        0     2037 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/__init__.py
+-rw-rw-rw-   0        0        0     3140 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/memory.py
+-rw-rw-rw-   0        0        0     2516 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/rabbitmq.py
+-rw-rw-rw-   0        0        0     4788 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/queue/redis.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.240616 aio-scrapy-2.0.9/aioscrapy/scrapyd/
+-rw-rw-rw-   0        0        0       68 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/scrapyd/__init__.py
+-rw-rw-rw-   0        0        0     1777 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/scrapyd/runner.py
+-rw-rw-rw-   0        0        0      734 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/serializer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.258422 aio-scrapy-2.0.9/aioscrapy/settings/
+-rw-rw-rw-   0        0        0    15781 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/settings/__init__.py
+-rw-rw-rw-   0        0        0     5432 2023-09-27 08:43:18.000000 aio-scrapy-2.0.9/aioscrapy/settings/default_settings.py
+-rw-rw-rw-   0        0        0     2402 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/signalmanager.py
+-rw-rw-rw-   0        0        0      610 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/signals.py
+-rw-rw-rw-   0        0        0     3426 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/spiderloader.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.268995 aio-scrapy-2.0.9/aioscrapy/spiders/
+-rw-rw-rw-   0        0        0     3934 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/spiders/__init__.py
+-rw-rw-rw-   0        0        0     2036 2023-12-05 07:56:11.000000 aio-scrapy-2.0.9/aioscrapy/statscollectors.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:04.778530 aio-scrapy-2.0.9/aioscrapy/templates/
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.270997 aio-scrapy-2.0.9/aioscrapy/templates/project/
+-rw-rw-rw-   0        0        0      112 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/aioscrapy.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.285303 aio-scrapy-2.0.9/aioscrapy/templates/project/module/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-12-05 07:04:56.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/middlewares.py.tmpl
+-rw-rw-rw-   0        0        0      164 2023-12-05 07:04:56.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/pipelines.py.tmpl
+-rw-rw-rw-   0        0        0     1421 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/settings.py.tmpl
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.303577 aio-scrapy-2.0.9/aioscrapy/templates/project/module/spiders/
+-rw-rw-rw-   0        0        0      164 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/templates/project/module/spiders/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.306579 aio-scrapy-2.0.9/aioscrapy/templates/spiders/
+-rw-rw-rw-   0        0        0      375 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/spiders/basic.tmpl
+-rw-rw-rw-   0        0        0      942 2023-12-05 07:11:48.000000 aio-scrapy-2.0.9/aioscrapy/templates/spiders/single.tmpl
+drwxrwxrwx   0        0        0        0 2024-04-03 06:32:05.414993 aio-scrapy-2.0.9/aioscrapy/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 08:42:04.000000 aio-scrapy-2.0.9/aioscrapy/utils/__init__.py
+-rw-rw-rw-   0        0        0     7208 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/conf.py
+-rw-rw-rw-   0        0        0     3295 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/curl.py
+-rw-rw-rw-   0        0        0      794 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/decorators.py
+-rw-rw-rw-   0        0        0     5467 2023-09-28 01:34:29.000000 aio-scrapy-2.0.9/aioscrapy/utils/deprecate.py
+-rw-rw-rw-   0        0        0      708 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/httpobj.py
+-rw-rw-rw-   0        0        0     1697 2024-04-03 06:24:20.000000 aio-scrapy-2.0.9/aioscrapy/utils/log.py
+-rw-rw-rw-   0        0        0     3509 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/misc.py
+-rw-rw-rw-   0        0        0      896 2023-09-26 07:33:08.000000 aio-scrapy-2.0.9/aioscrapy/utils/ossignal.py
+-rw-rw-rw-   0        0        0     2905 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/project.py
+-rw-rw-rw-   0        0        0     4577 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/python.py
+-rw-rw-rw-   0        0        0      487 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/utils/reqser.py
+-rw-rw-rw-   0        0        0     2418 2024-01-17 07:10:58.000000 aio-scrapy-2.0.9/aioscrapy/utils/request.py
+-rw-rw-rw-   0        0        0     1341 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/response.py
+-rw-rw-rw-   0        0        0     2282 2023-09-26 06:57:24.000000 aio-scrapy-2.0.9/aioscrapy/utils/signal.py
+-rw-rw-rw-   0        0        0      610 2023-09-26 06:57:24.000000 aio-scrapy-2.0.9/aioscrapy/utils/spider.py
+-rw-rw-rw-   0        0        0      833 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/template.py
+-rw-rw-rw-   0        0        0     2319 2023-09-22 09:42:23.000000 aio-scrapy-2.0.9/aioscrapy/utils/tools.py
+-rw-rw-rw-   0        0        0     2019 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/trackref.py
+-rw-rw-rw-   0        0        0     5464 2023-09-21 06:43:51.000000 aio-scrapy-2.0.9/aioscrapy/utils/url.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 06:32:05.430945 aio-scrapy-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2444 2023-10-07 03:17:40.000000 aio-scrapy-2.0.9/setup.py
```

### Comparing `aio-scrapy-2.0.8/LICENSE` & `aio-scrapy-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/PKG-INFO` & `aio-scrapy-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 2.0.8
+Version: 2.0.9
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aio-scrapy-2.0.8/README.md` & `aio-scrapy-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aio_scrapy.egg-info/PKG-INFO` & `aio-scrapy-2.0.9/aio_scrapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-scrapy
-Version: 2.0.8
+Version: 2.0.9
 Summary: A high-level Web Crawling and Web Scraping framework based on Asyncio
 Home-page: https://github.com/conlin-huang/aio-scrapy.git
 Author: conlin
 Author-email: 995018884@qq.com
 License: MIT
 Keywords: aio-scrapy,scrapy,aioscrapy,scrapy redis,asyncio,spider
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aio-scrapy-2.0.8/aio_scrapy.egg-info/SOURCES.txt` & `aio-scrapy-2.0.9/aio_scrapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aio_scrapy.egg-info/requires.txt` & `aio-scrapy-2.0.9/aio_scrapy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/cmdline.py` & `aio-scrapy-2.0.9/aioscrapy/cmdline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/crawl.py` & `aio-scrapy-2.0.9/aioscrapy/commands/crawl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/genspider.py` & `aio-scrapy-2.0.9/aioscrapy/commands/genspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/runspider.py` & `aio-scrapy-2.0.9/aioscrapy/commands/runspider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/settings.py` & `aio-scrapy-2.0.9/aioscrapy/commands/settings.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/commands/startproject.py` & `aio-scrapy-2.0.9/aioscrapy/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/aiohttp.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/httpx.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/httpx.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/driverpool.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/driverpool.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/playwright/webdriver.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/playwright/webdriver.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/pyhttpx.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/pyhttpx.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/downloader/handlers/requests.py` & `aio-scrapy-2.0.9/aioscrapy/core/downloader/handlers/requests.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/engine.py` & `aio-scrapy-2.0.9/aioscrapy/core/engine.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/scheduler.py` & `aio-scrapy-2.0.9/aioscrapy/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/core/scraper.py` & `aio-scrapy-2.0.9/aioscrapy/core/scraper.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/crawler.py` & `aio-scrapy-2.0.9/aioscrapy/crawler.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/db/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/absmanager.py` & `aio-scrapy-2.0.9/aioscrapy/db/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/aiomongo.py` & `aio-scrapy-2.0.9/aioscrapy/db/aiomongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/aiomysql.py` & `aio-scrapy-2.0.9/aioscrapy/db/aiomysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/aiopg.py` & `aio-scrapy-2.0.9/aioscrapy/db/aiopg.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/aiorabbitmq.py` & `aio-scrapy-2.0.9/aioscrapy/db/aiorabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/db/aioredis.py` & `aio-scrapy-2.0.9/aioscrapy/db/aioredis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/dupefilters/disk.py` & `aio-scrapy-2.0.9/aioscrapy/dupefilters/disk.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,58 +1,44 @@
 import os
 from typing import Optional, Set
 
-from aioscrapy import Request, Spider
+from aioscrapy import Request
 from aioscrapy.dupefilters import DupeFilterBase
-from aioscrapy.utils.log import logger
-from aioscrapy.utils.request import referer_str
 
 
 class DiskRFPDupeFilter(DupeFilterBase):
     """Request Fingerprint duplicates filter built with Disk storage"""
 
-    def __init__(self, path: Optional[str] = None, debug: bool = False):
+    def __init__(self, path: Optional[str] = None, debug: bool = False, info: bool = False):
         self.file: Optional["File object"] = None
         self.debug = debug
         self.fingerprints: Set = set()
         self.logdupes: bool = True
+        self.info: bool = info
         if path:
             self.file = open(os.path.join(path, 'requests.seen'), 'a+')
             self.file.seek(0)
             self.fingerprints.update(x.rstrip() for x in self.file)
 
     @classmethod
     def from_crawler(cls, crawler: "aioscrapy.crawler.Crawler"):
         debug = crawler.settings.getbool('DUPEFILTER_DEBUG')
+        info = crawler.settings.getbool('DUPEFILTER_INFO')
         path = crawler.settings.get('JOBDIR', './job_dir')
         if path and not os.path.exists(path):
             os.makedirs(path)
-        return cls(path, debug)
+        return cls(path, debug, info)
 
     async def request_seen(self, request: Request) -> bool:
         if request.fingerprint in self.fingerprints:
             return True
         self.fingerprints.add(request.fingerprint)
         if self.file:
             self.file.write(request.fingerprint + '\n')
         return False
 
     async def close(self, reason: str = '') -> None:
         if self.file:
             self.file.close()
 
-    def log(self, request: Request, spider: Spider):
-        if self.debug:
-            logger.debug("Filtered duplicate request: %(request)s (referer: %(referer)s)" % {
-                'request': request, 'referer': referer_str(request)
-            })
-        elif self.logdupes:
-            msg = ("Filtered duplicate request: %(request)s"
-                   " - no more duplicates will be shown"
-                   " (see DUPEFILTER_DEBUG to show all duplicates)")
-            logger.debug(msg % {'request': request})
-            self.logdupes = False
-
-        spider.crawler.stats.inc_value('dupefilter/filtered', spider=spider)
-
 
 RFPDupeFilter = DiskRFPDupeFilter
```

### Comparing `aio-scrapy-2.0.8/aioscrapy/dupefilters/redis.py` & `aio-scrapy-2.0.9/aioscrapy/dupefilters/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,51 @@
 from aioscrapy import Request
 from aioscrapy.db import db_manager
 from aioscrapy.dupefilters import DupeFilterBase
 
-from aioscrapy.utils.log import logger
-
 
 class RedisRFPDupeFilter(DupeFilterBase):
     """Request Fingerprint duplicates filter built with Set of Redis"""
 
     def __init__(
             self,
             server: "redis.asyncio.Redis",
             key: str,
             debug: bool = False,
-            keep_on_close: bool = True
+            keep_on_close: bool = True,
+            info: bool = False,
     ):
         self.server = server
         self.key = key
         self.debug = debug
         self.keep_on_close = keep_on_close
         self.logdupes: bool = True
+        self.info: bool = info
 
     @classmethod
     def from_crawler(cls, crawler: "aioscrapy.crawler.Crawler"):
         server = db_manager.redis.queue
         dupefilter_key = crawler.settings.get("SCHEDULER_DUPEFILTER_KEY", '%(spider)s:dupefilter')
         keep_on_close = crawler.settings.getbool("KEEP_DUPEFILTER_DATA_ON_CLOSE", True)
         key = dupefilter_key % {'spider': crawler.spider.name}
         debug = crawler.settings.getbool('DUPEFILTER_DEBUG', False)
-        instance = cls(server, key=key, debug=debug, keep_on_close=keep_on_close)
+        info = crawler.settings.getbool('DUPEFILTER_DEBUG', False)
+        instance = cls(server, key=key, debug=debug, keep_on_close=keep_on_close, info=info)
         return instance
 
     async def request_seen(self, request: Request):
         return await self.server.sadd(self.key, request.fingerprint) == 0
 
     async def close(self, reason=''):
         if not self.keep_on_close:
             await self.clear()
 
     async def clear(self):
         await self.server.delete(self.key)
 
-    def log(self, request, spider):
-        if self.debug:
-            logger.debug("Filtered duplicate request: %(request)s" % {'request': request})
-        elif self.logdupes:
-            msg = ("Filtered duplicate request %(request)s"
-                   " - no more duplicates will be shown"
-                   " (see DUPEFILTER_DEBUG to show all duplicates)")
-            logger.debug(msg % {'request': request})
-            self.logdupes = False
-        spider.crawler.stats.inc_value('dupefilter/filtered', spider=spider)
-
 
 class HashMap(object):
     def __init__(self, m, seed):
         self.m = m
         self.seed = seed
 
     def hash(self, value):
```

### Comparing `aio-scrapy-2.0.8/aioscrapy/exceptions.py` & `aio-scrapy-2.0.9/aioscrapy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/http/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/headers.py` & `aio-scrapy-2.0.9/aioscrapy/http/headers.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/request/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/http/request/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/request/form.py` & `aio-scrapy-2.0.9/aioscrapy/http/request/form.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/request/json_request.py` & `aio-scrapy-2.0.9/aioscrapy/http/request/json_request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/response/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/http/response/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/response/playwright.py` & `aio-scrapy-2.0.9/aioscrapy/http/response/playwright.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/http/response/text.py` & `aio-scrapy-2.0.9/aioscrapy/http/response/text.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/defaultheaders.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/defaultheaders.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/downloadtimeout.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/downloadtimeout.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/ja3fingerprint.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/ja3fingerprint.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/retry.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/retry.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     from aiohttp.client_exceptions import ClientError
 
     NEED_RETRY_ERROR += (ClientError,)
 except ImportError:
     pass
 
 try:
+    from anyio import EndOfStream
+
+    NEED_RETRY_ERROR += (EndOfStream,)
+except ImportError:
+    pass
+
+try:
     from httpx import HTTPError as HttpxError
 
     NEED_RETRY_ERROR += (HttpxError,)
 except ImportError:
     pass
 
 try:
```

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/stats.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/stats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/downloader/useragent.py` & `aio-scrapy-2.0.9/aioscrapy/libs/downloader/useragent.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/extensions/closespider.py` & `aio-scrapy-2.0.9/aioscrapy/libs/extensions/closespider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/extensions/corestats.py` & `aio-scrapy-2.0.9/aioscrapy/libs/extensions/corestats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/extensions/logstats.py` & `aio-scrapy-2.0.9/aioscrapy/libs/extensions/logstats.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/extensions/metric.py` & `aio-scrapy-2.0.9/aioscrapy/libs/extensions/metric.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/extensions/throttle.py` & `aio-scrapy-2.0.9/aioscrapy/libs/extensions/throttle.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/csv.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/csv.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/execl.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/execl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/mongo.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mongo.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/mysql.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/mysql.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/pipelines/pg.py` & `aio-scrapy-2.0.9/aioscrapy/libs/pipelines/pg.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/spider/depth.py` & `aio-scrapy-2.0.9/aioscrapy/libs/spider/depth.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/spider/httperror.py` & `aio-scrapy-2.0.9/aioscrapy/libs/spider/httperror.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/spider/offsite.py` & `aio-scrapy-2.0.9/aioscrapy/libs/spider/offsite.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/spider/referer.py` & `aio-scrapy-2.0.9/aioscrapy/libs/spider/referer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/libs/spider/urllength.py` & `aio-scrapy-2.0.9/aioscrapy/libs/spider/urllength.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/link.py` & `aio-scrapy-2.0.9/aioscrapy/link.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/logformatter.py` & `aio-scrapy-2.0.9/aioscrapy/logformatter.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/middleware/absmanager.py` & `aio-scrapy-2.0.9/aioscrapy/middleware/absmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/middleware/downloader.py` & `aio-scrapy-2.0.9/aioscrapy/middleware/downloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/middleware/itempipeline.py` & `aio-scrapy-2.0.9/aioscrapy/middleware/itempipeline.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/middleware/spider.py` & `aio-scrapy-2.0.9/aioscrapy/middleware/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/process.py` & `aio-scrapy-2.0.9/aioscrapy/process.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/proxy/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/proxy/redis.py` & `aio-scrapy-2.0.9/aioscrapy/proxy/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/queue/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/queue/memory.py` & `aio-scrapy-2.0.9/aioscrapy/queue/memory.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/queue/rabbitmq.py` & `aio-scrapy-2.0.9/aioscrapy/queue/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/queue/redis.py` & `aio-scrapy-2.0.9/aioscrapy/queue/redis.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/scrapyd/runner.py` & `aio-scrapy-2.0.9/aioscrapy/scrapyd/runner.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/serializer.py` & `aio-scrapy-2.0.9/aioscrapy/serializer.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/settings/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/settings/default_settings.py` & `aio-scrapy-2.0.9/aioscrapy/settings/default_settings.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/signalmanager.py` & `aio-scrapy-2.0.9/aioscrapy/signalmanager.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/signals.py` & `aio-scrapy-2.0.9/aioscrapy/signals.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/spiderloader.py` & `aio-scrapy-2.0.9/aioscrapy/spiderloader.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/spiders/__init__.py` & `aio-scrapy-2.0.9/aioscrapy/spiders/__init__.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/statscollectors.py` & `aio-scrapy-2.0.9/aioscrapy/statscollectors.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/templates/project/module/middlewares.py.tmpl` & `aio-scrapy-2.0.9/aioscrapy/templates/project/module/middlewares.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/templates/project/module/settings.py.tmpl` & `aio-scrapy-2.0.9/aioscrapy/templates/project/module/settings.py.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/templates/spiders/single.tmpl` & `aio-scrapy-2.0.9/aioscrapy/templates/spiders/single.tmpl`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/conf.py` & `aio-scrapy-2.0.9/aioscrapy/utils/conf.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/curl.py` & `aio-scrapy-2.0.9/aioscrapy/utils/curl.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/decorators.py` & `aio-scrapy-2.0.9/aioscrapy/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/deprecate.py` & `aio-scrapy-2.0.9/aioscrapy/utils/deprecate.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/httpobj.py` & `aio-scrapy-2.0.9/aioscrapy/utils/httpobj.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/log.py` & `aio-scrapy-2.0.9/aioscrapy/utils/log.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import warnings
 from typing import Type
 
 from loguru import logger as _logger
 
 from aioscrapy.settings import Settings
 
-_logger.remove(0)
+for _handler in _logger._core.handlers.values():
+    if _handler._name == '<stderr>':
+        _logger.remove(_handler._id)
 
 
 def configure_logging(spider: Type["Spider"], settings: Settings):
     formatter = settings.get('LOG_FORMAT')
     level = settings.get('LOG_LEVEL', 'INFO')
     enqueue = settings.get('ENQUEUE', True)
     if settings.get('LOG_STDOUT', True):
```

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/misc.py` & `aio-scrapy-2.0.9/aioscrapy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/ossignal.py` & `aio-scrapy-2.0.9/aioscrapy/utils/ossignal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/project.py` & `aio-scrapy-2.0.9/aioscrapy/utils/project.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/python.py` & `aio-scrapy-2.0.9/aioscrapy/utils/python.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/request.py` & `aio-scrapy-2.0.9/aioscrapy/utils/request.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/response.py` & `aio-scrapy-2.0.9/aioscrapy/utils/response.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/signal.py` & `aio-scrapy-2.0.9/aioscrapy/utils/signal.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/spider.py` & `aio-scrapy-2.0.9/aioscrapy/utils/spider.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/template.py` & `aio-scrapy-2.0.9/aioscrapy/utils/template.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/tools.py` & `aio-scrapy-2.0.9/aioscrapy/utils/tools.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/trackref.py` & `aio-scrapy-2.0.9/aioscrapy/utils/trackref.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/aioscrapy/utils/url.py` & `aio-scrapy-2.0.9/aioscrapy/utils/url.py`

 * *Files identical despite different names*

### Comparing `aio-scrapy-2.0.8/setup.py` & `aio-scrapy-2.0.9/setup.py`

 * *Files identical despite different names*

