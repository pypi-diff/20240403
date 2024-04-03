# Comparing `tmp/hyperiontf-0.2.5.tar.gz` & `tmp/hyperiontf-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperiontf-0.2.5.tar", max compression
+gzip compressed data, was "hyperiontf-0.3.5.tar", max compression
```

## Comparing `hyperiontf-0.2.5.tar` & `hyperiontf-0.3.5.tar`

### file list

```diff
@@ -1,148 +1,156 @@
--rw-r--r--   0        0        0    11357 2023-10-24 17:19:29.257507 hyperiontf-0.2.5/LICENSE
--rw-r--r--   0        0        0    61743 2024-03-05 20:05:34.920553 hyperiontf-0.2.5/README.md
--rw-r--r--   0        0        0      501 2024-03-05 20:05:34.921109 hyperiontf-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      804 2024-02-26 19:03:16.886882 hyperiontf-0.2.5/src/hyperiontf/__init__.py
--rw-r--r--   0        0        0       61 2023-10-24 17:19:29.258346 hyperiontf-0.2.5/src/hyperiontf/api/__init__.py
--rw-r--r--   0        0        0        1 2023-10-24 17:19:29.258457 hyperiontf-0.2.5/src/hyperiontf/api/rest_client/__init__.py
--rw-r--r--   0        0        0    28320 2024-02-26 19:03:16.887302 hyperiontf-0.2.5/src/hyperiontf/api/rest_client/client.py
--rw-r--r--   0        0        0    18293 2024-02-26 19:03:16.887939 hyperiontf-0.2.5/src/hyperiontf/api/rest_client/request.py
--rw-r--r--   0        0        0    10284 2024-02-26 19:03:16.889361 hyperiontf-0.2.5/src/hyperiontf/api/rest_client/response.py
--rw-r--r--   0        0        0       68 2024-02-26 19:03:16.889991 hyperiontf-0.2.5/src/hyperiontf/assertions/__init__.py
--rw-r--r--   0        0        0     1744 2024-02-26 19:03:16.890118 hyperiontf-0.2.5/src/hyperiontf/assertions/decorators.py
--rw-r--r--   0        0        0    95124 2024-02-26 19:03:16.891227 hyperiontf-0.2.5/src/hyperiontf/assertions/expect.py
--rw-r--r--   0        0        0    12001 2024-02-26 19:03:16.891539 hyperiontf-0.2.5/src/hyperiontf/assertions/expectation_result.py
--rw-r--r--   0        0        0     1038 2024-02-26 19:03:16.891663 hyperiontf-0.2.5/src/hyperiontf/assertions/helpers.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.891702 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/__init__.py
--rw-r--r--   0        0        0     7944 2024-02-26 19:03:16.891847 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/array_strategy.py
--rw-r--r--   0        0        0     7074 2024-02-26 19:03:16.891965 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/color_strategy.py
--rw-r--r--   0        0        0     3430 2024-02-26 19:03:16.892240 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/decorators.py
--rw-r--r--   0        0        0    10400 2024-02-26 19:03:16.892903 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/default_strategy.py
--rw-r--r--   0        0        0     8142 2024-02-26 19:03:16.893251 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/dict_strategy.py
--rw-r--r--   0        0        0     5372 2024-02-26 19:03:16.893388 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/filesystem_strategy.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.893417 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/image_strategy.py
--rw-r--r--   0        0        0    21136 2024-02-26 19:03:16.893592 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/numeric_strategy.py
--rw-r--r--   0        0        0    13069 2024-02-26 19:03:16.893835 hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/string_strategy.py
--rw-r--r--   0        0        0       49 2023-10-24 17:19:29.259629 hyperiontf-0.2.5/src/hyperiontf/configuration/__init__.py
--rw-r--r--   0        0        0      739 2023-10-24 17:19:29.259709 hyperiontf-0.2.5/src/hyperiontf/configuration/capabilities.py
--rw-r--r--   0        0        0     3488 2024-02-26 19:03:16.894889 hyperiontf-0.2.5/src/hyperiontf/configuration/config.py
--rw-r--r--   0        0        0     1269 2024-02-26 19:03:16.895752 hyperiontf-0.2.5/src/hyperiontf/configuration/section.py
--rw-r--r--   0        0        0      417 2023-10-24 17:19:29.259995 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/__init__.py
--rw-r--r--   0        0        0      403 2023-10-24 17:19:29.260088 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/desktop_capabilities.py
--rw-r--r--   0        0        0      328 2023-10-24 17:19:29.260166 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/element.py
--rw-r--r--   0        0        0      309 2023-10-24 17:19:29.260236 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/logger.py
--rw-r--r--   0        0        0      456 2023-10-24 17:19:29.260313 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/mobile_capabilities.py
--rw-r--r--   0        0        0      437 2023-10-24 17:19:29.260394 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/page_object.py
--rw-r--r--   0        0        0      397 2023-10-24 17:19:29.260506 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/rest.py
--rw-r--r--   0        0        0      772 2023-10-24 17:19:29.260587 hyperiontf-0.2.5/src/hyperiontf/configuration/sections/web_capabilities.py
--rw-r--r--   0        0        0        0 2023-10-24 17:19:29.260658 hyperiontf-0.2.5/src/hyperiontf/executors/__init__.py
--rw-r--r--   0        0        0      122 2023-10-24 17:19:29.260780 hyperiontf-0.2.5/src/hyperiontf/executors/pytest/__init__.py
--rw-r--r--   0        0        0     3607 2023-10-24 17:19:29.260882 hyperiontf-0.2.5/src/hyperiontf/executors/pytest/fixture.py
--rw-r--r--   0        0        0     2437 2024-02-26 19:03:16.896651 hyperiontf-0.2.5/src/hyperiontf/executors/pytest/logger_setup.py
--rw-r--r--   0        0        0       71 2024-02-26 19:03:16.896808 hyperiontf-0.2.5/src/hyperiontf/fs/__init__.py
--rw-r--r--   0        0        0     4273 2024-02-26 19:03:16.897014 hyperiontf-0.2.5/src/hyperiontf/fs/dir.py
--rw-r--r--   0        0        0    14236 2024-02-26 19:03:16.897421 hyperiontf-0.2.5/src/hyperiontf/fs/file.py
--rw-r--r--   0        0        0        0 2023-10-24 17:19:29.261047 hyperiontf-0.2.5/src/hyperiontf/helpers/__init__.py
--rw-r--r--   0        0        0       58 2023-10-24 17:19:29.261173 hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/__init__.py
--rw-r--r--   0        0        0      504 2023-10-24 17:19:29.261256 hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/singleton.py
--rw-r--r--   0        0        0     2699 2024-02-26 19:03:16.897598 hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/wait.py
--rw-r--r--   0        0        0     2467 2023-10-24 17:19:29.261352 hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/without_failure.py
--rw-r--r--   0        0        0     2460 2024-02-26 19:03:16.897751 hyperiontf-0.2.5/src/hyperiontf/helpers/dict_diff.py
--rw-r--r--   0        0        0      974 2023-10-24 17:19:29.261440 hyperiontf-0.2.5/src/hyperiontf/helpers/dict_heplers.py
--rw-r--r--   0        0        0      792 2023-10-24 17:19:29.261519 hyperiontf-0.2.5/src/hyperiontf/helpers/extend_instance.py
--rw-r--r--   0        0        0     1913 2024-02-26 19:03:16.898809 hyperiontf-0.2.5/src/hyperiontf/helpers/own_methods_helper.py
--rw-r--r--   0        0        0      892 2024-02-26 19:03:16.898960 hyperiontf-0.2.5/src/hyperiontf/helpers/rect_helpers.py
--rw-r--r--   0        0        0     3006 2023-10-24 17:19:29.261718 hyperiontf-0.2.5/src/hyperiontf/helpers/string_helpers.py
--rw-r--r--   0        0        0    11683 2024-02-26 19:03:16.899116 hyperiontf-0.2.5/src/hyperiontf/helpers/wagner_fischer.py
--rw-r--r--   0        0        0        0 2023-10-24 17:19:29.261800 hyperiontf-0.2.5/src/hyperiontf/infrastructure/__init__.py
--rw-r--r--   0        0        0     1725 2023-10-24 17:19:29.261909 hyperiontf-0.2.5/src/hyperiontf/infrastructure/event_blorker.py
--rw-r--r--   0        0        0       92 2023-10-24 17:19:29.262061 hyperiontf-0.2.5/src/hyperiontf/logging/__init__.py
--rwxr-xr-x   0        0        0     2674 2023-10-24 17:19:29.262347 hyperiontf-0.2.5/src/hyperiontf/logging/assets/build
--rw-r--r--   0        0        0      935 2023-10-24 17:19:29.262483 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/button-border-colors.css
--rw-r--r--   0        0        0      252 2023-10-24 17:19:29.262596 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/button.css
--rw-r--r--   0        0        0      665 2023-10-24 17:19:29.262691 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/colors.css
--rw-r--r--   0        0        0      392 2023-10-24 17:19:29.262890 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/filter-bar.css
--rw-r--r--   0        0        0     1048 2023-10-24 17:19:29.263063 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/header.css
--rw-r--r--   0        0        0     1677 2023-10-24 17:19:29.263197 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/icon-color-filters.css
--rw-r--r--   0        0        0    38307 2023-10-24 17:19:29.263493 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/icon-images.css
--rw-r--r--   0        0        0      285 2023-10-24 17:19:29.263707 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/icon.css
--rw-r--r--   0        0        0     2496 2023-10-24 17:19:29.263813 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/log-message.css
--rw-r--r--   0        0        0      135 2023-10-24 17:19:29.263926 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/misc.css
--rw-r--r--   0        0        0      884 2023-10-24 17:19:29.264039 hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/tooltip.css
--rw-r--r--   0        0        0      939 2023-10-24 17:19:29.264212 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/app.js
--rw-r--r--   0        0        0     4974 2023-10-24 17:19:29.264338 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/config.js
--rw-r--r--   0        0        0    11226 2023-10-24 17:19:29.264443 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/controlPanel.js
--rw-r--r--   0        0        0     1356 2023-10-24 17:19:29.264516 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/eventBroker.js
--rw-r--r--   0        0        0     2136 2023-10-24 17:19:29.264623 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/helpers.js
--rw-r--r--   0        0        0    40401 2023-10-24 17:19:29.264774 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/line.js
--rw-r--r--   0        0        0     5490 2023-10-24 17:19:29.264943 hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/logger.js
--rw-r--r--   0        0        0     1192 2023-10-24 17:19:29.265092 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/assert-true.svg
--rw-r--r--   0        0        0     2530 2023-10-24 17:19:29.265196 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/backtrace.svg
--rw-r--r--   0        0        0     1424 2023-10-24 17:19:29.265281 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/collapse.svg
--rw-r--r--   0        0        0      724 2023-10-24 17:19:29.265354 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/column.svg
--rw-r--r--   0        0        0     1936 2023-10-24 17:19:29.265448 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/debug.svg
--rw-r--r--   0        0        0     1371 2023-10-24 17:19:29.265561 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/error.svg
--rw-r--r--   0        0        0     1432 2023-10-24 17:19:29.265680 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/expand.svg
--rw-r--r--   0        0        0     3067 2023-10-24 17:19:29.265778 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/fatal.svg
--rw-r--r--   0        0        0     1852 2023-10-24 17:19:29.265906 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/info.svg
--rw-r--r--   0        0        0      615 2023-10-24 17:19:29.266003 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/level.svg
--rw-r--r--   0        0        0     2582 2023-10-24 17:19:29.266106 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/log.svg
--rw-r--r--   0        0        0     1347 2023-10-24 17:19:29.266198 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/page-source.svg
--rw-r--r--   0        0        0      847 2023-10-24 17:19:29.266288 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/screen-snap.svg
--rw-r--r--   0        0        0     3786 2023-10-24 17:19:29.266369 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/timestamp.svg
--rw-r--r--   0        0        0     2555 2023-10-24 17:19:29.266474 hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/warning.svg
--rw-r--r--   0        0        0    67094 2023-10-24 17:19:29.266730 hyperiontf-0.2.5/src/hyperiontf/logging/assets/template.html
--rw-r--r--   0        0        0     2485 2023-10-24 17:19:29.267068 hyperiontf-0.2.5/src/hyperiontf/logging/file_handler.py
--rw-r--r--   0        0        0     4531 2024-03-05 20:05:34.921553 hyperiontf-0.2.5/src/hyperiontf/logging/formatter.py
--rw-r--r--   0        0        0      715 2023-10-24 17:19:29.267216 hyperiontf-0.2.5/src/hyperiontf/logging/helpers.py
--rw-r--r--   0        0        0     1606 2024-02-26 19:03:16.899820 hyperiontf-0.2.5/src/hyperiontf/logging/log_depth_manager.py
--rw-r--r--   0        0        0     2115 2023-10-24 17:19:29.267380 hyperiontf-0.2.5/src/hyperiontf/logging/log_file_manager.py
--rw-r--r--   0        0        0     4642 2023-10-24 17:19:29.267468 hyperiontf-0.2.5/src/hyperiontf/logging/logger.py
--rw-r--r--   0        0        0    13371 2024-03-05 20:05:34.922175 hyperiontf-0.2.5/src/hyperiontf/typing.py
--rw-r--r--   0        0        0      831 2024-02-26 19:03:16.901409 hyperiontf-0.2.5/src/hyperiontf/ui/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.901460 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.901661 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/__init__.py
--rw-r--r--   0        0        0     8351 2024-02-26 19:03:16.901846 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/element.py
--rw-r--r--   0        0        0     1212 2024-02-26 19:03:16.901932 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/map_exception.py
--rw-r--r--   0        0        0     1626 2024-02-26 19:03:16.902046 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/map_locator.py
--rw-r--r--   0        0        0     5396 2024-02-26 19:03:16.902133 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/page.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.902166 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/__init__.py
--rw-r--r--   0        0        0     1871 2024-02-26 19:03:16.902363 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/assert_stale_element_reference.py
--rw-r--r--   0        0        0    11651 2024-02-26 19:03:16.902560 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/element.py
--rw-r--r--   0        0        0      938 2024-02-26 19:03:16.902655 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/map_exception.py
--rw-r--r--   0        0        0     1732 2024-02-26 19:03:16.902788 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/map_locator.py
--rw-r--r--   0        0        0     5558 2024-02-26 19:03:16.902878 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/page.py
--rw-r--r--   0        0        0     1693 2024-02-26 19:03:16.903054 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/selenium_to_playwright_script.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.903130 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/__init__.py
--rw-r--r--   0        0        0     9708 2024-02-26 19:03:16.903322 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/element.py
--rw-r--r--   0        0        0     1268 2024-02-26 19:03:16.903410 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/map_exception.py
--rw-r--r--   0        0        0     1204 2024-03-05 20:05:34.922374 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/map_locator.py
--rw-r--r--   0        0        0    13049 2024-03-05 20:05:34.922622 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/page.py
--rw-r--r--   0        0        0     2752 2024-03-05 20:05:34.923094 hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/win_app_driver.py
--rw-r--r--   0        0        0     7578 2024-03-05 20:05:34.923622 hyperiontf-0.2.5/src/hyperiontf/ui/automation_adapter_manager.py
--rw-r--r--   0        0        0     7038 2023-10-24 17:19:29.268661 hyperiontf-0.2.5/src/hyperiontf/ui/by.py
--rw-r--r--   0        0        0    14333 2024-02-26 19:03:16.904934 hyperiontf-0.2.5/src/hyperiontf/ui/color.py
--rw-r--r--   0        0        0     5389 2024-03-05 20:05:34.924013 hyperiontf-0.2.5/src/hyperiontf/ui/content_manager.py
--rw-r--r--   0        0        0     3285 2023-10-24 17:19:29.268885 hyperiontf-0.2.5/src/hyperiontf/ui/context_manager.py
--rw-r--r--   0        0        0        0 2023-10-24 17:19:29.269056 hyperiontf-0.2.5/src/hyperiontf/ui/decorators/__init__.py
--rw-r--r--   0        0        0     5322 2024-02-26 19:03:16.906050 hyperiontf-0.2.5/src/hyperiontf/ui/decorators/autolog_class_method_helper.py
--rw-r--r--   0        0        0     4827 2024-02-26 19:03:16.906693 hyperiontf-0.2.5/src/hyperiontf/ui/decorators/element_accessor.py
--rw-r--r--   0        0        0     3237 2024-03-05 20:05:34.924231 hyperiontf-0.2.5/src/hyperiontf/ui/decorators/element_error_recovery.py
--rw-r--r--   0        0        0     9074 2023-10-24 17:19:29.269717 hyperiontf-0.2.5/src/hyperiontf/ui/decorators/page_object_helpers.py
--rw-r--r--   0        0        0     1424 2023-10-24 17:19:29.269866 hyperiontf-0.2.5/src/hyperiontf/ui/desktop_window.py
--rw-r--r--   0        0        0    40311 2024-02-26 19:03:16.908186 hyperiontf-0.2.5/src/hyperiontf/ui/element.py
--rw-r--r--   0        0        0    10024 2024-02-26 19:03:16.908802 hyperiontf-0.2.5/src/hyperiontf/ui/elements.py
--rw-r--r--   0        0        0        0 2024-02-26 19:03:16.908896 hyperiontf-0.2.5/src/hyperiontf/ui/eql/__init__.py
--rw-r--r--   0        0        0     1749 2024-02-26 19:03:16.909075 hyperiontf-0.2.5/src/hyperiontf/ui/eql/elements_query_language.ebnf
--rw-r--r--   0        0        0     4934 2024-02-26 19:03:16.909237 hyperiontf-0.2.5/src/hyperiontf/ui/eql/executor.py
--rw-r--r--   0        0        0     2430 2024-02-26 19:03:16.909434 hyperiontf-0.2.5/src/hyperiontf/ui/eql/lexer.py
--rw-r--r--   0        0        0     4301 2024-02-26 19:03:16.909532 hyperiontf-0.2.5/src/hyperiontf/ui/eql/parser.py
--rw-r--r--   0        0        0     1531 2024-03-05 20:05:34.924431 hyperiontf-0.2.5/src/hyperiontf/ui/iframe.py
--rw-r--r--   0        0        0    18257 2024-02-26 19:03:16.910135 hyperiontf-0.2.5/src/hyperiontf/ui/locatable.py
--rw-r--r--   0        0        0     1505 2023-10-24 17:19:29.270606 hyperiontf-0.2.5/src/hyperiontf/ui/mobile_screen.py
--rw-r--r--   0        0        0     1233 2023-10-24 17:19:29.270708 hyperiontf-0.2.5/src/hyperiontf/ui/page_object_base.py
--rw-r--r--   0        0        0     9362 2024-03-05 20:05:34.924692 hyperiontf-0.2.5/src/hyperiontf/ui/viewport_manager.py
--rw-r--r--   0        0        0     2242 2023-10-24 17:19:29.272297 hyperiontf-0.2.5/src/hyperiontf/ui/webpage.py
--rw-r--r--   0        0        0     1762 2024-02-26 19:03:16.910808 hyperiontf-0.2.5/src/hyperiontf/ui/webview.py
--rw-r--r--   0        0        0      816 2024-02-26 19:03:16.911169 hyperiontf-0.2.5/src/hyperiontf/ui/widget.py
--rw-r--r--   0        0        0     3728 2023-10-24 17:19:29.272634 hyperiontf-0.2.5/src/hyperiontf/ui/window_manager.py
--rw-r--r--   0        0        0    62460 1970-01-01 00:00:00.000000 hyperiontf-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-24 17:19:29.257507 hyperiontf-0.3.5/LICENSE
+-rw-r--r--   0        0        0    61743 2024-03-05 20:05:34.920553 hyperiontf-0.3.5/README.md
+-rw-r--r--   0        0        0      595 2024-04-03 12:42:34.980013 hyperiontf-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      860 2024-04-03 12:42:34.980937 hyperiontf-0.3.5/src/hyperiontf/__init__.py
+-rw-r--r--   0        0        0       61 2023-10-24 17:19:29.258346 hyperiontf-0.3.5/src/hyperiontf/api/__init__.py
+-rw-r--r--   0        0        0        1 2023-10-24 17:19:29.258457 hyperiontf-0.3.5/src/hyperiontf/api/rest_client/__init__.py
+-rw-r--r--   0        0        0    28320 2024-02-26 19:03:16.887302 hyperiontf-0.3.5/src/hyperiontf/api/rest_client/client.py
+-rw-r--r--   0        0        0    18293 2024-02-26 19:03:16.887939 hyperiontf-0.3.5/src/hyperiontf/api/rest_client/request.py
+-rw-r--r--   0        0        0    10284 2024-02-26 19:03:16.889361 hyperiontf-0.3.5/src/hyperiontf/api/rest_client/response.py
+-rw-r--r--   0        0        0       68 2024-02-26 19:03:16.889991 hyperiontf-0.3.5/src/hyperiontf/assertions/__init__.py
+-rw-r--r--   0        0        0     1744 2024-02-26 19:03:16.890118 hyperiontf-0.3.5/src/hyperiontf/assertions/decorators.py
+-rw-r--r--   0        0        0   104203 2024-04-03 12:42:34.981966 hyperiontf-0.3.5/src/hyperiontf/assertions/expect.py
+-rw-r--r--   0        0        0    12012 2024-04-03 12:42:34.983210 hyperiontf-0.3.5/src/hyperiontf/assertions/expectation_result.py
+-rw-r--r--   0        0        0     1038 2024-02-26 19:03:16.891663 hyperiontf-0.3.5/src/hyperiontf/assertions/helpers.py
+-rw-r--r--   0        0        0     3347 2024-04-03 12:42:34.984485 hyperiontf-0.3.5/src/hyperiontf/assertions/image_expectation_result.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.891702 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/__init__.py
+-rw-r--r--   0        0        0     7944 2024-03-10 18:42:22.586694 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/array_strategy.py
+-rw-r--r--   0        0        0     7074 2024-02-26 19:03:16.891965 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/color_strategy.py
+-rw-r--r--   0        0        0     3430 2024-02-26 19:03:16.892240 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/decorators.py
+-rw-r--r--   0        0        0    10400 2024-02-26 19:03:16.892903 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/default_strategy.py
+-rw-r--r--   0        0        0     8142 2024-02-26 19:03:16.893251 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/dict_strategy.py
+-rw-r--r--   0        0        0     5372 2024-02-26 19:03:16.893388 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/filesystem_strategy.py
+-rw-r--r--   0        0        0    60946 2024-04-03 12:42:34.985556 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/image_strategy.py
+-rw-r--r--   0        0        0    21136 2024-02-26 19:03:16.893592 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/numeric_strategy.py
+-rw-r--r--   0        0        0    13069 2024-02-26 19:03:16.893835 hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/string_strategy.py
+-rw-r--r--   0        0        0       49 2023-10-24 17:19:29.259629 hyperiontf-0.3.5/src/hyperiontf/configuration/__init__.py
+-rw-r--r--   0        0        0      739 2023-10-24 17:19:29.259709 hyperiontf-0.3.5/src/hyperiontf/configuration/capabilities.py
+-rw-r--r--   0        0        0     3531 2024-04-03 12:42:34.986374 hyperiontf-0.3.5/src/hyperiontf/configuration/config.py
+-rw-r--r--   0        0        0     1269 2024-02-26 19:03:16.895752 hyperiontf-0.3.5/src/hyperiontf/configuration/section.py
+-rw-r--r--   0        0        0      458 2024-04-03 12:42:34.986934 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/__init__.py
+-rw-r--r--   0        0        0      403 2023-10-24 17:19:29.260088 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/desktop_capabilities.py
+-rw-r--r--   0        0        0      328 2023-10-24 17:19:29.260166 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/element.py
+-rw-r--r--   0        0        0      309 2023-10-24 17:19:29.260236 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/logger.py
+-rw-r--r--   0        0        0      456 2023-10-24 17:19:29.260313 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/mobile_capabilities.py
+-rw-r--r--   0        0        0     4836 2024-04-03 12:42:34.987364 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/page_object.py
+-rw-r--r--   0        0        0      397 2023-10-24 17:19:29.260506 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/rest.py
+-rw-r--r--   0        0        0      373 2024-04-03 12:42:34.987791 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/visual.py
+-rw-r--r--   0        0        0      772 2023-10-24 17:19:29.260587 hyperiontf-0.3.5/src/hyperiontf/configuration/sections/web_capabilities.py
+-rw-r--r--   0        0        0        0 2023-10-24 17:19:29.260658 hyperiontf-0.3.5/src/hyperiontf/executors/__init__.py
+-rw-r--r--   0        0        0      122 2023-10-24 17:19:29.260780 hyperiontf-0.3.5/src/hyperiontf/executors/pytest/__init__.py
+-rw-r--r--   0        0        0     3607 2023-10-24 17:19:29.260882 hyperiontf-0.3.5/src/hyperiontf/executors/pytest/fixture.py
+-rw-r--r--   0        0        0     2437 2024-02-26 19:03:16.896651 hyperiontf-0.3.5/src/hyperiontf/executors/pytest/logger_setup.py
+-rw-r--r--   0        0        0       71 2024-02-26 19:03:16.896808 hyperiontf-0.3.5/src/hyperiontf/fs/__init__.py
+-rw-r--r--   0        0        0     4273 2024-02-26 19:03:16.897014 hyperiontf-0.3.5/src/hyperiontf/fs/dir.py
+-rw-r--r--   0        0        0    14236 2024-02-26 19:03:16.897421 hyperiontf-0.3.5/src/hyperiontf/fs/file.py
+-rw-r--r--   0        0        0        0 2023-10-24 17:19:29.261047 hyperiontf-0.3.5/src/hyperiontf/helpers/__init__.py
+-rw-r--r--   0        0        0       58 2023-10-24 17:19:29.261173 hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/__init__.py
+-rw-r--r--   0        0        0      504 2023-10-24 17:19:29.261256 hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/singleton.py
+-rw-r--r--   0        0        0     2699 2024-02-26 19:03:16.897598 hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/wait.py
+-rw-r--r--   0        0        0     2467 2023-10-24 17:19:29.261352 hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/without_failure.py
+-rw-r--r--   0        0        0     2460 2024-02-26 19:03:16.897751 hyperiontf-0.3.5/src/hyperiontf/helpers/dict_diff.py
+-rw-r--r--   0        0        0      974 2023-10-24 17:19:29.261440 hyperiontf-0.3.5/src/hyperiontf/helpers/dict_heplers.py
+-rw-r--r--   0        0        0      792 2023-10-24 17:19:29.261519 hyperiontf-0.3.5/src/hyperiontf/helpers/extend_instance.py
+-rw-r--r--   0        0        0      294 2024-04-03 12:42:34.988536 hyperiontf-0.3.5/src/hyperiontf/helpers/numeric_helpers.py
+-rw-r--r--   0        0        0     1913 2024-02-26 19:03:16.898809 hyperiontf-0.3.5/src/hyperiontf/helpers/own_methods_helper.py
+-rw-r--r--   0        0        0      892 2024-02-26 19:03:16.898960 hyperiontf-0.3.5/src/hyperiontf/helpers/rect_helpers.py
+-rw-r--r--   0        0        0     3006 2023-10-24 17:19:29.261718 hyperiontf-0.3.5/src/hyperiontf/helpers/string_helpers.py
+-rw-r--r--   0        0        0    11683 2024-02-26 19:03:16.899116 hyperiontf-0.3.5/src/hyperiontf/helpers/wagner_fischer.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:42:34.988634 hyperiontf-0.3.5/src/hyperiontf/image_processing/__init__.py
+-rw-r--r--   0        0        0    10645 2024-04-03 12:42:34.989181 hyperiontf-0.3.5/src/hyperiontf/image_processing/image.py
+-rw-r--r--   0        0        0        0 2023-10-24 17:19:29.261800 hyperiontf-0.3.5/src/hyperiontf/infrastructure/__init__.py
+-rw-r--r--   0        0        0     1725 2023-10-24 17:19:29.261909 hyperiontf-0.3.5/src/hyperiontf/infrastructure/event_blorker.py
+-rw-r--r--   0        0        0       92 2023-10-24 17:19:29.262061 hyperiontf-0.3.5/src/hyperiontf/logging/__init__.py
+-rwxr-xr-x   0        0        0     2674 2023-10-24 17:19:29.262347 hyperiontf-0.3.5/src/hyperiontf/logging/assets/build
+-rw-r--r--   0        0        0      935 2023-10-24 17:19:29.262483 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/button-border-colors.css
+-rw-r--r--   0        0        0      252 2023-10-24 17:19:29.262596 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/button.css
+-rw-r--r--   0        0        0      665 2023-10-24 17:19:29.262691 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/colors.css
+-rw-r--r--   0        0        0      392 2023-10-24 17:19:29.262890 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/filter-bar.css
+-rw-r--r--   0        0        0     1048 2023-10-24 17:19:29.263063 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/header.css
+-rw-r--r--   0        0        0     1677 2023-10-24 17:19:29.263197 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/icon-color-filters.css
+-rw-r--r--   0        0        0    38307 2023-10-24 17:19:29.263493 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/icon-images.css
+-rw-r--r--   0        0        0      285 2023-10-24 17:19:29.263707 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/icon.css
+-rw-r--r--   0        0        0     2496 2023-10-24 17:19:29.263813 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/log-message.css
+-rw-r--r--   0        0        0      135 2023-10-24 17:19:29.263926 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/misc.css
+-rw-r--r--   0        0        0      884 2023-10-24 17:19:29.264039 hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/tooltip.css
+-rw-r--r--   0        0        0      939 2023-10-24 17:19:29.264212 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/app.js
+-rw-r--r--   0        0        0     4974 2023-10-24 17:19:29.264338 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/config.js
+-rw-r--r--   0        0        0    11226 2023-10-24 17:19:29.264443 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/controlPanel.js
+-rw-r--r--   0        0        0     1356 2023-10-24 17:19:29.264516 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/eventBroker.js
+-rw-r--r--   0        0        0     2136 2023-10-24 17:19:29.264623 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/helpers.js
+-rw-r--r--   0        0        0    40401 2023-10-24 17:19:29.264774 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/line.js
+-rw-r--r--   0        0        0     5490 2023-10-24 17:19:29.264943 hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/logger.js
+-rw-r--r--   0        0        0     1192 2023-10-24 17:19:29.265092 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/assert-true.svg
+-rw-r--r--   0        0        0     2530 2023-10-24 17:19:29.265196 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/backtrace.svg
+-rw-r--r--   0        0        0     1424 2023-10-24 17:19:29.265281 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/collapse.svg
+-rw-r--r--   0        0        0      724 2023-10-24 17:19:29.265354 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/column.svg
+-rw-r--r--   0        0        0     1936 2023-10-24 17:19:29.265448 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/debug.svg
+-rw-r--r--   0        0        0     1371 2023-10-24 17:19:29.265561 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/error.svg
+-rw-r--r--   0        0        0     1432 2023-10-24 17:19:29.265680 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/expand.svg
+-rw-r--r--   0        0        0     3067 2023-10-24 17:19:29.265778 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/fatal.svg
+-rw-r--r--   0        0        0     1852 2023-10-24 17:19:29.265906 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/info.svg
+-rw-r--r--   0        0        0      615 2023-10-24 17:19:29.266003 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/level.svg
+-rw-r--r--   0        0        0     2582 2023-10-24 17:19:29.266106 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/log.svg
+-rw-r--r--   0        0        0     1347 2023-10-24 17:19:29.266198 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/page-source.svg
+-rw-r--r--   0        0        0      847 2023-10-24 17:19:29.266288 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/screen-snap.svg
+-rw-r--r--   0        0        0     3786 2023-10-24 17:19:29.266369 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/timestamp.svg
+-rw-r--r--   0        0        0     2555 2023-10-24 17:19:29.266474 hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/warning.svg
+-rw-r--r--   0        0        0    67094 2023-10-24 17:19:29.266730 hyperiontf-0.3.5/src/hyperiontf/logging/assets/template.html
+-rw-r--r--   0        0        0     2485 2023-10-24 17:19:29.267068 hyperiontf-0.3.5/src/hyperiontf/logging/file_handler.py
+-rw-r--r--   0        0        0     4531 2024-03-05 20:05:34.921553 hyperiontf-0.3.5/src/hyperiontf/logging/formatter.py
+-rw-r--r--   0        0        0      715 2023-10-24 17:19:29.267216 hyperiontf-0.3.5/src/hyperiontf/logging/helpers.py
+-rw-r--r--   0        0        0     1606 2024-02-26 19:03:16.899820 hyperiontf-0.3.5/src/hyperiontf/logging/log_depth_manager.py
+-rw-r--r--   0        0        0     2115 2023-10-24 17:19:29.267380 hyperiontf-0.3.5/src/hyperiontf/logging/log_file_manager.py
+-rw-r--r--   0        0        0     4642 2023-10-24 17:19:29.267468 hyperiontf-0.3.5/src/hyperiontf/logging/logger.py
+-rw-r--r--   0        0        0    13824 2024-04-03 12:42:34.989611 hyperiontf-0.3.5/src/hyperiontf/typing.py
+-rw-r--r--   0        0        0      831 2024-02-26 19:03:16.901409 hyperiontf-0.3.5/src/hyperiontf/ui/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.901460 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.901661 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/__init__.py
+-rw-r--r--   0        0        0     8365 2024-04-03 12:42:34.990060 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/element.py
+-rw-r--r--   0        0        0     1212 2024-02-26 19:03:16.901932 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/map_exception.py
+-rw-r--r--   0        0        0     1626 2024-02-26 19:03:16.902046 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/map_locator.py
+-rw-r--r--   0        0        0     6054 2024-04-03 12:42:34.990669 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/page.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.902166 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/__init__.py
+-rw-r--r--   0        0        0     1871 2024-02-26 19:03:16.902363 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/assert_stale_element_reference.py
+-rw-r--r--   0        0        0    11703 2024-04-03 12:42:34.990880 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/element.py
+-rw-r--r--   0        0        0      938 2024-02-26 19:03:16.902655 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/map_exception.py
+-rw-r--r--   0        0        0     1732 2024-02-26 19:03:16.902788 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/map_locator.py
+-rw-r--r--   0        0        0     6942 2024-04-03 12:42:34.991442 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/page.py
+-rw-r--r--   0        0        0     1693 2024-02-26 19:03:16.903054 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/selenium_to_playwright_script.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.903130 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/__init__.py
+-rw-r--r--   0        0        0     9722 2024-04-03 12:42:34.991968 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/element.py
+-rw-r--r--   0        0        0     1268 2024-02-26 19:03:16.903410 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/map_exception.py
+-rw-r--r--   0        0        0     1204 2024-03-05 20:05:34.922374 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/map_locator.py
+-rw-r--r--   0        0        0    13927 2024-04-03 12:42:34.992623 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/page.py
+-rw-r--r--   0        0        0     4320 2024-04-03 12:42:34.993551 hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/win_app_driver.py
+-rw-r--r--   0        0        0     7578 2024-03-05 20:05:34.923622 hyperiontf-0.3.5/src/hyperiontf/ui/automation_adapter_manager.py
+-rw-r--r--   0        0        0     7038 2023-10-24 17:19:29.268661 hyperiontf-0.3.5/src/hyperiontf/ui/by.py
+-rw-r--r--   0        0        0    14333 2024-02-26 19:03:16.904934 hyperiontf-0.3.5/src/hyperiontf/ui/color.py
+-rw-r--r--   0        0        0     5389 2024-03-05 20:05:34.924013 hyperiontf-0.3.5/src/hyperiontf/ui/content_manager.py
+-rw-r--r--   0        0        0     3285 2023-10-24 17:19:29.268885 hyperiontf-0.3.5/src/hyperiontf/ui/context_manager.py
+-rw-r--r--   0        0        0        0 2023-10-24 17:19:29.269056 hyperiontf-0.3.5/src/hyperiontf/ui/decorators/__init__.py
+-rw-r--r--   0        0        0     5322 2024-02-26 19:03:16.906050 hyperiontf-0.3.5/src/hyperiontf/ui/decorators/autolog_class_method_helper.py
+-rw-r--r--   0        0        0     4827 2024-02-26 19:03:16.906693 hyperiontf-0.3.5/src/hyperiontf/ui/decorators/element_accessor.py
+-rw-r--r--   0        0        0     3237 2024-03-05 20:05:34.924231 hyperiontf-0.3.5/src/hyperiontf/ui/decorators/element_error_recovery.py
+-rw-r--r--   0        0        0     9074 2023-10-24 17:19:29.269717 hyperiontf-0.3.5/src/hyperiontf/ui/decorators/page_object_helpers.py
+-rw-r--r--   0        0        0     1424 2023-10-24 17:19:29.269866 hyperiontf-0.3.5/src/hyperiontf/ui/desktop_window.py
+-rw-r--r--   0        0        0    46855 2024-04-03 12:42:34.994475 hyperiontf-0.3.5/src/hyperiontf/ui/element.py
+-rw-r--r--   0        0        0    10024 2024-02-26 19:03:16.908802 hyperiontf-0.3.5/src/hyperiontf/ui/elements.py
+-rw-r--r--   0        0        0        0 2024-02-26 19:03:16.908896 hyperiontf-0.3.5/src/hyperiontf/ui/eql/__init__.py
+-rw-r--r--   0        0        0     1749 2024-02-26 19:03:16.909075 hyperiontf-0.3.5/src/hyperiontf/ui/eql/elements_query_language.ebnf
+-rw-r--r--   0        0        0     4934 2024-02-26 19:03:16.909237 hyperiontf-0.3.5/src/hyperiontf/ui/eql/executor.py
+-rw-r--r--   0        0        0     2430 2024-02-26 19:03:16.909434 hyperiontf-0.3.5/src/hyperiontf/ui/eql/lexer.py
+-rw-r--r--   0        0        0     4301 2024-02-26 19:03:16.909532 hyperiontf-0.3.5/src/hyperiontf/ui/eql/parser.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:42:34.994577 hyperiontf-0.3.5/src/hyperiontf/ui/helpers/__init__.py
+-rw-r--r--   0        0        0     1981 2024-04-03 12:42:34.995201 hyperiontf-0.3.5/src/hyperiontf/ui/helpers/prepare_expect_object.py
+-rw-r--r--   0        0        0    10368 2024-04-03 12:42:34.995622 hyperiontf-0.3.5/src/hyperiontf/ui/helpers/visual.py
+-rw-r--r--   0        0        0     1531 2024-03-05 20:05:34.924431 hyperiontf-0.3.5/src/hyperiontf/ui/iframe.py
+-rw-r--r--   0        0        0    18257 2024-02-26 19:03:16.910135 hyperiontf-0.3.5/src/hyperiontf/ui/locatable.py
+-rw-r--r--   0        0        0     1505 2023-10-24 17:19:29.270606 hyperiontf-0.3.5/src/hyperiontf/ui/mobile_screen.py
+-rw-r--r--   0        0        0     9255 2024-04-03 12:42:34.996064 hyperiontf-0.3.5/src/hyperiontf/ui/page_object_base.py
+-rw-r--r--   0        0        0    19960 2024-04-03 12:42:34.997042 hyperiontf-0.3.5/src/hyperiontf/ui/viewport_manager.py
+-rw-r--r--   0        0        0     2576 2024-04-03 12:42:34.998126 hyperiontf-0.3.5/src/hyperiontf/ui/webpage.py
+-rw-r--r--   0        0        0     1762 2024-02-26 19:03:16.910808 hyperiontf-0.3.5/src/hyperiontf/ui/webview.py
+-rw-r--r--   0        0        0      816 2024-02-26 19:03:16.911169 hyperiontf-0.3.5/src/hyperiontf/ui/widget.py
+-rw-r--r--   0        0        0     7948 2024-04-03 12:42:34.999034 hyperiontf-0.3.5/src/hyperiontf/ui/window_manager.py
+-rw-r--r--   0        0        0    62630 1970-01-01 00:00:00.000000 hyperiontf-0.3.5/PKG-INFO
```

### Comparing `hyperiontf-0.2.5/LICENSE` & `hyperiontf-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/README.md` & `hyperiontf-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/__init__.py` & `hyperiontf-0.3.5/src/hyperiontf/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,16 @@
 from .logging import getLogger
 from .assertions import expect, verify
 from .api import Client as RESTClient
 from .configuration import config
 
 from .fs import File, Dir
 
