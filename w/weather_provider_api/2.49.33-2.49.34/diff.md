# Comparing `tmp/weather_provider_api-2.49.33.tar.gz` & `tmp/weather_provider_api-2.49.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weather_provider_api-2.49.33.tar", max compression
+gzip compressed data, was "weather_provider_api-2.49.34.tar", max compression
```

## Comparing `weather_provider_api-2.49.33.tar` & `weather_provider_api-2.49.34.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0    17098 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/LICENSE
-drwxr-xr-x   0        0        0        0 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/LICENSES/
--rw-r--r--   0        0        0    10438 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/LICENSES/Apache-2.0.txt
--rw-r--r--   0        0        0    12890 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/LICENSES/CC-BY-2.5.txt
--rw-r--r--   0        0        0    15199 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/LICENSES/MPL-2.0.txt
--rw-r--r--   0        0        0    11816 2024-03-05 15:30:10.013856 weather_provider_api-2.49.33/README.md
--rw-r--r--   0        0        0     3115 2024-03-05 15:30:33.929977 weather_provider_api-2.49.33/pyproject.toml
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/__init__.py
--rw-r--r--   0        0        0     2651 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/__main__.py
--rw-r--r--   0        0        0     1821 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/app_version.py
--rw-r--r--   0        0        0     1054 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/config/__init__.py
--rw-r--r--   0        0        0      913 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/config/config.toml
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/core/__init__.py
--rw-r--r--   0        0        0     3009 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/core/application.py
--rw-r--r--   0        0        0      478 2024-03-05 15:30:10.017856 weather_provider_api-2.49.33/weather_provider_api/core/base_model.py
--rw-r--r--   0        0        0      135 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/exceptions/__init__.py
--rw-r--r--   0        0        0      263 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/exceptions/additional_responses.py
--rw-r--r--   0        0        0      267 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/exceptions/api_models.py
--rw-r--r--   0        0        0      704 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/exceptions/exceptions.py
--rw-r--r--   0        0        0     2278 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/gunicorn_application.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/__init__.py
--rw-r--r--   0        0        0     2157 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/cors.py
--rw-r--r--   0        0        0     2006 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/exception_handling.py
--rw-r--r--   0        0        0     1310 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/headers.py
--rw-r--r--   0        0        0     5267 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/logging_handler.py
--rw-r--r--   0        0        0     1318 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/mounting.py
--rw-r--r--   0        0        0     1642 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/prometheus.py
--rw-r--r--   0        0        0      348 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/rate_limiter.py
--rw-r--r--   0        0        0     4375 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/initializers/validation.py
--rw-r--r--   0        0        0       46 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/utils/__init__.py
--rw-r--r--   0        0        0      696 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/core/utils/example_responses.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/__init__.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/__init__.py
--rw-r--r--   0        0        0     6446 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_models.py
--rw-r--r--   0        0        0     5806 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_view_v1.py
--rw-r--r--   0        0        0     9649 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_view_v2.py
--rw-r--r--   0        0        0       91 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/base_models/__init__.py
--rw-r--r--   0        0        0     5975 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/base_models/model.py
--rw-r--r--   0        0        0     1135 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/base_models/source.py
--rw-r--r--   0        0        0     6686 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/controller.py
--rw-r--r--   0        0        0      726 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/exceptions.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/repository/__init__.py
--rw-r--r--   0        0        0    14191 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/repository/repository.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/__init__.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/__init__.py
--rw-r--r--   0        0        0      681 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/cds.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/__init__.py
--rw-r--r--   0        0        0    13309 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/downloader.py
--rw-r--r--   0        0        0     6408 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
--rw-r--r--   0        0        0     6840 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
--rw-r--r--   0        0        0    15187 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
--rw-r--r--   0        0        0      591 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/factors.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/models/__init__.py
--rw-r--r--   0        0        0     8711 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/models/era5land.py
--rw-r--r--   0        0        0     7833 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/__init__.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
--rw-r--r--   0        0        0     6930 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
--rw-r--r--   0        0        0    23812 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
--rw-r--r--   0        0        0     9169 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
--rw-r--r--   0        0        0     1495 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/knmi.py
--rw-r--r--   0        0        0      421 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
--rw-r--r--   0        0        0     4963 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
--rw-r--r--   0        0        0     5320 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
--rw-r--r--   0        0        0    15117 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
--rw-r--r--   0        0        0     4781 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
--rw-r--r--   0        0        0    11062 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
--rw-r--r--   0        0        0    13328 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
--rw-r--r--   0        0        0    19917 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/stations.py
--rw-r--r--   0        0        0     7014 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/utils.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
--rw-r--r--   0        0        0     5148 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/__init__.py
--rw-r--r--   0        0        0     3048 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/date_helpers.py
--rw-r--r--   0        0        0     1397 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/file_helpers.py
--rw-r--r--   0        0        0     5742 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/geo_position.py
--rw-r--r--   0        0        0     1791 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/grid_helpers.py
--rw-r--r--   0        0        0      447 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/pandas_helpers.py
--rw-r--r--   0        0        0     5052 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/serializers.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/__init__.py
--rw-r--r--   0        0        0      393 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/erase_arome_repository.py
--rw-r--r--   0        0        0      413 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/erase_era5land_repository.py
--rw-r--r--   0        0        0      438 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/erase_era5sl_repository.py
--rw-r--r--   0        0        0      497 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/erase_waarnemingen_register.py
--rw-r--r--   0        0        0      383 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/update_arome_repository.py
--rw-r--r--   0        0        0      401 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/update_era5land_repository.py
--rw-r--r--   0        0        0      371 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/update_era5sl_repository.py
--rw-r--r--   0        0        0      462 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/scripts/update_waarnemingen_register.py
--rw-r--r--   0        0        0      140 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/versions/__init__.py
--rw-r--r--   0        0        0      796 2024-03-05 15:30:10.021856 weather_provider_api-2.49.33/weather_provider_api/versions/v1.py
--rw-r--r--   0        0        0      772 2024-03-05 15:30:10.025856 weather_provider_api-2.49.33/weather_provider_api/versions/v2.py
--rw-r--r--   0        0        0    13004 1970-01-01 00:00:00.000000 weather_provider_api-2.49.33/PKG-INFO
+-rw-r--r--   0        0        0    17098 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/LICENSE
+drwxr-xr-x   0        0        0        0 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/LICENSES/
+-rw-r--r--   0        0        0    10438 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/LICENSES/Apache-2.0.txt
+-rw-r--r--   0        0        0    12890 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/LICENSES/CC-BY-2.5.txt
+-rw-r--r--   0        0        0    15199 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/LICENSES/MPL-2.0.txt
+-rw-r--r--   0        0        0    11816 2024-04-03 06:53:07.932158 weather_provider_api-2.49.34/README.md
+-rw-r--r--   0        0        0     3110 2024-04-03 06:53:34.464088 weather_provider_api-2.49.34/pyproject.toml
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/__init__.py
+-rw-r--r--   0        0        0     2651 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/__main__.py
+-rw-r--r--   0        0        0     1821 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/app_version.py
+-rw-r--r--   0        0        0     1054 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/config/__init__.py
+-rw-r--r--   0        0        0      913 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/config/config.toml
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/__init__.py
+-rw-r--r--   0        0        0     2995 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/application.py
+-rw-r--r--   0        0        0      478 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/base_model.py
+-rw-r--r--   0        0        0      135 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/exceptions/__init__.py
+-rw-r--r--   0        0        0      263 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/exceptions/additional_responses.py
+-rw-r--r--   0        0        0      267 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/exceptions/api_models.py
+-rw-r--r--   0        0        0      704 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/exceptions/exceptions.py
+-rw-r--r--   0        0        0     2278 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/gunicorn_application.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/__init__.py
+-rw-r--r--   0        0        0     2157 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/cors.py
+-rw-r--r--   0        0        0     2006 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/exception_handling.py
+-rw-r--r--   0        0        0     1310 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/headers.py
+-rw-r--r--   0        0        0     5297 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/logging_handler.py
+-rw-r--r--   0        0        0     1318 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/mounting.py
+-rw-r--r--   0        0        0     1642 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/prometheus.py
+-rw-r--r--   0        0        0      348 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/rate_limiter.py
+-rw-r--r--   0        0        0     4375 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/initializers/validation.py
+-rw-r--r--   0        0        0       46 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/utils/__init__.py
+-rw-r--r--   0        0        0      696 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/core/utils/example_responses.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/__init__.py
+-rw-r--r--   0        0        0     6446 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_models.py
+-rw-r--r--   0        0        0     5806 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_view_v1.py
+-rw-r--r--   0        0        0     9649 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_view_v2.py
+-rw-r--r--   0        0        0       91 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/base_models/__init__.py
+-rw-r--r--   0        0        0     5975 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/base_models/model.py
+-rw-r--r--   0        0        0     1135 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/base_models/source.py
+-rw-r--r--   0        0        0     6686 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/controller.py
+-rw-r--r--   0        0        0      726 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/exceptions.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/repository/__init__.py
+-rw-r--r--   0        0        0    14191 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/repository/repository.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/__init__.py
+-rw-r--r--   0        0        0      681 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/cds.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/__init__.py
+-rw-r--r--   0        0        0    13309 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/downloader.py
+-rw-r--r--   0        0        0     6408 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py
+-rw-r--r--   0        0        0     6840 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py
+-rw-r--r--   0        0        0    15187 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py
+-rw-r--r--   0        0        0      591 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/factors.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/models/__init__.py
+-rw-r--r--   0        0        0     8711 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/models/era5land.py
+-rw-r--r--   0        0        0     7833 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/models/era5sl.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/__init__.py
+-rw-r--r--   0        0        0     6930 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py
+-rw-r--r--   0        0        0    23812 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py
+-rw-r--r--   0        0        0     9169 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py
+-rw-r--r--   0        0        0     1495 2024-04-03 06:53:07.936158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/knmi.py
+-rw-r--r--   0        0        0      421 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/knmi_factors.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/__init__.py
+-rw-r--r--   0        0        0     4963 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py
+-rw-r--r--   0        0        0     5320 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py
+-rw-r--r--   0        0        0    15117 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py
+-rw-r--r--   0        0        0     4781 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py
+-rw-r--r--   0        0        0    11062 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/pluim.py
+-rw-r--r--   0        0        0    13328 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py
+-rw-r--r--   0        0        0    19917 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/stations.py
+-rw-r--r--   0        0        0     7014 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/utils.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/weather_alert/__init__.py
+-rw-r--r--   0        0        0     5148 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/__init__.py
+-rw-r--r--   0        0        0     3048 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/date_helpers.py
+-rw-r--r--   0        0        0     1397 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/file_helpers.py
+-rw-r--r--   0        0        0     5742 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/geo_position.py
+-rw-r--r--   0        0        0     1791 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/grid_helpers.py
+-rw-r--r--   0        0        0      447 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/pandas_helpers.py
+-rw-r--r--   0        0        0     5052 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/serializers.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/__init__.py
+-rw-r--r--   0        0        0      393 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/erase_arome_repository.py
+-rw-r--r--   0        0        0      413 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/erase_era5land_repository.py
+-rw-r--r--   0        0        0      438 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/erase_era5sl_repository.py
+-rw-r--r--   0        0        0      497 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/erase_waarnemingen_register.py
+-rw-r--r--   0        0        0      383 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/update_arome_repository.py
+-rw-r--r--   0        0        0      401 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/update_era5land_repository.py
+-rw-r--r--   0        0        0      371 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/update_era5sl_repository.py
+-rw-r--r--   0        0        0      462 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/scripts/update_waarnemingen_register.py
+-rw-r--r--   0        0        0      140 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/versions/__init__.py
+-rw-r--r--   0        0        0      796 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/versions/v1.py
+-rw-r--r--   0        0        0      772 2024-04-03 06:53:07.940158 weather_provider_api-2.49.34/weather_provider_api/versions/v2.py
+-rw-r--r--   0        0        0    13001 1970-01-01 00:00:00.000000 weather_provider_api-2.49.34/PKG-INFO
```

### Comparing `weather_provider_api-2.49.33/LICENSE` & `weather_provider_api-2.49.34/LICENSE`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/LICENSES/Apache-2.0.txt` & `weather_provider_api-2.49.34/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/LICENSES/CC-BY-2.5.txt` & `weather_provider_api-2.49.34/LICENSES/CC-BY-2.5.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/LICENSES/MPL-2.0.txt` & `weather_provider_api-2.49.34/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/README.md` & `weather_provider_api-2.49.34/README.md`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/pyproject.toml` & `weather_provider_api-2.49.34/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 [tool.poetry]
 name = "weather_provider_api"