+from .image_processing.image import Image
+
 __all__ = [
     "By",
     "getLogger",
     "WebPage",
     "MobileScreen",
     "DesktopWindow",
     "Widget",
@@ -47,8 +49,9 @@
     "expect",
     "verify",
     "config",
     "RESTClient",
     "File",
     "Dir",
     "Color",
+    "Image",
 ]
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/api/rest_client/client.py` & `hyperiontf-0.3.5/src/hyperiontf/api/rest_client/client.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/api/rest_client/request.py` & `hyperiontf-0.3.5/src/hyperiontf/api/rest_client/request.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/api/rest_client/response.py` & `hyperiontf-0.3.5/src/hyperiontf/api/rest_client/response.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/decorators.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/expect.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/expect.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 from typing import Optional, Type, Union, Any
 from hyperiontf.logging.logger import Logger
 from hyperiontf.ui.color import Color
+from hyperiontf.image_processing.image import Image
 from .decorators import auto_log, type_check
 from hyperiontf.assertions.strategy.default_strategy import DefaultStrategy
 from hyperiontf.assertions.strategy.numeric_strategy import NumericStrategy
 from hyperiontf.assertions.strategy.string_strategy import StringStrategy
 from hyperiontf.assertions.strategy.array_strategy import ArrayStrategy
 from hyperiontf.assertions.strategy.dict_strategy import DictStrategy
 from hyperiontf.assertions.strategy.color_strategy import ColorStrategy
 from hyperiontf.assertions.strategy.filesystem_strategy import FileSystemStrategy