-version = "2.49.033"
+version = "2.49.034"
 description = "Weather Provider Libraries and API"
 authors = ["Verbindingsteam", "Raoul Linnenbank <58594297+rflinnenbank@users.noreply.github.com>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository="https://github.com/alliander-opensource/wpla/"
 include = [
     {path = "var_maps/*.json", format = "wheel"}
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-fastapi = "^0.104.1"
+fastapi = "^0.110.1"
 requests = "^2.31.0"
 geopy = "^2.3.0"
 numpy = "^1.26.2"
 gunicorn = "^21.2.0"
-lxml = "^4.9.1"
+lxml = "^5.2.1"
 starlette-prometheus = "^0.9.0"
 beautifulsoup4 = "^4.12.2"
 netcdf4 = "^1.6.5"
 tomli = "^2.0.1"
 pandas = "^2.1.3"
-xarray = "^2023.11"
+xarray = "^2024.3.0"
 cfgrib = "^0.9.10.4"
-uvicorn = "^0.24.0.post1"
+uvicorn = "^0.29.0"
 slowapi = "^0.1.7"
 loguru = "^0.7.2"
 email-validator = "^2.1.0.post1"
 eccodes = "^1.6.1"
-ecmwflibs = "0.5.1"
+ecmwflibs = "0.6.3"
 accept-types = "^0.4.1"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 coverage = "^6.5.0"
```

### Comparing `weather_provider_api-2.49.33/weather_provider_api/__main__.py` & `weather_provider_api-2.49.34/weather_provider_api/__main__.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/app_version.py` & `weather_provider_api-2.49.34/weather_provider_api/app_version.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/config/__init__.py` & `weather_provider_api-2.49.34/weather_provider_api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/config/config.toml` & `weather_provider_api-2.49.34/weather_provider_api/config/config.toml`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/application.py` & `weather_provider_api-2.49.34/weather_provider_api/core/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,25 @@
 
 #  SPDX-FileCopyrightText: 2019-2023 Alliander N.V.
 #  SPDX-License-Identifier: MPL-2.0
 
 """ Main Application """
 
 from fastapi import FastAPI
-from fastapi.openapi.utils import get_openapi
 from starlette.responses import RedirectResponse
 
 from weather_provider_api.app_version import APP_VERSION
 from weather_provider_api.config import APP_CONFIG
 from weather_provider_api.core.initializers.cors import initialize_cors_middleware
 from weather_provider_api.core.initializers.exception_handling import initialize_exception_handler
 from weather_provider_api.core.initializers.headers import initialize_header_metadata
 from weather_provider_api.core.initializers.logging_handler import initialize_logging
 from weather_provider_api.core.initializers.mounting import mount_api_version
 from weather_provider_api.core.initializers.prometheus import initialize_prometheus_interface
 from weather_provider_api.core.initializers.validation import initialize_api_validation
-
 from weather_provider_api.versions.v1 import app as v1
 from weather_provider_api.versions.v2 import app as v2
 
 
 def _build_api_application() -> FastAPI:
     """The main method for building a standardized FastAPI application for use with for instance Uvicorn.
 
@@ -37,14 +35,15 @@
     app_title = APP_CONFIG["base"]["title"]
     app_description = APP_CONFIG["base"]["description"]
 
     # Setting up the base application
     application = FastAPI(
         version=APP_VERSION,
         title=app_title,
+        summary=app_description,
         description=app_description,
         contact={"name": APP_CONFIG["maintainer"]["name"], "email": APP_CONFIG["maintainer"]["email_address"]},
     )
     application.openapi_version = "3.0.2"
 
     # Attach logging
     application.add_event_handler("startup", initialize_logging)
```

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/exceptions/exceptions.py` & `weather_provider_api-2.49.34/weather_provider_api/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/gunicorn_application.py` & `weather_provider_api-2.49.34/weather_provider_api/core/gunicorn_application.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/cors.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/cors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/exception_handling.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/exception_handling.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/headers.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/headers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/logging_handler.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/logging_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         30: "WARNING",
         20: "INFO",
         10: "DEBUG",
         0: "NOTSET",
     }
 
     def emit(self, record: logging.LogRecord) -> None:
-        """Emission method that intercepts the original logging message using Python's base logging system and
+        """Emission method that intercepts the original logging message using Python's base logging system and  # noqa: D205
          re-formats it (if needed) to match Loguru systems.
 
         Args:
             record: The original logging LogRecord object that holds a record to be converted.
 
         Returns:
             Nothing. We bind the converted message directly to de Loguru logger for processing.
@@ -62,16 +62,17 @@
 
         # Log the message as intended by writing the converted data to the proper log area.
         log = logger.bind(request_id="app")
         log.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def initialize_logging():
-    """The method that initializes and sets our custom logging system as the default, and reroutes other logging
+    """The method that initializes and sets our custom logging system as the default, and reroutes other logging  # noqa: D205
      systems to use our system instead.
+
     Returns:
         Nothing. The logging system itself is overwritten.
     """
     logger.remove()  # Remove any existing default loggers from Loguru
 
     # Log formats:
     #  - [Elastic]: Holds the official format set as the Chapter standard by Data & Analytics.
```

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/mounting.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/mounting.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/prometheus.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/prometheus.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/initializers/validation.py` & `weather_provider_api-2.49.34/weather_provider_api/core/initializers/validation.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/core/utils/example_responses.py` & `weather_provider_api-2.49.34/weather_provider_api/core/utils/example_responses.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_models.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_models.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_view_v1.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_view_v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/api_view_v2.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/api_view_v2.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/base_models/model.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/base_models/model.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/base_models/source.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/base_models/source.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/controller.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/controller.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/exceptions.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/exceptions.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/repository/repository.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/repository/repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/cds.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/cds.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/downloader.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/era5land_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/era5sl_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/client/utils_era5.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/factors.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/factors.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/models/era5land.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/models/era5land.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/cds/models/era5sl.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/cds/models/era5sl.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/actuele_waarnemingen_register_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/arome_repository.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/client/knmi_downloader.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/knmi.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/knmi.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/actuele_waarnemingen_register.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/daggegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/harmonie_arome.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/pluim.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/pluim.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/models/uurgegevens.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/stations.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/stations.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/knmi/utils.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/knmi/utils.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/sources/weather_alert/weather_alert.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/date_helpers.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/date_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/file_helpers.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/geo_position.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/geo_position.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/grid_helpers.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/routers/weather/utils/serializers.py` & `weather_provider_api-2.49.34/weather_provider_api/routers/weather/utils/serializers.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/versions/v1.py` & `weather_provider_api-2.49.34/weather_provider_api/versions/v1.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/weather_provider_api/versions/v2.py` & `weather_provider_api-2.49.34/weather_provider_api/versions/v2.py`

 * *Files identical despite different names*

### Comparing `weather_provider_api-2.49.33/PKG-INFO` & `weather_provider_api-2.49.34/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: weather_provider_api
-Version: 2.49.33
+Version: 2.49.34
 Summary: Weather Provider Libraries and API
 Home-page: https://github.com/alliander-opensource/wpla/
 License: MPL-2.0
 Author: Verbindingsteam
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: accept-types (>=0.4.1,<0.5.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: cfgrib (>=0.9.10.4,<0.10.0.0)
 Requires-Dist: eccodes (>=1.6.1,<2.0.0)
-Requires-Dist: ecmwflibs (==0.5.1)
+Requires-Dist: ecmwflibs (==0.6.3)
 Requires-Dist: email-validator (>=2.1.0.post1,<3.0.0)
-Requires-Dist: fastapi (>=0.104.1,<0.105.0)
+Requires-Dist: fastapi (>=0.110.1,<0.111.0)
 Requires-Dist: geopy (>=2.3.0,<3.0.0)
 Requires-Dist: gunicorn (>=21.2.0,<22.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: lxml (>=5.2.1,<6.0.0)
 Requires-Dist: netcdf4 (>=1.6.5,<2.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: pandas (>=2.1.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: slowapi (>=0.1.7,<0.2.0)
 Requires-Dist: starlette-prometheus (>=0.9.0,<0.10.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: uvicorn (>=0.24.0.post1,<0.25.0)
-Requires-Dist: xarray (>=2023.11,<2024.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
+Requires-Dist: xarray (>=2024.3.0,<2025.0.0)
 Project-URL: Repository, https://github.com/alliander-opensource/wpla/
 Description-Content-Type: text/markdown
 
 <!--
 SPDX-FileCopyrightText: 2019-2022 Alliander N.V.
 SPDX-License-Identifier: MPL-2.0
 -->
```