+from hyperiontf.assertions.strategy.image_strategy import ImageStrategy
 from .expectation_result import ExpectationResult
+from .image_expectation_result import ImageExpectationResult
 
 STRATEGIES_MAP = {
     "bool": NumericStrategy,
     "int": NumericStrategy,
     "float": NumericStrategy,
     "str": StringStrategy,
     "list": ArrayStrategy,
     "set": ArrayStrategy,
     "tuple": ArrayStrategy,
     "dict": DictStrategy,
     "Color": ColorStrategy,
     "File": FileSystemStrategy,
     "Dir": FileSystemStrategy,
+    "Image": ImageStrategy,
 }
 
 
 class Expect:
     """
     A central class in the testing framework that provides a fluent interface for asserting
     various conditions on a given value. It dynamically selects an appropriate strategy
@@ -88,15 +92,15 @@
             STRATEGIES_MAP.get(actual_value.__class__.__name__, DefaultStrategy)(
                 actual_value
             )
         )
         self.prefix = prefix
 
     @auto_log
-    def to_be(self, expected_value: Any) -> ExpectationResult:
+    def to_be(self, expected_value: Any) -> Type[ExpectationResult]:
         """
         Asserts that the actual value is equal to the expected value. The definition of equality
         is strategy-specific: for numeric types, it means numerical equality; for strings, it means
         exact string match; for files, it may involve comparing file contents or checksums; and for
         collections, it could mean structural equality.
 
         This method is applicable across various types, including but not limited to numbers, strings,
@@ -137,15 +141,15 @@
             The interpretation of "containment" varies by the type of the actual value. For exact
             behavior and limitations, refer to the documentation of the specific strategy classes
             applicable to the actual value's type.
         """
         return self.strategy.to_contain(expected_value)  # type: ignore
 
     @auto_log
-    def not_to_be(self, expected_value: Any) -> ExpectationResult:
+    def not_to_be(self, expected_value: Any) -> Type[ExpectationResult]:
         """
         Asserts that the actual value is not equal to the expected value. The interpretation of inequality
         is strategy-specific and can range from simple value mismatches to complex structural differences
         in collections or files.
 
         This method is universally applicable, suitable for numbers, strings, collections (lists, sets, tuples),
         dictionaries, and file system entities, ensuring that the actual value does not match the expected value
@@ -1107,15 +1111,15 @@
             Utilizing this assertion ensures that file-specific operations, such as reading or writing content, are
             performed on valid file entities, aiding in the prevention of errors and the enforcement of filesystem
             integrity within applications or testing environments.
         """
         return self.strategy.to_be_file()  # type: ignore
 
     @auto_log
-    @type_check(supported_strategies=[FileSystemStrategy])
+    @type_check(supported_strategies=[FileSystemStrategy, ImageStrategy])
     def to_exist(self) -> ExpectationResult:
         """
         Asserts that the actual filesystem entity, whether a file or directory, exists at the specified path. This method
         is vital for confirming the presence of expected filesystem objects before proceeding with operations that require
         their existence, such as opening files or traversing directories.
 
         Returns:
@@ -1125,14 +1129,30 @@
         Note:
             This assertion is fundamental to ensuring the readiness of the filesystem for operations, supporting the
             robust handling of file and directory access, modification, and validation tasks.
         """
         return self.strategy.to_exist()  # type: ignore
 
     @auto_log
+    @type_check(supported_strategies=[FileSystemStrategy, ImageStrategy])
+    def not_to_exist(self) -> ExpectationResult:
+        """
+        Asserts that the actual filesystem entity, whether a file or directory, does not exists at the specified path.
+
+        Returns:
+            ExpectationResult: An object representing the result of the check, indicating whether the filesystem entity
+                               does not exists, including the path checked and whether the check passed or failed.
+
+        Note:
+            This assertion is fundamental to ensuring the readiness of the filesystem for operations, supporting the
+            robust handling of file and directory access, modification, and validation tasks.
+        """
+        return self.strategy.not_to_exist()  # type: ignore
+
+    @auto_log
     @type_check(supported_strategies=[FileSystemStrategy])
     def to_be_directory(self) -> ExpectationResult:
         """
         Asserts that the actual value represents a directory in the filesystem. This method is critical for validating
         that a given path or entity corresponds to a directory, ensuring that operations expecting to interact with
         directory structures, such as listing contents or creating subdirectories, are feasible.
 
@@ -1722,7 +1742,124 @@
             This assertion supports nuanced color comparisons, acknowledging slight variations in color and transparency
             that may be acceptable in many applications. It allows for flexible validation of color properties, ensuring
             that colors are similar to an acceptable degree based on the provided thresholds.
         """
         return self.strategy.to_be_approximately_equal(  # type: ignore
             expected_value, percentage_threshold, alpha_threshold
         )  # type: ignore
+
+    @auto_log
+    @type_check(supported_strategies=[ImageStrategy])
+    def to_be_similar(
+        self,
+        expected_value: Union[str, Image],
+        mismatch_threshold: float = 10,
+        compare_regions: Optional[list] = None,
+        exclude_regions: Optional[list] = None,
+    ) -> ImageExpectationResult:
+        """
+        Asserts that the actual image is similar to the expected image within a defined mismatch threshold,
+        optionally considering or ignoring specific regions for a more targeted comparison.
+
+        This method compares the actual image to the expected image, allowing for a specified degree of variation
+        between them as defined by the mismatch_threshold. The comparison can be fine-tuned by specifying regions
+        of the image to specifically compare or exclude from the comparison. The comparison algorithm assesses
+        similarity on a pixel-by-pixel basis, adjusted for the designated threshold and regional focus.
+
+        The mismatch_threshold parameter defines the acceptable percentage difference between the images, allowing
+        for minor variations due to compression artifacts, rendering differences, or other acceptable noise. The
+        method supports selective focus through compare_regions and selective ignorance via exclude_regions, enabling
+        nuanced comparison scenarios where full image matching is unnecessary or impractical.
+
+        Args:
+            expected_value (Image): The expected image to compare against the actual image. It should be an instance
+                                    of the Image class, encapsulating the image data along with any relevant metadata.
+            mismatch_threshold (float): The permissible percentage difference between the images, representing the
+                                        tolerance for discrepancies to still consider the images as similar.
+            compare_regions (Optional[list]): Optional list of regions to specifically include in the comparison, with
+                                              each region defined as a dictionary containing 'x', 'y', 'width', and 'height'.
+            exclude_regions (Optional[list]): Optional list of regions to exclude from the comparison, with each region
+                                              similarly defined as a dictionary.
+
+        Returns:
+            ImageExpectationResult: An object encapsulating the comparison result, indicating whether the actual image
+                                    is considered similar to the expected image within the threshold and any specified
+                                    regional focus. The result includes a similarity score and may include a difference
+                                    image for visualization.
+        """
+        return self.strategy.to_be_similar(expected_value, mismatch_threshold, compare_regions, exclude_regions)  # type: ignore
+
+    @auto_log
+    @type_check(supported_strategies=[ImageStrategy])
+    def to_match_in_specified_regions(
+        self,
+        expected_value: Image,
+        compare_regions: list,
+        mismatch_threshold: float = 0,
+    ) -> ImageExpectationResult:
+        """
+        Asserts that selected regions within the actual image match corresponding regions in the expected image,
+        within an optional mismatch threshold. This method allows focused comparison on parts of the images that
+        are of particular interest, potentially ignoring the rest of the image content.
+
+        The compare_regions argument should be a list of dictionaries, each defining a region with 'x', 'y', 'width',
+        and 'height' keys. The comparison assesses each specified region independently, comparing the actual image's
+        region against the corresponding region in the expected image. If a mismatch_threshold is provided, minor
+        differences between the compared regions up to the specified threshold are tolerated.
+
+        This method is especially useful for scenarios where only certain parts of the image are relevant for
+        comparison, allowing testers to specify exactly which regions should match between the actual and expected
+        images, thus providing granular control over the comparison process.
+
+        Args:
+            expected_value (Image): The expected image to compare against the actual image. It should be an instance
+                                    of the Image class, containing the image data along with any relevant metadata.
+            compare_regions (list): A list of dictionaries, each specifying a rectangular region in the images to
+                                    compare. Each dictionary should have 'x', 'y', 'width', and 'height' keys.
+            mismatch_threshold (float, optional): An optional threshold for allowed mismatch percentage within the
+                                                  specified regions, defaulting to 0 for an exact match requirement.
+
+        Returns:
+            ImageExpectationResult: An object encapsulating the comparison result, indicating whether the specified
+                                    regions of the actual image match those in the expected image within the given
+                                    tolerance. Includes detailed results for each region compared, and a comprehensive
+                                    match assessment.
+        """
+        return self.strategy.to_match_in_specified_regions(expected_value, compare_regions, mismatch_threshold)  # type: ignore
+
+    @auto_log
+    @type_check(supported_strategies=[ImageStrategy])
+    def to_match_excluding_regions(
+        self,
+        expected_value: Image,
+        exclude_regions: list,
+        mismatch_threshold: float = 0,
+    ) -> ImageExpectationResult:
+        """
+        Asserts that the actual image matches the expected image, excluding the differences in specified regions,
+        within a permissible mismatch threshold. This method allows exclusion of certain image areas from the
+        comparison, focusing the match assessment on the remaining regions.
+
+        The exclude_regions argument should be a list of dictionaries, each dictating a region to be excluded with
+        'x', 'y', 'width', and 'height' keys. These regions are ignored during the comparison, enabling testers to
+        isolate and exclude areas with known or irrelevant differences. The mismatch_threshold parameter allows
+        a defined tolerance level for the matching process in the non-excluded areas of the images.
+
+        This functionality is particularly valuable when certain image sections are dynamic or irrelevant to the
+        test's intent, enabling precise and focused image analysis that disregards these areas.
+
+        Args:
+            expected_value (Image): The expected image to compare against the actual image, encapsulating the image
+                                    data along with any pertinent metadata.
+            exclude_regions (list): A list of dictionaries, each specifying a rectangular region in the images to
+                                    be excluded from the comparison. Each dictionary should define 'x', 'y', 'width',
+                                    and 'height' keys.
+            mismatch_threshold (float, optional): An optional threshold defining the allowed percentage of mismatch
+                                                 in the non-excluded areas, with 0 requiring exact match.
+
+        Returns:
+            ImageExpectationResult: An object detailing the comparison results, indicating whether the non-excluded
+                                    regions of the actual image match the expected image within the set mismatch
+                                    tolerance. The result object provides an aggregate assessment and may include
+                                    detailed analysis or visualization data.
+        """
+        return self.strategy.to_match_excluding_regions(expected_value, exclude_regions, mismatch_threshold)  # type: ignore
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/expectation_result.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/expectation_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,26 +200,26 @@
 
         Args:
             other (bool or ExpectationResult): The object to compare with.
 
         Returns:
             bool: True if equal, False otherwise.
         """
-        if isinstance(other, (bool, ExpectationResult)):
+        if isinstance(other, (bool, ExpectationResult, int)):
             return self.result == bool(other)
         return NotImplemented
 
     def __str__(self):
         """
         Returns the informal string representation of the ExpectationResult.
 
         Returns:
             str: A concise, user-friendly description of the comparison.
         """
-        return f"[{self.sender}] {self.prefix} {self.action} {self.expectation_type} {self.status}.\n{self.comparison_info}"
+        return f"[{self.sender}] {self.prefix or ''} {self.action} {self.expectation_type} {self.status}.\n{self.comparison_info}"
 
     def __repr__(self):
         """
         Returns the formal string representation of the ExpectationResult.
 
         Returns:
             str: A string that represents the object, including all attributes.
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/helpers.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/array_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/array_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/color_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/color_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/decorators.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/decorators.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/default_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/default_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/dict_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/dict_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/filesystem_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/filesystem_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/numeric_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/numeric_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/assertions/strategy/string_strategy.py` & `hyperiontf-0.3.5/src/hyperiontf/assertions/strategy/string_strategy.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/configuration/capabilities.py` & `hyperiontf-0.3.5/src/hyperiontf/configuration/capabilities.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/configuration/config.py` & `hyperiontf-0.3.5/src/hyperiontf/configuration/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from hyperiontf.helpers.string_helpers import camel_to_snake_case
 from hyperiontf.configuration.sections import (
     Logger,
     Element,
     PageObject,
     DesktopCapabilities,
     WebCapabilities,
+    Visual,
 )
 from hyperiontf.configuration.sections import Rest, MobileCapabilities
 
 import os
 
 
 @Singleton
@@ -26,14 +27,15 @@
         self.logger = Logger()
         self.page_object = PageObject()
         self.element = Element()
         self.web_capabilities = WebCapabilities()
         self.mobile_capabilities = MobileCapabilities()
         self.desktop_capabilities = DesktopCapabilities()
         self.rest = Rest()
+        self.visual = Visual()
 
     def _parse_config_data(self, data):
         """
         Parse configuration data and update the sections.
 
         Parameters:
             data (dict): Dictionary containing the configuration data.
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/configuration/section.py` & `hyperiontf-0.3.5/src/hyperiontf/configuration/section.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/configuration/sections/web_capabilities.py` & `hyperiontf-0.3.5/src/hyperiontf/configuration/sections/web_capabilities.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/executors/pytest/fixture.py` & `hyperiontf-0.3.5/src/hyperiontf/executors/pytest/fixture.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/executors/pytest/logger_setup.py` & `hyperiontf-0.3.5/src/hyperiontf/executors/pytest/logger_setup.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/fs/dir.py` & `hyperiontf-0.3.5/src/hyperiontf/fs/dir.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/fs/file.py` & `hyperiontf-0.3.5/src/hyperiontf/fs/file.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/wait.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/wait.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/decorators/without_failure.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/decorators/without_failure.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/dict_diff.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/dict_diff.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/dict_heplers.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/dict_heplers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/extend_instance.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/extend_instance.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/own_methods_helper.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/own_methods_helper.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/rect_helpers.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/rect_helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/string_helpers.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/string_helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/helpers/wagner_fischer.py` & `hyperiontf-0.3.5/src/hyperiontf/helpers/wagner_fischer.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/infrastructure/event_blorker.py` & `hyperiontf-0.3.5/src/hyperiontf/infrastructure/event_blorker.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/build` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/build`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/button-border-colors.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/button-border-colors.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/colors.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/colors.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/header.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/header.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/icon-color-filters.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/icon-color-filters.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/icon-images.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/icon-images.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/log-message.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/log-message.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/css/tooltip.css` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/css/tooltip.css`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/app.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/config.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/config.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/controlPanel.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/controlPanel.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/eventBroker.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/eventBroker.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/helpers.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/helpers.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/line.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/line.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/js/logger.js` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/js/logger.js`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/assert-true.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/assert-true.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/backtrace.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/backtrace.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/collapse.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/collapse.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/column.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/column.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/debug.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/debug.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/error.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/error.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/expand.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/expand.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/fatal.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/fatal.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/info.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/info.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/level.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/level.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/log.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/log.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/page-source.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/page-source.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/screen-snap.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/screen-snap.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/timestamp.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/timestamp.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/svg/warning.svg` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/svg/warning.svg`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/assets/template.html` & `hyperiontf-0.3.5/src/hyperiontf/logging/assets/template.html`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/file_handler.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/file_handler.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/formatter.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/helpers.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/log_depth_manager.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/log_depth_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/log_file_manager.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/log_file_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/logging/logger.py` & `hyperiontf-0.3.5/src/hyperiontf/logging/logger.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/typing.py` & `hyperiontf-0.3.5/src/hyperiontf/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
 WEB_FAMILY = [AutomationTool.SELENIUM, AutomationTool.PLAYWRIGHT]
 MOBILE_FAMILY = [AutomationTool.APPIUM]
 DESKTOP_FAMILY = [
     AutomationTool.APPIUM,
     AutomationTool.AUTOIT,
     AutomationTool.XDOTOOL,
     AutomationTool.PYAUTOGUI,
+    AutomationTool.WIN_APP_DRIVER,
 ]
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 # Log Sources
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
@@ -316,14 +317,29 @@
     LT: ComparisonOperator = "<"
     LE: ComparisonOperator = "<="
     GT: ComparisonOperator = ">"
     GE: ComparisonOperator = ">="
 
 
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+# Visual Section
+# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
+
+VisualModeType = Literal[
+    "collect",
+    "compare",
+]
+
+
+class VisualMode:
+    COLLECT: VisualModeType = "collect"
+    COMPARE: VisualModeType = "compare"
+
+
+# - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 # Rest Client Typing
 # - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -
 
 HTTPMethodType = Literal["GET", "POST", "PUT", "DELETE", "HEAD", "OPTIONS", "PATCH"]
 
 
 class HTTPMethod:
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/__init__.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/element.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,15 @@
         Submit the form associated with the element (if applicable).
 
         Raises:
             HyperionException: If any exception occurs during the form submission.
         """
         self.element.submit()
 
+    @property
     @map_exception
     def screenshot_as_base64(self):
         return self.element.screenshot_as_base64
 
     @map_exception
     def screenshot(self, path):
         return self.element.screenshot(path)
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/map_exception.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/map_locator.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/appium/page.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/appium/page.py`

 * *Files 8% similar despite different names*

```diff
@@ -182,7 +182,34 @@
                 "title": "Native app context page source",
                 "type": "html",
                 "url": base_64_src_url,
             }
         )
 
         return attachments
+
+    @property
+    @map_exception
+    def size(self):
+        return self.driver.get_window_size()
+
+    @property
+    @map_exception
+    def location(self):
+        return self.driver.get_window_position()
+
+    @property
+    @map_exception
+    def rect(self):
+        return self.driver.get_window_rect()
+
+    @map_exception
+    def set_window_size(self, width, height):
+        self.driver.set_window_size(width, height)
+
+    @map_exception
+    def set_window_location(self, x, y):
+        self.driver.set_window_position(x, y)
+
+    @map_exception
+    def set_window_rect(self, x, y, width, height):
+        self.driver.set_window_rect(x, y, width, height)
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/assert_stale_element_reference.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/assert_stale_element_reference.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/element.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import base64
+
 from .map_locator import convert_locator
 from .map_exception import map_exception
 from .assert_stale_element_reference import assert_stale_reference
 from hyperiontf.ui import By
 from hyperiontf.typing import (
     LocatorStrategies,
     UnsupportedLocatorException,
@@ -356,18 +358,18 @@
             f"Unsupported {locator.by} locator for Selenium WebDriver"
         )
 
     @assert_stale_reference
     def get_iframe_content(self):
         return self.element.content_frame()
 
+    @property
     @map_exception
     @assert_stale_reference
     def screenshot_as_base64(self):
-        # async API, avoiding it as we work in sync mode
-        return ""
+        screenshot_as_bytes = self.element.screenshot()
+        return base64.b64encode(screenshot_as_bytes).decode("utf-8")
 
     @map_exception
     @assert_stale_reference
     def screenshot(self, path):
-        # async API, avoiding it as we work in sync mode
-        pass
+        self.element.screenshot(path=path)
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/map_exception.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/map_locator.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/page.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/page.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .selenium_to_playwright_script import convert_to_function
 from .element import Element
 from hyperiontf.typing import LocatorStrategies
 
 import base64
 
 logger = getLogger()
+adapter_logger = getLogger("PlaywrightAdapter")
 
 if config.logger.intercept_selenium_logs:
     logger.merge_logger_stream(AutomationTool.SELENIUM)
 
 
 class Page:
     playwright = None
@@ -164,14 +165,57 @@
         self.page.screenshot(path=path)
 
     @property
     @map_exception
     def page_source(self):
         return self.page.content()
 
+    @property
+    @map_exception
+    def size(self):
+        adapter_logger.debug(
+            "Window size getter:\nPlaywright does not actually manage window "
+            "size!\nReturning viewport size instead!"
+        )
+        return self.page.viewport_size
+
+    @property
+    @map_exception
+    def location(self):
+        adapter_logger.debug(
+            "Window location getter:\nPlaywright does not actually manage window "
+            "location!\nReturning zero coordinate instead!"
+        )
+        return {"x": 0, "y": 0}
+
+    @map_exception
+    def set_window_size(self, width, height):
+        adapter_logger.debug(
+            "Window size setter:\nPlaywright does not actually manage window "
+            "size!\nSetting viewport size instead!"
+        )
+        self.page.set_viewport_size({"width": width, "height": height})
+
+    @map_exception
+    def set_window_location(self, x_, y_):
+        adapter_logger.warning(
+            "Window location setter:\nPlaywright does not actually manage window "
+            "location!\nNothing to do here!"
+        )
+
+    @map_exception
+    def set_window_rect(self, x, y, width, height):
+        self.set_window_location(x, y)
+        self.set_window_size(width, height)
+
+    @property
+    @map_exception
+    def rect(self):
+        return {**self.size, **self.location}
+
     def dump(self):
         attachments = []
 
         self.switch_to_default_content()
 
         base_64_img_URL = f"data:image/png;base64,{self.screenshot_as_base64}"
         attachments.append(
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/playwright/selenium_to_playwright_script.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/playwright/selenium_to_playwright_script.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/element.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,15 @@
         if locator.by == LocatorStrategies.SCRIPT:
             return self.page.execute_script(locator.value, self.element)
 
         raise UnsupportedLocatorException(
             f"Unsupported {locator.by} locator for Selenium WebDriver"
         )
 
+    @property
     @map_exception
     def screenshot_as_base64(self):
         return self.element.screenshot_as_base64
 
     @map_exception
     def screenshot(self, path):
         return self.element.screenshot(path)
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/map_exception.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/map_exception.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/map_locator.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/map_locator.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/adapters/selenium/page.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/adapters/selenium/page.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .map_exception import map_exception
 from .element import Element
 
 from hyperiontf.typing import LocatorStrategies
 
 import base64
 
+from .win_app_driver import WinAppDriver
+
 logger = getLogger()
 
 if config.logger.intercept_selenium_logs:
     logger.merge_logger_stream(AutomationTool.SELENIUM)
 
 BROWSER_START_METHODS = {
     Browser.CHROME: "start_chrome_browser",
@@ -353,30 +355,62 @@
             file.write(screenshot_as_bytes)
 
     @property
     @map_exception
     def page_source(self):
         return self.driver.page_source
 
+    @property
+    @map_exception
+    def size(self):
+        return self.driver.get_window_size()
+
+    @property
+    @map_exception
+    def location(self):
+        return self.driver.get_window_position()
+
+    @property
+    @map_exception
+    def rect(self):
+        return self.driver.get_window_rect()
+
+    @map_exception
+    def set_window_size(self, width, height):
+        self.driver.set_window_size(width, height)
+
+    @map_exception
+    def set_window_location(self, x, y):
+        self.driver.set_window_position(x, y)
+
+    @map_exception
+    def set_window_rect(self, x, y, width, height):
+        self.driver.set_window_rect(x, y, width, height)
+
     def dump(self):
         attachments = []
+        if isinstance(self.driver, WinAppDriver):
+            source_code_content_type = "xml"
+        else:
+            source_code_content_type = "html"
+
         for index, window in enumerate(self.window_handles):
             self.switch_to_window(window)
 
             base_64_img_URL = f"data:image/png;base64,{self.screenshot_as_base64}"
             attachments.append(
                 {
                     "title": f"Window {index + 1} screenshot",
                     "type": "image",
                     "url": base_64_img_URL,
                 }
             )
 
             base_64_src_url = (
-                f"data:text/html;base64,"
+                f"data:text/{source_code_content_type};base64,"
                 f"{base64.b64encode(self.page_source.encode('utf-8')).decode('utf-8')}"
             )
             attachments.append(
                 {
                     "title": f"Window {index + 1} page source",
                     "type": "html",
                     "url": base_64_src_url,
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/automation_adapter_manager.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/automation_adapter_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/by.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/by.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/color.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/color.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/content_manager.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/content_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/context_manager.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/context_manager.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/decorators/autolog_class_method_helper.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/decorators/autolog_class_method_helper.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/decorators/element_accessor.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/decorators/element_accessor.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/decorators/element_error_recovery.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/decorators/element_error_recovery.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/decorators/page_object_helpers.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/decorators/page_object_helpers.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/desktop_window.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/desktop_window.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/element.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/element.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,35 @@
 import time
-from typing import Optional, Union, List, Any
+from typing import Optional, Union, List, Type
 
 from hyperiontf.logging import getLogger
 from hyperiontf.typing import NoSuchElementException
 from hyperiontf.ui.decorators.element_error_recovery import error_recovery
 
 from .locatable import LocatableElement
-from hyperiontf.assertions.expect import Expect
 from hyperiontf.assertions.expectation_result import ExpectationResult
 from hyperiontf.helpers.decorators.wait import wait
 from hyperiontf.helpers.rect_helpers import are_rectangles_equal
+from hyperiontf.image_processing.image import Image
+from hyperiontf.ui.helpers.prepare_expect_object import prepare_expect_object
+
+from hyperiontf.configuration import config
+from hyperiontf.typing import VisualModeType
+from hyperiontf.assertions.image_expectation_result import ImageExpectationResult
+
+from hyperiontf.ui.helpers.visual import (
+    verify_visual_match,
+    verify_visual_exclusion_match,
+    verify_visual_match_in_regions,
+)
+from hyperiontf.ui.helpers.visual import (
+    assert_visual_match,
+    assert_visual_match_in_regions,
+    assert_visual_exclusion_match,
+)
 
 logger = getLogger("Element")
 
 
 class Element(LocatableElement):
     def __init__(self, parent, locator, name):
         super().__init__(parent, locator, name)
@@ -320,55 +336,53 @@
         if log:
             logger.info(
                 f"[{self.__full_name__}] getting element's rectangle(location + size): {rect}"
             )
         return rect
 
     @error_recovery(logger=logger)
-    def make_screenshot(self, filepath: Optional[str] = None):
+    def make_screenshot(self, filepath: Optional[str] = None) -> Image:
         """
         Takes a screenshot of the element.
 
         Parameters:
             filepath (Optional[str]): The file path where the screenshot should be saved. If not specified,
                                       the screenshot will be returned as a base64 encoded string.
 
         Returns:
             Union[str, None]: The base64 encoded string of the screenshot if no filepath is provided, otherwise None.
         """
-        if filepath:
-            return self.element_adapter.screenshot(
-                filepath
-            )  # Replace with the actual path
-        else:
-            return self.element_adapter.scrrenshot_as_base64
+        return Image(path=filepath, img_data=self.element_adapter.screenshot_as_base64)
 
     def screenshot(
         self,
         message: Optional[str] = "Element screen snap",
         title: Optional[str] = "Element screen snap",
     ):
         """
         Logs a screenshot of the element along with a custom message and title.
 
         Parameters:
             message (Optional[str]): The message to accompany the screenshot in the log.
             title (Optional[str]): The title for the screenshot attachment in the log.
         """
-        base_64_img_URL = f"data:text/html;{self.make_screenshot()}"
         logger.info(
             message,
             extra={
                 "attachments": [
-                    {"title": title, "type": "image", "url": base_64_img_URL}
+                    {
+                        "title": title,
+                        "type": "image",
+                        "url": self.make_screenshot().to_base64(),
+                    }
                 ]
             },
         )
 
-    def assert_text(self, expected_text) -> ExpectationResult:
+    def assert_text(self, expected_text) -> Type[ExpectationResult]:
         """
         Asserts that the element's text matches the expected text. This method simplifies the syntax
         by directly integrating the assertion with the element's text retrieval, reducing code verbosity
         and enhancing readability and supportability.
 
         Behind the scenes, this utilizes the Expect class to perform the comparison and logging,
         ensuring that an exception is raised if the assertion fails, providing immediate feedback
@@ -381,20 +395,20 @@
             ExpectationResult: An object representing the result of the comparison, which also behaves
                                 as a boolean indicating the success (True) or failure (False) of the assertion.
 
         Raises:
             FailedExpectationException: If the actual text of the element does not match the expected text.
         """
         actual_value = self.get_text(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's text."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's text.", logger
         )
         return expect.to_be(expected_text)
 
-    def assert_attribute(self, attr_name, expected_text) -> ExpectationResult:
+    def assert_attribute(self, attr_name, expected_text) -> Type[ExpectationResult]:
         """
         Asserts that a specific attribute of the element has the expected value. Similar to `assert_text`,
         this method leverages the framework's assertion API to minimize verbosity by combining attribute retrieval
         and assertion into a single operation.
 
         It uses the Expect class for performing the comparison, logging the result, and raising an exception
         if the assertion fails, thus halting the test execution for immediate issue identification.
@@ -406,20 +420,24 @@
         Returns:
             ExpectationResult: The outcome of the assertion, acting as a boolean value to indicate success or failure.
 
         Raises:
             FailedExpectationException: If the actual value of the specified attribute does not match the expected value.
         """
         actual_value = self.get_attribute(attr_name, log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, f"Asserting element's '{attr_name}' attribute"
+        expect = prepare_expect_object(
+            self,
+            actual_value,
+            True,
+            f"Asserting element's '{attr_name}' attribute",
+            logger,
         )
         return expect.to_be(expected_text)
 
-    def assert_style(self, attr_name, expected_text) -> ExpectationResult:
+    def assert_style(self, attr_name, expected_text) -> Type[ExpectationResult]:
         """
         Asserts that the element's style for a given property matches the expected value. This convenience method
         reduces code complexity by encapsulating both the retrieval of the style property and the assertion logic
         into one straightforward call.
 
         Utilizing the Expect class, this method ensures detailed logging and comparison, throwing an exception
         for a failed assertion to provide clear feedback during test execution.
@@ -431,20 +449,24 @@
         Returns:
             ExpectationResult: A boolean-like object indicating the assertion result, with detailed comparison logs.
 
         Raises:
             FailedExpectationException: If the element's style value does not meet the expected condition.
         """
         actual_value = self.get_style(attr_name, log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, f"Asserting element's '{attr_name}' style value."
+        expect = prepare_expect_object(
+            self,
+            actual_value,
+            True,
+            f"Asserting element's '{attr_name}' style value.",
+            logger,
         )
         return expect.to_be(expected_text)
 
-    def verify_text(self, expected_text) -> ExpectationResult:
+    def verify_text(self, expected_text) -> Type[ExpectationResult]:
         """
         Verifies that the element's text matches the expected text without stopping test execution on failure.
         This method provides a non-blocking approach to check element states, logging all outcomes for traceability.
 
         Utilizing the Expect class for comparison, it logs the result extensively, allowing the test to continue
         even if the verification fails, thus enhancing issue traceability while maintaining test flow.
 
@@ -452,20 +474,20 @@
             expected_text (str): The text that the element's text is expected to match.
 
         Returns:
             ExpectationResult: An object representing the verification result, behaving as a boolean to indicate
                                 success (True) or failure (False), with detailed logging for both outcomes.
         """
         actual_value = self.get_text(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's text."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's text.", logger
         )
         return verify.to_be(expected_text)
 
-    def verify_attribute(self, attr_name, expected_text) -> ExpectationResult:
+    def verify_attribute(self, attr_name, expected_text) -> Type[ExpectationResult]:
         """
         Verifies the value of a specific attribute of the element matches the expected value, logging the outcome
         without halting the test on failure. This method simplifies checking attribute values by combining retrieval
         and verification, providing clear logs for both success and failure cases.
 
         It leverages the Expect class for detailed comparison and logging, enhancing test traceability without
         interrupting the test flow for verifications.
@@ -475,20 +497,24 @@
             expected_text (str): The expected attribute value.
 
         Returns:
             ExpectationResult: A boolean-like object indicating the verification result, with comprehensive logs.
 
         """
         actual_value = self.get_attribute(attr_name, log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, f"Verifying element's '{attr_name}' attribute"
+        verify = prepare_expect_object(
+            self,
+            actual_value,
+            False,
+            f"Verifying element's '{attr_name}' attribute",
+            logger,
         )
         return verify.to_be(expected_text)
 
-    def verify_style(self, attr_name, expected_text) -> ExpectationResult:
+    def verify_style(self, attr_name, expected_text) -> Type[ExpectationResult]:
         """
         Verifies the element's style for a given property matches the expected value, providing extensive logging
         for both success and failure without stopping the test. This method reduces verbosity by encapsulating the
         style property retrieval and verification in one call, improving readability and maintainability.
 
         Uses the Expect class for comparison, ensuring that detailed outcome logs are produced, thereby facilitating
         better issue traceability while allowing test execution to continue regardless of the verification result.
@@ -499,20 +525,24 @@
 
         Returns:
             ExpectationResult: An object representing the verification outcome, acting as a boolean for success or
                                 failure, with detailed logging included.
 
         """
         actual_value = self.get_style(attr_name, log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, f"Verifying element's '{attr_name}' style value."
+        verify = prepare_expect_object(
+            self,
+            actual_value,
+            False,
+            f"Verifying element's '{attr_name}' style value.",
+            logger,
         )
         return verify.to_be(expected_text)
 
-    def assert_visible(self) -> ExpectationResult:
+    def assert_visible(self) -> Type[ExpectationResult]:
         """
         Asserts that the element is visible on the page. It utilizes a private method to check visibility
         without additional logging, integrating seamlessly with the framework's assertion API for clarity
         and succinctness in test scripts.
 
         This method leverages the Expect class for performing the assertion and logging, raising an exception
         if the assertion fails, to provide immediate feedback on test failure with detailed traceability.
@@ -521,70 +551,70 @@
             ExpectationResult: An object representing the assertion result, behaving as a boolean to indicate
                                 the success (True) or failure (False) of the assertion.
 
         Raises:
             AssertionError: If the element is not visible.
         """
         actual_value = self._get_is_displayed(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's visibility."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's visibility.", logger
         )
         return expect.to_be(True)
 
-    def verify_visible(self) -> ExpectationResult:
+    def verify_visible(self) -> Type[ExpectationResult]:
         """
         Verifies that the element is visible on the page without stopping test execution on failure.
         This method enhances script readability and test flow by providing a non-blocking verification
         with detailed outcome logging.
 
         Returns:
             ExpectationResult: An object representing the verification result, acting as a boolean to indicate
                                 success (True) or failure (False), with detailed logging for both outcomes.
         """
         actual_value = self._get_is_displayed(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's visibility."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's visibility.", logger
         )
         return verify.to_be(True)
 
-    def assert_hidden(self) -> ExpectationResult:
+    def assert_hidden(self) -> Type[ExpectationResult]:
         """
         Asserts that the element is hidden (not displayed) on the page. This method uses a private method
         to check the element's hidden state without additional logging, ensuring test script clarity and
         maintenance ease.
 
         Returns:
             ExpectationResult: An object indicating the assertion result, capable of acting as a boolean value.
                                 Detailed logging is provided for traceability.
 
         Raises:
             AssertionError: If the element is visible instead of hidden.
         """
         actual_value = self._get_is_displayed(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's hidden state."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's hidden state.", logger
         )
         return expect.to_be(False)
 
-    def verify_hidden(self) -> ExpectationResult:
+    def verify_hidden(self) -> Type[ExpectationResult]:
         """
         Verifies that the element is hidden (not displayed) on the page, providing a flexible verification
         method that logs outcomes without interrupting test execution on failure.
 
         Returns:
             ExpectationResult: A boolean-like object indicating the verification outcome, with extensive logging
                                 provided for both success and failure cases.
         """
         actual_value = self._get_is_displayed(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's hidden state."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's hidden state.", logger
         )
         return verify.to_be(False)
 
-    def assert_enabled(self) -> ExpectationResult:
+    def assert_enabled(self) -> Type[ExpectationResult]:
         """
         Asserts that the element is enabled and interactive. It utilizes a private method to check the
         enabled state without additional logging, streamlining integration with the framework's assertion API.
 
         This method leverages the Expect class for performing the assertion and logging, raising an exception
         if the assertion fails, to provide immediate feedback on test failure with detailed traceability.
 
@@ -592,68 +622,68 @@
             ExpectationResult: An object representing the assertion result, behaving as a boolean to indicate
                                 the success (True) or failure (False) of the assertion.
 
         Raises:
             AssertionError: If the element is not enabled.
         """
         actual_value = self._get_is_enabled(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's enabled state."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's enabled state.", logger
         )
         return expect.to_be(True)
 
-    def verify_enabled(self) -> ExpectationResult:
+    def verify_enabled(self) -> Type[ExpectationResult]:
         """
         Verifies that the element is enabled without stopping test execution on failure. This method provides
         a non-blocking approach to check the element's enabled state, enhancing test flow with detailed logging.
 
         Returns:
             ExpectationResult: An object representing the verification result, acting as a boolean to indicate
                                 success (True) or failure (False), with detailed logging for both outcomes.
         """
         actual_value = self._get_is_enabled(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's enabled state."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's enabled state.", logger
         )
         return verify.to_be(True)
 
-    def assert_disabled(self) -> ExpectationResult:
+    def assert_disabled(self) -> Type[ExpectationResult]:
         """
         Asserts that the element is disabled. This method uses a private method to check the element's disabled
         state without additional logging, ensuring clarity and ease of maintenance in test scripts.
 
         Returns:
             ExpectationResult: An object indicating the assertion result, capable of acting as a boolean value.
                                 Detailed logging is provided for traceability.
 
         Raises:
             AssertionError: If the element is enabled instead of disabled.
         """
         actual_value = self._get_is_enabled(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's disabled state."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's disabled state.", logger
         )
         return expect.to_be(False)
 
-    def verify_disabled(self) -> ExpectationResult:
+    def verify_disabled(self) -> Type[ExpectationResult]:
         """
         Verifies that the element is disabled, logging the outcome without interrupting test execution on failure.
         This method offers a flexible verification approach with comprehensive outcome logging for better traceability.
 
         Returns:
             ExpectationResult: A boolean-like object indicating the verification outcome, with extensive logging
                                 provided for both success and failure cases.
         """
         actual_value = self._get_is_enabled(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's disabled state."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's disabled state.", logger
         )
         return verify.to_be(False)
 
-    def assert_selected(self) -> ExpectationResult:
+    def assert_selected(self) -> Type[ExpectationResult]:
         """
         Asserts that the element is selected (e.g., for checkboxes or radio buttons). It uses a private method
         to check the selected state without additional logging, integrating seamlessly with the framework's
         assertion API for clear and concise test scripts.
 
         This method employs the Expect class to perform the assertion and logging, raising an exception if
         the assertion fails, to provide immediate feedback on test failure with detailed traceability.
@@ -662,64 +692,180 @@
             ExpectationResult: An object representing the assertion result, behaving as a boolean to indicate
                                 the success (True) or failure (False) of the assertion.
 
         Raises:
             AssertionError: If the element is not selected.
         """
         actual_value = self._get_is_selected(log=False)
-        expect = self._prepare_expect_object(
-            actual_value, True, "Asserting element's selected state."
+        expect = prepare_expect_object(
+            self, actual_value, True, "Asserting element's selected state.", logger
         )
         return expect.to_be(True)
 
-    def verify_selected(self) -> ExpectationResult:
+    def verify_selected(self) -> Type[ExpectationResult]:
         """
         Verifies that the element is selected without stopping test execution on failure. This method offers
         a non-blocking approach to verify the element's selected state, enhancing test flow with detailed logging.
 
         Returns:
             ExpectationResult: An object representing the verification result, acting as a boolean to indicate
                                 success (True) or failure (False), with detailed logging for both outcomes.
         """
         actual_value = self._get_is_selected(log=False)
-        verify = self._prepare_expect_object(
-            actual_value, False, "Verifying element's selected state."
+        verify = prepare_expect_object(
+            self, actual_value, False, "Verifying element's selected state.", logger
         )
         return verify.to_be(True)
 
-    def _prepare_expect_object(
-        self, actual_value: Any, is_assertion: bool, prefix: str
+    def verify_visual_match(
+        self,
+        expected_value: Union[Image, str],
+        mismatch_threshold: float = config.visual.default_mismatch_threshold,
+        compare_regions: Optional[list] = None,
+        exclude_regions: Optional[list] = None,
+        mode: VisualModeType = config.visual.mode,
+    ) -> ImageExpectationResult:
+        """
+        Verifies that the current visual state matches the expected visual reference within the defined mismatch threshold.
+        This method supports optional focusing on specific regions for comparison or exclusion, depending on the test's needs.
+
+        Args:
+            expected_value (Union[Image, str]): The expected image or a path to the image file against which the actual image is compared.
+            mismatch_threshold (float): The allowable percentage difference between the images to consider them as matching.
+            compare_regions (Optional[list]): A list of regions (dictionaries with 'x', 'y', 'width', and 'height' keys) to exclusively compare.
+            exclude_regions (Optional[list]): A list of regions to exclude from the comparison.
+            mode (VisualModeType): The mode of operation (collect or compare) which can override the default behavior.
+
+        Returns:
+            ImageExpectationResult: The result of the visual comparison, including a similarity score and potential difference image.
+        """
+        return verify_visual_match(
+            self,
+            expected_value,
+            mismatch_threshold,
+            compare_regions,
+            exclude_regions,
+            mode,
+            logger,
+        )
+
+    def assert_visual_match(
+        self,
+        expected_value: Union[Image, str],
+        mismatch_threshold: float = config.visual.default_mismatch_threshold,
+        compare_regions: Optional[list] = None,
+        exclude_regions: Optional[list] = None,
+        mode: VisualModeType = config.visual.mode,
+    ) -> ImageExpectationResult:
+        """
+        Asserts that the current visual state matches the expected visual reference within a defined mismatch threshold.
+        Allows focusing on or excluding specific regions for comparison, providing flexibility for varied testing needs.
+
+        Args:
+            expected_value (Union[Image, str]): The expected image or path to the image file for comparison.
+            mismatch_threshold (float): The permissible percentage difference between the images for a successful match.
+            compare_regions (Optional[list]): Specific regions to compare, defined as dictionaries with coordinates and dimensions.
+            exclude_regions (Optional[list]): Regions to be excluded from the comparison.
+            mode (VisualModeType): The mode setting which determines the behavior (collect or compare).
+
+        Returns:
+            ImageExpectationResult: The outcome of the visual assertion, including details on similarity and any differences.
+        """
+        return assert_visual_match(
+            self,
+            expected_value,
+            mismatch_threshold,
+            compare_regions,
+            exclude_regions,
+            mode,
+            logger,
+        )
+
+    def verify_visual_match_in_regions(
+        self,
+        expected_value: Union[Image, str],
+        compare_regions: Optional[list] = None,
+        mismatch_threshold: float = config.visual.default_partial_mismatch_threshold,
+        mode: VisualModeType = config.visual.mode,
+    ):
+
+        return verify_visual_match_in_regions(
+            self, expected_value, compare_regions, mismatch_threshold, mode, logger
+        )
+
+    def assert_visual_match_in_regions(
+        self,
+        expected_value: Union[Image, str],
+        compare_regions: Optional[list] = None,
+        mismatch_threshold: float = config.visual.default_partial_mismatch_threshold,
+        mode: VisualModeType = config.visual.mode,
     ):
         """
-        Prepares an Expect object configured for either assertion or verification against an element's properties.
-        This method centralizes the creation of Expect objects, setting them up with the necessary context for
-        performing comparisons, logging outcomes, and controlling test flow based on the operation type (assertion
-        or verification).
+        Verifies that designated regions within the visual state match the expected reference, considering an optional mismatch threshold.
+        This method is particularly useful for tests that target specific areas of the visual representation.
 
-        The method distinguishes between assertions and verifications by the is_assertion parameter. Assertions
-        will halt test execution on failure by raising an exception, while verifications log the outcome and
-        allow the test to continue, enhancing traceability and flexibility in test scripting.
+        Args:
+            expected_value (Union[Image, str]): The reference image or path to the image file for focused comparison.
+            compare_regions (list): The regions within the image to compare, each defined with 'x', 'y', 'width', and 'height'.
+            mismatch_threshold (float): The allowed variance percentage between the specified regions of the images.
+            mode (VisualModeType): The operational mode (collect or compare) affecting the method's behavior.
 
-        Parameters:
-            actual_value (str|bool): The actual value retrieved from the element, to be compared against an expected value.
-            is_assertion (bool): Indicates whether the Expect object is being prepared for an assertion (True)
-                                 or a verification (False). This controls whether failures result in raised exceptions
-                                 or logged outcomes without stopping the test.
-            prefix (str): A message prefix to prepend to log entries, providing context about the comparison being performed.
+        Returns:
+            ImageExpectationResult: Detailed results of the region-specific visual comparison.
+        """
+        return assert_visual_match_in_regions(
+            self, expected_value, compare_regions, mismatch_threshold, mode, logger
+        )
+
+    def verify_visual_exclusion_match(
+        self,
+        expected_value: Union[Image, str],
+        exclude_regions: Optional[list] = None,
+        mismatch_threshold: float = config.visual.default_mismatch_threshold,
+        mode: VisualModeType = config.visual.mode,
+    ) -> ImageExpectationResult:
+        """
+        Verifies the visual match excluding certain regions, ideal for ignoring known variabilities or non-relevant sections.
+        Offers a way to concentrate verification on stable, significant areas of the visual content.
+
+        Args:
+            expected_value (Union[Image, str]): The reference image or path for the exclusion-based comparison.
+            exclude_regions (Optional[list]): Regions to omit during the verification, specified with their coordinates and dimensions.
+            mismatch_threshold (float): Permitted percentage of difference in the non-excluded image areas.
+            mode (VisualModeType): The running mode (collect or compare), influencing the execution context.
 
         Returns:
-            Expect: An Expect object configured with the actual value, logging details, and operational mode (assert or verify),
-                    ready for performing comparisons and handling outcomes appropriately.
+            ImageExpectationResult: The outcome of the comparison, emphasizing the non-excluded areas.
         """
-        return Expect(
-            actual_value,
-            sender=self.__full_name__,
-            logger=logger,
-            is_assertion=is_assertion,
-            prefix=prefix,
+        return verify_visual_exclusion_match(
+            self, expected_value, exclude_regions, mismatch_threshold, mode, logger
+        )
+
+    def assert_visual_exclusion_match(
+        self,
+        expected_value: Union[Image, str],
+        exclude_regions: Optional[list] = None,
+        mismatch_threshold: float = config.visual.default_mismatch_threshold,
+        mode: VisualModeType = config.visual.mode,
+    ) -> ImageExpectationResult:
+        """
+        Asserts a visual match while disregarding specified regions, suitable for bypassing dynamic or irrelevant image parts.
+        Enhances test accuracy by focusing assertions on essential and predictable image segments.
+
+        Args:
+            expected_value (Union[Image, str]): The expected image or file path for focused exclusion assertion.
+            exclude_regions (Optional[list]): Areas to exclude, each defined by 'x', 'y', 'width', and 'height'.
+            mismatch_threshold (float): Acceptance threshold for variations outside the excluded regions.
+            mode (VisualModeType): Configuration setting to switch between collect and compare modes.
+
+        Returns:
+            ImageExpectationResult: Detailed assertion results, highlighting the examined image portions.
+        """
+        return assert_visual_exclusion_match(
+            self, expected_value, exclude_regions, mismatch_threshold, mode, logger
         )
 
     @wait()
     def wait_until_found(self):
         """
         Waits until the element is found on the page. This method continuously attempts to find the element until it is present or the specified timeout is reached.
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/elements.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/elements.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/eql/elements_query_language.ebnf` & `hyperiontf-0.3.5/src/hyperiontf/ui/eql/elements_query_language.ebnf`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/eql/executor.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/eql/executor.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/eql/lexer.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/eql/lexer.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/eql/parser.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/eql/parser.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/iframe.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/iframe.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/locatable.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/locatable.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/mobile_screen.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/mobile_screen.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/webpage.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/webpage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 import time
+from typing import Optional
 
 from .decorators.autolog_class_method_helper import (
     auto_decorate_class_methods_with_logging,
 )
 from hyperiontf.logging import getLogger
-from hyperiontf.typing import Platform, LoggerSource, PlatformType, OSType
+from hyperiontf.typing import (
+    Platform,
+    LoggerSource,
+    PlatformType,
+    OSType,
+    ViewportLabelType,
+)
 import platform
 from .page_object_base import BasePageObject
 from .content_manager import ContentManager
 from .window_manager import WindowManager
 from .viewport_manager import ViewportManager
 from .automation_adapter_manager import AutomationAdaptersManager
 from hyperiontf.configuration import config
@@ -22,14 +29,21 @@
         self.viewport_manager = ViewportManager(self, self.logger)
         auto_decorate_class_methods_with_logging(self, WebPage, self.logger)
 
     @property
     def viewport(self):
         return self.viewport_manager.current_viewport
 
+    @viewport.setter
+    def viewport(self, viewport: ViewportLabelType):
+        self.viewport_manager.set_viewport(viewport)
+
+    def change_viewport(self, width: int, height: Optional[int] = None) -> None:
+        self.viewport_manager.resize(width, height)
+
     @property
     def platform(self) -> PlatformType:
         return Platform.WEB
 
     @property
     def os(self) -> OSType | str:
         return platform.system()
```

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/webview.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/webview.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/src/hyperiontf/ui/widget.py` & `hyperiontf-0.3.5/src/hyperiontf/ui/widget.py`

 * *Files identical despite different names*

### Comparing `hyperiontf-0.2.5/PKG-INFO` & `hyperiontf-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: hyperiontf
-Version: 0.2.5
+Version: 0.3.5
 Summary: Hyperion Testing Framework
 License: Apache 2.0 License
 Author: Oleksiy Bondar
 Author-email: bondaroleksiyandriyovich@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Appium-Python-Client (>=3.2.0,<4.0.0)
 Requires-Dist: jsonschema (>=4.20.0,<5.0.0)
+Requires-Dist: opencv-contrib-python (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: playwright (>=1.41.2,<2.0.0)
 Requires-Dist: ply (>=3.11,<4.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: selenium (>=4.18.1,<5.0.0)
 Requires-Dist: webdriver_manager (>=4.0.1,<5.0.0)
 Description-Content-Type: text/markdown
```

