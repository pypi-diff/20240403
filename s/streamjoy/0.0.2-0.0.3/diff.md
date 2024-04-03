# Comparing `tmp/streamjoy-0.0.2.tar.gz` & `tmp/streamjoy-0.0.3.tar.gz`

## Comparing `streamjoy-0.0.2.tar` & `streamjoy-0.0.3.tar`

### file list

```diff
@@ -1,75 +1,78 @@
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.2/.editorconfig
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.2/HOWTOCONTRIBUTE.md
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.2/HOWTORELEASE.md
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 streamjoy-0.0.2/mkdocs.yml
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 streamjoy-0.0.2/.github/workflows/build.yml
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.2/.github/workflows/documentation.yml
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.2/.github/workflows/release.yml
--rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/best_practices.md
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/index.md
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/package_design.md
--rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/supported_formats.md
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/core.md
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/models.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/renderers.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/settings.md
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/streams.md
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/api_reference/wrappers.md
--rw-r--r--   0        0        0    32485 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/assets/design.svg
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/air_temperature.md
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/co2_timeseries.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/gender_gapminder.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/nice_orbit.md
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/oisst_globe.md
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/sea_ice.md
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/sine_wave.md
--rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/stream_code.md
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/example_recipes/temperature_anomaly.md
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.2/docs/stylesheets/extra.css
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/.gitignore
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/__init__.py
--rw-r--r--   0        0        0     8760 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/_utils.py
--rw-r--r--   0        0        0     2760 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/core.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/models.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/pandas.py
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/renderers.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/settings.py
--rw-r--r--   0        0        0    50758 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/streams.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/wrappers.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.2/streamjoy/xarray.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_core.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_models.py
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_pandas.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_renderers.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_settings.py
--rw-r--r--   0        0        0     2615 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_streams.py
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_wrappers.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/test_xarray.py
--rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png
--rw-r--r--   0        0        0    67272 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png
--rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.nc
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/gapminder.csv
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/gapminder.parquet
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/.zattrs
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/.zgroup
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/.zmetadata
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/air/.zarray
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/air/.zattrs
--rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/air/0.0.0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lat/.zarray
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lat/.zattrs
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lat/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lon/.zarray
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lon/.zattrs
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/lon/0
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/time/.zarray
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/time/.zattrs
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.2/tests/data/air.zarr/time/0
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 streamjoy-0.0.2/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.2/LICENSE
--rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 streamjoy-0.0.2/README.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 streamjoy-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     7034 2020-02-02 00:00:00.000000 streamjoy-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.editorconfig
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 streamjoy-0.0.3/HOWTOCONTRIBUTE.md
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 streamjoy-0.0.3/HOWTORELEASE.md
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 streamjoy-0.0.3/mkdocs.yml
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     5502 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/best_practices.md
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/index.md
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/package_design.md
+-rw-r--r--   0        0        0     2688 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/supported_formats.md
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/core.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/models.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/renderers.md
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/settings.md
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/streams.md
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/api_reference/wrappers.md
+-rw-r--r--   0        0        0    32485 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/assets/design.svg
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/air_temperature.md
+-rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/co2_timeseries.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/gender_gapminder.md
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/nice_orbit.md
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/oisst_globe.md
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/sea_ice.md
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/sine_wave.md
+-rw-r--r--   0        0        0     3579 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/stream_code.md
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/example_recipes/temperature_anomaly.md
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 streamjoy-0.0.3/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/.gitignore
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/__init__.py
+-rw-r--r--   0        0        0    10055 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/_utils.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/core.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/models.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/pandas.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/polars.py
+-rw-r--r--   0        0        0     3736 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/renderers.py
+-rw-r--r--   0        0        0    20373 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/serializers.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/settings.py
+-rw-r--r--   0        0        0    36573 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/streams.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/wrappers.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 streamjoy-0.0.3/streamjoy/xarray.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1328 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_core.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_models.py
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_pandas.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_renderers.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_settings.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_streams.py
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_wrappers.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/test_xarray.py
+-rw-r--r--   0        0        0    77959 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png
+-rw-r--r--   0        0        0    67272 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png
+-rw-r--r--   0        0        0    71503 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.nc
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/gapminder.csv
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/gapminder.parquet
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/.zattrs
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/.zgroup
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/.zmetadata
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/air/.zarray
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/air/.zattrs
+-rw-r--r--   0        0        0    43023 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/air/0.0.0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lat/.zarray
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lat/.zattrs
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lat/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lon/.zarray
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lon/.zattrs
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/lon/0
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/time/.zarray
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/time/.zattrs
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 streamjoy-0.0.3/tests/data/air.zarr/time/0
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 streamjoy-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 streamjoy-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6471 2020-02-02 00:00:00.000000 streamjoy-0.0.3/README.md
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 streamjoy-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7077 2020-02-02 00:00:00.000000 streamjoy-0.0.3/PKG-INFO
```

### Comparing `streamjoy-0.0.2/CONTRIBUTING.md` & `streamjoy-0.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/HOWTOCONTRIBUTE.md` & `streamjoy-0.0.3/HOWTOCONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/mkdocs.yml` & `streamjoy-0.0.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/.github/workflows/build.yml` & `streamjoy-0.0.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/.github/workflows/documentation.yml` & `streamjoy-0.0.3/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/.github/workflows/release.yml` & `streamjoy-0.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/best_practices.md` & `streamjoy-0.0.3/docs/best_practices.md`

 * *Files 5% similar despite different names*

```diff
@@ -175,8 +175,26 @@
 
 Matplotlib is not always thread-safe, so if you're seeing flickering, set `threads_per_worker=1`.
 
 ```python
 from streamjoy import stream
 
 stream(..., threads_per_worker=1)
-```
+```
+
+## 🖥️ Specify `client` if using a remote cluster
+
+If you're using a remote cluster, specify the `client` argument to use the Dask client.
+
+```python
+from dask.distributed import Client
+
+client = Client()
+stream(..., client=client)
+```
+
+## 🪣 Use `fsspec` to read/write intermediate files on a remote filesystem
+
+```python
+fs = fsspec.filesystem('s3', anon=False)
+stream(..., fsspec_fs=fs, scratch_dir="bucket-name/streamjoy_scratch")
+```
```

### Comparing `streamjoy-0.0.2/docs/package_design.md` & `streamjoy-0.0.3/docs/package_design.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/supported_formats.md` & `streamjoy-0.0.3/docs/supported_formats.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,27 @@
 stream(df, uri="gapminder.mp4", groupby="Country", title="{Year}")
 ```
 
 <video controls="true" allowfullscreen="true">
 <source src="https://github.com/ahuang11/streamjoy/assets/15331990/be0fc06c-c821-4c45-91a3-8c898e730851" type="video/mp4">
 </video>
 
+## 🐻‍❄️ Polars DataFrame
+```python
+from streamjoy import stream
+import polars as pl
+
+df = pl.read_csv(
+    "https://raw.githubusercontent.com/franlopezguzman/gapminder-with-bokeh/master/gapminder_tidy.csv"
+)
+df = df.query("Country in ['United States', 'China', 'South Africa']")
+stream(df, uri="gapminder.mp4", groupby="Country", title="{Year}")
+```
+
+
 ## 🗄️ XArray Dataset or DataArray
 
 ```python
 from streamjoy import stream
 import xarray as xr
 
 ds = xr.tutorial.open_dataset("air_temperature").isel(time=slice(0, 100))
```

### Comparing `streamjoy-0.0.2/docs/api_reference/settings.md` & `streamjoy-0.0.3/docs/api_reference/settings.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/assets/design.svg` & `streamjoy-0.0.3/docs/assets/design.svg`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/air_temperature.md` & `streamjoy-0.0.3/docs/example_recipes/air_temperature.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/co2_timeseries.md` & `streamjoy-0.0.3/docs/example_recipes/co2_timeseries.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/gender_gapminder.md` & `streamjoy-0.0.3/docs/example_recipes/gender_gapminder.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/nice_orbit.md` & `streamjoy-0.0.3/docs/example_recipes/nice_orbit.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/oisst_globe.md` & `streamjoy-0.0.3/docs/example_recipes/oisst_globe.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/sea_ice.md` & `streamjoy-0.0.3/docs/example_recipes/sea_ice.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/sine_wave.md` & `streamjoy-0.0.3/docs/example_recipes/sine_wave.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/stream_code.md` & `streamjoy-0.0.3/docs/example_recipes/stream_code.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/docs/example_recipes/temperature_anomaly.md` & `streamjoy-0.0.3/docs/example_recipes/temperature_anomaly.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/streamjoy/__init__.py` & `streamjoy-0.0.3/streamjoy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     default_pandas_renderer,
     default_xarray_renderer,
 )
 from .settings import config, file_handlers, obj_handlers
 from .streams import GifStream, Mp4Stream
 from .wrappers import wrap_holoviews, wrap_matplotlib
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 __all__ = [
     "GifStream",
     "ImageText",
     "Mp4Stream",
     "Paused",
     "config",
```

### Comparing `streamjoy-0.0.2/streamjoy/_utils.py` & `streamjoy-0.0.3/streamjoy/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import inspect
 import logging
+import os
 from collections.abc import Iterable
 from io import BytesIO
 from itertools import islice
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable
 
 import imageio.v3 as iio
@@ -130,15 +131,15 @@
         import requests
     except ImportError:
         raise ImportError("To directly read from a URL, `pip install requests`")
 
     url_path = Path(url)
     file_name = f"{url_path.parent.parent.name}_{url_path.parent.name}_{url_path.name}"
     uri = resolve_uri(file_name=file_name, scratch_dir=scratch_dir, in_memory=in_memory)
-    if isinstance(uri, Path) and uri.exists():
+    if not isinstance(uri, BytesIO) and os.path.exists(uri):
         return uri
 
     response = requests.get(url, stream=True)
     response.raise_for_status()
     with open(uri, "wb") as f:
         for chunk in response.iter_content(chunk_size=8192):
             if chunk:
@@ -191,21 +192,30 @@
     return True
 
 
 def resolve_uri(
     file_name: str | None = None,
     scratch_dir: str | Path | None = None,
     in_memory: bool = False,
-) -> Path | BytesIO:
+    fsspec_fs: Any | None = None,
+) -> str | Path | BytesIO:
     if in_memory:
         return BytesIO()
 
-    output_dir = Path(get_config_default("scratch_dir", scratch_dir, warn=False))
-    output_dir.mkdir(exist_ok=True, parents=True)
-    uri = output_dir / file_name
+    output_dir = get_config_default("scratch_dir", scratch_dir, warn=False)
+    if fsspec_fs:
+        try:
+            fsspec_fs.mkdir(output_dir, exist_ok=True, parents=True)
+        except FileExistsError:
+            pass
+        uri = os.path.join(output_dir, file_name)
+    else:
+        output_dir = Path(output_dir)
+        output_dir.mkdir(exist_ok=True, parents=True)
+        uri = output_dir / file_name
     return uri
 
 
 def pop_kwargs(callable: Callable, kwargs: dict) -> None:
     args_spec = inspect.getfullargspec(callable)
     return {arg: kwargs.pop(arg) for arg in args_spec.args if arg in kwargs}
 
@@ -288,13 +298,45 @@
     repeat = int(seconds * fps)
     for _ in range(repeat):
         write(image, **write_kwargs)
     return image
 
 
 def imread_with_pause(
-    uri: Any | Paused, extension: str | None = None, plugin: str | None = None
+    uri: Any | Paused,
+    extension: str | None = None,
+    plugin: str | None = None,
+    fsspec_fs: Any | None = None,
 ) -> np.ndarray | Paused:
     imread_kwargs = dict(extension=extension, plugin=plugin)
+    seconds = None
     if isinstance(uri, Paused):
-        return Paused(iio.imread(uri.output, **imread_kwargs).squeeze(), uri.seconds)
-    return iio.imread(uri, **imread_kwargs).squeeze()
+        seconds = uri.seconds
+        uri = uri.output
+    if fsspec_fs:
+        with fsspec_fs.open(uri, "rb") as f:
+            image = iio.imread(f, **imread_kwargs)
+    else:
+        image = iio.imread(uri, **imread_kwargs).squeeze()
+    image = image.squeeze()
+    if seconds is None:
+        return image
+    else:
+        return Paused(output=image, seconds=seconds)
+
+
+def subset_resources_renderer_iterables(
+    resources: Any, renderer_iterables: list[Any], max_frames: int
+):
+    if len(resources) > max_frames and max_frames != -1:
+        color = config["logging_warning_color"]
+        reset = config["logging_reset_color"]
+        logging.warning(
+            f"There are a total of {len(resources)} frames, "
+            f"but streaming only {color}{max_frames}{reset}. "
+            f"Set max_frames to -1 to stream all frames."
+        )
+    resources = resources[: max_frames or max_frames]
+    renderer_iterables = [
+        iterable[: len(resources)] for iterable in renderer_iterables or []
+    ]
+    return resources, renderer_iterables
```

### Comparing `streamjoy-0.0.2/streamjoy/core.py` & `streamjoy-0.0.3/streamjoy/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from io import BytesIO
 from pathlib import Path
 from typing import Any, Callable, Literal
 
+from .serializers import serialize_appropriately
 from .streams import AnyStream, ConnectedStreams, GifStream, Mp4Stream
 
 
 def stream(
     resources: Any,
     uri: str | Path | BytesIO | None = None,
     renderer: Callable | None = None,
@@ -41,28 +42,25 @@
     if extension == ".mp4":
         stream_cls = Mp4Stream
     elif extension == ".gif":
         stream_cls = GifStream
     else:
         stream_cls = AnyStream
 
-    resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-        stream_cls._expand_from_any(
-            resources, renderer, renderer_iterables, renderer_kwargs or {}, **kwargs
-        )
-    )
-
-    stream = stream_cls(
-        resources=resources,
-        renderer=renderer,
-        renderer_iterables=renderer_iterables,
-        renderer_kwargs=renderer_kwargs,
+    serialized = serialize_appropriately(
+        stream_cls,
+        resources,
+        renderer,
+        renderer_iterables,
+        renderer_kwargs or {},
         **kwargs,
     )
 
+    stream = stream_cls(**serialized.param.values(), **serialized.kwargs)
+
     if uri:
         return stream.write(uri=uri, extension=extension)
     return stream
 
 
 def connect(
     streams: list[AnyStream | GifStream | Mp4Stream],
```

### Comparing `streamjoy-0.0.2/streamjoy/models.py` & `streamjoy-0.0.3/streamjoy/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -88,7 +88,32 @@
             (x, y),
             self.text,
             font=font,
             fill=self.color,
             anchor=self.anchor,
             **self.kwargs,
         )
+
+
+class Serialized(param.Parameterized):
+    resources = param.List(doc="The list of resources.")
+    renderer = param.Callable(doc="The rendering function to use on the resources.")
+    renderer_iterables = param.List(
+        doc="Additional iterable arguments to pass to the renderer.",
+        allow_None=True,
+    )
+    renderer_kwargs = param.Dict(
+        doc="Additional keyword arguments to pass to the renderer.",
+        allow_None=True,
+    )
+
+    def __init__(
+        self, resources, renderer, renderer_iterables, renderer_kwargs, kwargs, **params
+    ):
+        super().__init__(
+            resources=resources,
+            renderer=renderer,
+            renderer_iterables=renderer_iterables,
+            renderer_kwargs=renderer_kwargs,
+            **params,
+        )
+        self.kwargs = kwargs
```

### Comparing `streamjoy-0.0.2/streamjoy/renderers.py` & `streamjoy-0.0.3/streamjoy/renderers.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 
     try:
         import pandas as pd
     except ImportError:
         pd = None
 
     try:
+        import polars as pl
+    except ImportError:
+        pl = None
+
+    try:
         import xarray as xr
     except ImportError:
         xr = None
 
     try:
         import holoviews as hv
     except ImportError:
@@ -58,14 +63,35 @@
             df_group.plot(*args, ax=ax, label=group, **kwargs)
     else:
         df_sub.plot(*args, ax=ax, **kwargs)
 
     return fig
 
 
+def default_polars_renderer(
+    df_sub: pl.DataFrame, *args: tuple[Any], **kwargs: dict[str, Any]
+) -> hv.Element:
+    """
+    Render a polars DataFrame using HoloViews.
+
+    Args:
+        df_sub: The DataFrame to render.
+        *args: Additional positional arguments to pass to the renderer.
+        **kwargs: Additional keyword arguments to pass to the renderer.
+
+    Returns:
+        The rendered HoloViews Element.
+    """
+    by = kwargs.pop("groupby", None)
+    if by:
+        kwargs["by"] = by
+    hv_obj = df_sub.plot(*args, **kwargs)
+    return default_holoviews_renderer(hv_obj)
+
+
 def default_xarray_renderer(
     da_sel: xr.DataArray, *args: tuple[Any], **kwargs: dict[str, Any]
 ) -> plt.Figure:
     """
     Render an xarray DataArray using matplotlib.
 
     Args:
```

### Comparing `streamjoy-0.0.2/streamjoy/settings.py` & `streamjoy-0.0.3/streamjoy/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,19 +38,21 @@
     "logging_datefmt": "%I:%M%p",
     "logging_warning_color": "\x1b[31;1m",
     "logging_success_color": "\x1b[32;1m",
     "logging_reset_color": "\x1b[0m",
 }
 
 obj_handlers = {
-    "xarray.Dataset": "_expand_from_xarray",
-    "xarray.DataArray": "_expand_from_xarray",
-    "pandas.DataFrame": "_expand_from_pandas",
-    "pandas.Series": "_expand_from_pandas",
-    "holoviews": "_expand_from_holoviews",
+    "xarray.Dataset": "serialize_xarray",
+    "xarray.DataArray": "serialize_xarray",
+    "pandas.DataFrame": "serialize_pandas",
+    "pandas.Series": "serialize_pandas",
+    "holoviews": "serialize_holoviews",
+    "polars.DataFrame": "serialize_polars",
+    "polars.Series": "serialize_polars",
 }
 
 file_handlers = {
     ".nc": {
         "import_path": "xarray.open_mfdataset",
     },
     ".nc4": {
```

### Comparing `streamjoy-0.0.2/streamjoy/streams.py` & `streamjoy-0.0.3/streamjoy/streams.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import base64
 import gc
 from abc import abstractmethod
 from collections.abc import Iterable, Sequence
 from functools import partial
-from inspect import isgenerator
 from io import BytesIO
 from itertools import zip_longest
 from pathlib import Path
 from textwrap import indent
 from typing import TYPE_CHECKING, Any, Callable
 
 import dask.delayed
@@ -18,29 +17,37 @@
 import param
 from dask.distributed import Client, Future, fire_and_forget
 from imageio.core.v3_plugin_api import PluginV3
 from PIL import Image, ImageDraw
 
 from . import _utils
 from .models import ImageText, Paused
-from .renderers import (
-    default_holoviews_renderer,
-    default_pandas_renderer,
-    default_xarray_renderer,
+from .serializers import (
+    serialize_appropriately,
+    serialize_holoviews,
+    serialize_pandas,
+    serialize_paths,
+    serialize_polars,
+    serialize_url,
+    serialize_xarray,
 )
-from .settings import config, file_handlers, obj_handlers
-from .wrappers import wrap_holoviews, wrap_matplotlib
+from .settings import config
 
 if TYPE_CHECKING:
     try:
         import pandas as pd
     except ImportError:
         pd = None
 
     try:
+        import polars as pl
+    except ImportError:
+        pl = None
+
+    try:
         import xarray as xr
     except ImportError:
         xr = None
 
     try:
         import holoviews as hv
     except ImportError:
@@ -159,14 +166,18 @@
         doc="The directory to use for temporary files.", check_exists=False
     )
 
     in_memory = param.Boolean(
         doc="Whether to store intermediate results in memory.",
     )
 
+    fsspec_fs = param.Parameter(
+        doc="The fsspec filesystem to use for reading and writing.",
+    )
+
     display = param.Boolean(
         doc="Whether to display the output in the notebook after rendering.",
     )
 
     _tbd_kwargs = param.Dict(doc="Params that are currently unknown.")
 
     _extension = ""
@@ -182,469 +193,96 @@
         for param_key in set(params):
             if param_key not in self.param:
                 params["_tbd_kwargs"][param_key] = params.pop(param_key)
 
         super().__init__(**params)
 
     @classmethod
-    def _select_obj_handler(cls, resources: Any) -> MediaStream:
-        if isinstance(resources, str) and "://" in resources:
-            return cls._expand_from_url
-        if isinstance(resources, (Path, str)):
-            return cls._expand_from_paths
-
-        for class_or_package_name, method_name in obj_handlers.items():
-            module = getattr(resources, "__module__", "").split(".", maxsplit=1)[0]
-            type_ = type(resources).__name__
-            if (
-                f"{module}.{type_}" == class_or_package_name
-                or module == class_or_package_name
-            ):
-                return getattr(cls, method_name)
-
-        raise ValueError(
-            f"Could not find a method to handle {type(resources)}; "
-            f"supported classes/packages are {list(obj_handlers.keys())}."
-        )
-
-    @classmethod
-    def _expand_from_xarray(
-        cls,
-        resources: xr.Dataset | xr.DataArray,
-        renderer: Callable | None = None,
-        renderer_iterables: list[Any] | None = None,
-        renderer_kwargs: dict | None = None,
-        **kwargs,
-    ):
-        ds = resources
-        dim = kwargs.pop("dim", None)
-        var = kwargs.pop("var", None)
-
-        ds = _utils.validate_xarray(ds, dim=dim, var=var)
-        if not dim:
-            dim = list(ds.dims)[0]
-            _utils.warn_default_used("dim", dim, suffix="from the dataset")
-        elif dim not in ds.dims:
-            raise ValueError(f"{dim!r} not in {ds.dims!r}")
-
-        total_frames = len(ds[dim])
-        max_frames = _utils.get_max_frames(total_frames, kwargs.get("max_frames"))
-        resources = [ds.isel({dim: i}) for i in range(max_frames)]
-
-        renderer_kwargs = renderer_kwargs or {}
-        renderer_kwargs.update(_utils.pop_from_cls(cls, kwargs))
-
-        if renderer is None:
-            renderer = wrap_matplotlib(
-                in_memory=kwargs.get("in_memory"),
-                scratch_dir=kwargs.get("scratch_dir"),
-            )(default_xarray_renderer)
-            ds_0 = resources[0]
-            if ds_0.ndim >= 2:
-                renderer_kwargs["vmin"] = renderer_kwargs.get(
-                    "vmin", _utils.get_result(ds_0.min()).item()
-                )
-                renderer_kwargs["vmax"] = renderer_kwargs.get(
-                    "vmax", _utils.get_result(ds_0.max()).item()
-                )
-            else:
-                renderer_kwargs["ylim"] = renderer_kwargs.get(
-                    "ylim",
-                    (
-                        _utils.get_result(ds_0.min()).item(),
-                        _utils.get_result(ds_0.max()).item(),
-                    ),
-                )
-        return resources, renderer, renderer_iterables, renderer_kwargs, kwargs
-
-    @classmethod
-    def _expand_from_pandas(
-        cls,
-        resources: pd.DataFrame,
-        renderer: Callable | None = None,
-        renderer_iterables: list[Any] | None = None,
-        renderer_kwargs: dict | None = None,
-        **kwargs,
-    ):
-        import pandas as pd
-
-        df = resources
-        groupby = kwargs.get("groupby")
-
-        total_frames = df.groupby(groupby).size().max() if groupby else len(df)
-        max_frames = _utils.get_max_frames(total_frames, kwargs.get("max_frames"))
-        resources = [
-            df.groupby(groupby, as_index=False).head(i) if groupby else df.head(i)
-            for i in range(1, max_frames + 1)
-        ]
-
-        renderer_kwargs = renderer_kwargs or {}
-        renderer_kwargs.update(_utils.pop_from_cls(cls, kwargs))
-
-        if renderer is None:
-            renderer = wrap_matplotlib(
-                in_memory=kwargs.get("in_memory"),
-                scratch_dir=kwargs.get("scratch_dir"),
-            )(default_pandas_renderer)
-            if "x" not in renderer_kwargs:
-                if df.index.name or isinstance(df, pd.Series):
-                    renderer_kwargs["x"] = df.index.name
-                else:
-                    for col in df.columns:
-                        if col != groupby:
-                            break
-                    renderer_kwargs["x"] = col
-                _utils.warn_default_used(
-                    "x", renderer_kwargs["x"], suffix="from the dataframe"
-                )
-            if "y" not in renderer_kwargs:
-                if isinstance(df, pd.Series):
-                    col = df.name
-                else:
-                    numeric_cols = df.select_dtypes(include="number").columns
-                    for col in numeric_cols:
-                        if col not in (renderer_kwargs["x"], groupby):
-                            break
-                renderer_kwargs["y"] = col
-                _utils.warn_default_used(
-                    "y", renderer_kwargs["y"], suffix="from the dataframe"
-                )
-            if "xlabel" not in renderer_kwargs:
-                renderer_kwargs["xlabel"] = (
-                    renderer_kwargs["x"].title().replace("_", " ")
-                )
-            if "ylabel" not in renderer_kwargs:
-                renderer_kwargs["ylabel"] = (
-                    renderer_kwargs["y"].title().replace("_", " ")
-                )
-
-        return resources, renderer, renderer_iterables, renderer_kwargs, kwargs
-
-    @classmethod
-    def _expand_from_holoviews(
-        cls,
-        resources: hv.HoloMap | hv.DynamicMap,
-        renderer: Callable | None = None,
-        renderer_iterables: list[Any] | None = None,
-        renderer_kwargs: dict | None = None,
-        **kwargs,
-    ):
-        import holoviews as hv
-
-        backend = hv.Store.current_backend
-        hv.extension(backend)
-
-        def _select_element(hv_obj, key):
-            try:
-                resource = hv_obj[key]
-            except Exception:
-                resource = hv_obj.select(**{kdims[0].name: key})
-            return resource
-
-        hv_obj = resources
-        if isinstance(hv_obj, (hv.core.spaces.DynamicMap, hv.core.spaces.HoloMap)):
-            hv_map = hv_obj
-        elif issubclass(
-            type(hv_obj), (hv.core.layout.Layoutable, hv.core.overlay.Overlayable)
-        ):
-            hv_map = hv_obj[0]
-
-        if not isinstance(hv_map, (hv.core.spaces.DynamicMap, hv.core.spaces.HoloMap)):
-            raise ValueError("Can only handle HoloMap and DynamicMap objects.")
-        elif isinstance(hv_map, hv.core.spaces.DynamicMap):
-            kdims = hv_map.kdims
-            keys = hv_map.kdims[0].values
-        else:
-            kdims = hv_map.kdims
-            keys = hv_map.keys()
-
-        if len(kdims) > 1:
-            raise ValueError("Can only handle 1D HoloViews objects.")
-
-        resources = [_select_element(hv_obj, key).opts(title=str(key)) for key in keys]
-
-        renderer_kwargs = renderer_kwargs or {}
-        renderer_kwargs.update(_utils.pop_from_cls(cls, kwargs))
-
-        if renderer is None:
-            renderer = wrap_holoviews(
-                in_memory=kwargs.get("in_memory"),
-                scratch_dir=kwargs.get("scratch_dir"),
-            )(default_holoviews_renderer)
-            clims = {}
-            for hv_el in hv_obj.traverse(full_breadth=False):
-                if isinstance(hv_el, hv.DynamicMap):
-                    hv.render(hv_el, backend=backend)
-
-                if isinstance(hv_el, hv.Element):
-                    if hv_el.ndims > 1:
-                        vdim = hv_el.vdims[0].name
-                        array = hv_el.dimension_values(vdim)
-                        clim = (np.nanmin(array), np.nanmax(array))
-                        clims[vdim] = clim
-            renderer_kwargs.update(
-                backend=backend,
-                clims=clims,
-            )
-
-        if kwargs.get("processes"):
-            cls.logger.warning(
-                "HoloViews rendering does not support processes; "
-                "setting processes=False."
-            )
-        kwargs["processes"] = False
-        return resources, renderer, renderer_iterables, renderer_kwargs, kwargs
-
-    @classmethod
-    def _expand_from_url(
+    def from_xarray(
         cls,
-        resources: str,
+        ds: xr.Dataset | xr.DataArray,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
+        dim: str | None = None,
+        var: str | None = None,
         **kwargs,
     ) -> MediaStream:
-        import re
-
-        import requests
-        from bs4 import BeautifulSoup
-
-        base_url = resources
-        pattern = kwargs.pop("pattern", None)
-        sort_key = kwargs.pop("sort_key", None)
-        max_files = kwargs.pop("max_files", None)
-        file_handler = kwargs.pop("file_handler", None)
-        file_handler_kwargs = kwargs.pop("file_handler_kwargs", None)
-
-        response = requests.get(resources)
-        content_type = response.headers.get("Content-Type")
-
-        if pattern is not None:
-            response.raise_for_status()
-            soup = BeautifulSoup(response.text, "html.parser")
-            href = re.compile(pattern.replace("*", ".*"))
-            links = soup.find_all("a", href=href)
-        else:
-            if content_type.startswith("text"):
-                raise ValueError(
-                    f"A pattern must be provided if the URL is a directory of files; "
-                    f"got {resources!r}."
-                )
-            links = [{"href": ""}]
-
-        max_files = _utils.get_config_default(
-            "max_files", max_files, total_value=len(links), suffix="links"
-        )
-        if max_files > 0:
-            links = links[:max_files]
-
-        if len(links) == 0:
-            raise ValueError(
-                f"No links found with pattern {pattern!r} at {base_url!r}."
-            )
-
-        # download files
-        urls = [base_url + link.get("href") for link in links]
-        client = _utils.get_distributed_client(
-            client=kwargs.get("client"),
-            processes=kwargs.get("processes"),
-            threads_per_worker=kwargs.get("threads_per_worker"),
-        )
-
-        futures = _utils.map_over(
-            client,
-            _utils.download_file,
-            urls,
-            kwargs.get("batch_size"),
-            scratch_dir=kwargs.get("scratch_dir"),
-            in_memory=kwargs.get("in_memory"),
-        )
-        paths = client.gather(futures)
-        return cls._expand_from_paths(
-            paths,
-            sort_key=sort_key,
-            max_files=max_files,
-            file_handler=file_handler,
-            file_handler_kwargs=file_handler_kwargs,
+        serialized = serialize_xarray(
+            cls,
+            ds,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
+            dim=dim,
+            var=var,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
-    def _expand_from_paths(
-        cls,
-        resources: list[str | Path] | str,
-        renderer: Callable | None = None,
-        renderer_iterables: list[Any] | None = None,
-        renderer_kwargs: dict | None = None,
-        **kwargs,
-    ) -> MediaStream:
-        if isinstance(resources, str):
-            resources = [resources]
-
-        sort_key = kwargs.pop("sort_key", None)
-        max_files = kwargs.pop("max_files", None)
-        file_handler = kwargs.pop("file_handler", None)
-        file_handler_kwargs = kwargs.pop("file_handler_kwargs", None)
-
-        paths = sorted(resources, key=sort_key)
-
-        max_files = _utils.get_config_default(
-            "max_files", max_files, total_value=len(paths), suffix="paths"
-        )
-        if max_files > 0:
-            paths = paths[:max_files]
-
-        # find a file handler
-        extension = Path(paths[0]).suffix
-        file_handler_meta = file_handlers.get(extension, {})
-        file_handler_import_path = file_handler_meta.get("import_path")
-        file_handler_concat_path = file_handler_meta.get("concat_path")
-        if file_handler is None and file_handler_import_path is not None:
-            file_handler = _utils.import_function(file_handler_import_path)
-            if file_handler_concat_path is not None:
-                file_handler_concat = _utils.import_function(file_handler_concat_path)
-
-        # read as objects
-        if file_handler is not None:
-            if file_handler_concat_path is not None:
-                resources = file_handler_concat(
-                    file_handler(path, **(file_handler_kwargs or {})) for path in paths
-                )
-            else:
-                resources = file_handler(paths, **(file_handler_kwargs or {}))
-            return cls._expand_from_any(
-                resources, renderer, renderer_iterables, renderer_kwargs, **kwargs
-            )
-
-        # or simply return image paths
-        return paths, renderer, renderer_iterables, renderer_kwargs, kwargs
-
-    @classmethod
-    def _subset_resources_renderer_iterables(
-        cls, resources: Any, renderer_iterables: list[Any], max_frames: int
-    ):
-        if len(resources) > max_frames and max_frames != -1:
-            color = config["logging_warning_color"]
-            reset = config["logging_reset_color"]
-            cls.logger.warning(
-                f"There are a total of {len(resources)} frames, "
-                f"but streaming only {color}{max_frames}{reset}. "
-                f"Set max_frames to -1 to stream all frames."
-            )
-        resources = resources[: max_frames or max_frames]
-        renderer_iterables = [
-            iterable[: len(resources)] for iterable in renderer_iterables or []
-        ]
-        return resources, renderer_iterables
-
-    @classmethod
-    def _expand_from_any(
-        cls,
-        resources: Any,
-        renderer: Callable,
-        renderer_iterables: list[Any],
-        renderer_kwargs: dict[str, Any],
-        **kwargs,
-    ):
-        if not (isinstance(resources, (list, tuple)) or isgenerator(resources)):
-            obj_handler = cls._select_obj_handler(resources)
-            _utils.validate_renderer_iterables(resources, renderer_iterables)
-
-            resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-                obj_handler(
-                    resources,
-                    renderer=renderer,
-                    renderer_iterables=renderer_iterables,
-                    renderer_kwargs=renderer_kwargs,
-                    **kwargs,
-                )
-            )
-            max_frames = _utils.get_max_frames(len(resources), kwargs.get("max_frames"))
-            kwargs["max_frames"] = max_frames
-            resources, renderer_iterables = cls._subset_resources_renderer_iterables(
-                resources, renderer_iterables, max_frames
-            )
-            _utils.pop_kwargs(obj_handler, renderer_kwargs)
-            _utils.pop_kwargs(obj_handler, kwargs)
-        return resources, renderer, renderer_iterables, renderer_kwargs, kwargs
-
-    @classmethod
-    def from_xarray(
+    def from_pandas(
         cls,
-        ds: xr.Dataset | xr.DataArray,
+        df: pd.DataFrame,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
-        dim: str | None = None,
-        var: str | None = None,
+        groupby: str | None = None,
         **kwargs,
     ) -> MediaStream:
-        resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-            cls._expand_from_xarray(
-                ds,
-                renderer=renderer,
-                renderer_kwargs=renderer_kwargs,
-                dim=dim,
-                var=var,
-                **kwargs,
-            )
-        )
-        return cls(
-            resources=resources,
+        serialized = serialize_pandas(
+            cls,
+            resources=df,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
+            groupby=groupby,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
-    def from_pandas(
+    def from_polars(
         cls,
-        df: pd.DataFrame,
+        df: pl.DataFrame,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
         groupby: str | None = None,
         **kwargs,
     ) -> MediaStream:
-        resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-            cls._expand_from_pandas(
-                df, renderer, renderer_kwargs, groupby=groupby, **kwargs
-            )
-        )
-        return cls(
-            resources=resources,
+        serialized = serialize_polars(
+            cls,
+            resources=df,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
+            groupby=groupby,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
     def from_holoviews(
         cls,
         hv_obj: hv.HoloMap | hv.DynamicMap,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
         **kwargs,
     ) -> MediaStream:
-        resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-            cls._expand_from_holoviews(hv_obj, renderer, renderer_kwargs, **kwargs)
-        )
-        return cls(
-            resources=resources,
+        serialized = serialize_holoviews(
+            cls,
+            resources=hv_obj,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
     def from_url(
         cls,
         base_url: str,
         pattern: str | None = None,
         sort_key: Callable | None = None,
@@ -652,35 +290,28 @@
         file_handler: Callable | None = None,
         file_handler_kwargs: dict | None = None,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
         **kwargs,
     ) -> MediaStream:
-        resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-            cls._expand_from_url(
-                base_url,
-                pattern=pattern,
-                sort_key=sort_key,
-                max_files=max_files,
-                file_handler=file_handler,
-                file_handler_kwargs=file_handler_kwargs,
-                renderer=renderer,
-                renderer_iterables=renderer_iterables,
-                renderer_kwargs=renderer_kwargs,
-                **kwargs,
-            )
-        )
-        return cls(
-            resources=resources,
+        serialized = serialize_url(
+            cls,
+            resources=base_url,
+            pattern=pattern,
+            sort_key=sort_key,
+            max_files=max_files,
+            file_handler=file_handler,
+            file_handler_kwargs=file_handler_kwargs,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
     def from_directory(
         cls,
         base_dir: str | Path,
         pattern: str,
         sort_key: Callable | None = None,
@@ -689,34 +320,27 @@
         file_handler_kwargs: dict | None = None,
         renderer: Callable | None = None,
         renderer_iterables: list[Any] | None = None,
         renderer_kwargs: dict | None = None,
         **kwargs,
     ) -> MediaStream:
         paths = Path(base_dir).glob(pattern)
-        resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-            cls._expand_from_paths(
-                paths,
-                sort_key=sort_key,
-                max_files=max_files,
-                file_handler=file_handler,
-                file_handler_kwargs=file_handler_kwargs,
-                renderer=renderer,
-                renderer_iterables=renderer_iterables,
-                renderer_kwargs=renderer_kwargs,
-                **kwargs,
-            )
-        )
-        return cls(
-            resources=resources,
+        serialized = serialize_paths(
+            cls,
+            resources=paths,
+            sort_key=sort_key,
+            max_files=max_files,
+            file_handler=file_handler,
+            file_handler_kwargs=file_handler_kwargs,
             renderer=renderer,
             renderer_iterables=renderer_iterables,
             renderer_kwargs=renderer_kwargs,
             **kwargs,
         )
+        return cls(**serialized.param.values(), **serialized.kwargs)
 
     @classmethod
     def _display_in_notebook(
         cls, obj: Any, display: bool = True, is_media: bool = True
     ) -> None:
         if not _utils.using_notebook() or not display:
             return
@@ -794,23 +418,27 @@
             ]
             resources = dask.compute(jobs, scheduler="threads")[0]
         resource_0 = _utils.get_result(_utils.get_first(resources))
 
         is_like_image = isinstance(resource_0, np.ndarray) and resource_0.ndim == 3
         if not is_like_image:
             try:
-                _utils.imread_with_pause(resource_0)
+                _utils.imread_with_pause(resource_0, fsspec_fs=self.fsspec_fs)
             except Exception as exc:
                 raise ValueError(
                     f"Could not read the first resource as an image: {resource_0!r}; "
                     f"if matplotlib or holoviews, try wrapping it with "
                     f"`streamjoy.wrap_matplotlib` or `streamjoy.wrap_holoviews`."
                 ) from exc
             images = _utils.map_over(
-                self.client, _utils.imread_with_pause, resources, batch_size
+                self.client,
+                _utils.imread_with_pause,
+                resources,
+                batch_size,
+                fsspec_fs=self.fsspec_fs,
             )
         else:
             images = resources
 
         del resource_0
         return images
 
@@ -907,17 +535,22 @@
             else:
                 renderer_kwargs[key] = value
 
         if resources is None:
             resources = self.resources
             renderer_iterables = self.renderer_iterables
         else:
-            resources, renderer, renderer_iterables, renderer_kwargs, kwargs = (
-                self._expand_from_any(resources, renderer, renderer_kwargs, **kwargs)
+            serialized = serialize_appropriately(
+                self, resources, renderer, renderer_kwargs, **kwargs
             )
+            resources = serialized.resources
+            renderer = serialized.renderer
+            renderer_iterables = serialized.renderer_iterables
+            renderer_kwargs = serialized.renderer_kwargs
+            kwargs = serialized.kwargs
 
         # Do this after for efficiency; also it's possible processes is set to False
         self.client = _utils.get_distributed_client(
             self.client,
             processes=self.processes,
             threads_per_worker=self.threads_per_worker,
         )
@@ -990,14 +623,15 @@
             f"---\n"
             f"Output:\n"
             f"  max_frames: {self.max_frames}\n"
             f"  fps: {self.fps}\n"
             f"  display: {self.display}\n"
             f"  scratch_dir: {self.scratch_dir}\n"
             f"  in_memory: {self.in_memory}\n"
+            f"  fsspec_fs: {self.fsspec_fs}\n"
         )
 
         if self.intro_title or self.intro_subtitle or self.intro_watermark:
             repr_str += "---\nIntro:\n"
             repr_str += f"  intro_title: {self.intro_title}\n"
             repr_str += f"  intro_subtitle: {self.intro_subtitle}\n"
             repr_str += f"  intro_watermark: {self.intro_watermark}\n"
@@ -1111,15 +745,15 @@
         if init:
             init_kwargs["fps"] = self.fps
             buf.init_video_stream(self.codec, **init_kwargs)
 
         intro_frame = self._create_intro(images)
         self._prepend_intro(buf, intro_frame, **write_kwargs)
 
-        for image in images:
+        for i, image in enumerate(images):
             image = _utils.get_result(image)
 
             pause = None
             if isinstance(image, Paused):
                 pause = image.seconds
                 image = image.output
 
@@ -1131,17 +765,19 @@
             buf.write_frame(image, **write_kwargs)
 
             if pause is not None:
                 _utils.repeat_frame(
                     buf.write_frame, image, pause, self.fps, **write_kwargs
                 )
 
-        _utils.repeat_frame(
-            buf.write_frame, image, self.ending_pause, self.fps, **write_kwargs
-        )
+            if i == len(images) - 1:
+                _utils.repeat_frame(
+                    buf.write_frame, image, self.ending_pause, self.fps, **write_kwargs
+                )
+            del image
 
     def write(
         self,
         uri: str | Path | BytesIO | None = None,
         resources: Any | None = None,
         **kwargs: dict[str, Any],
     ) -> Path | BytesIO:
@@ -1436,15 +1072,15 @@
                     stream.intro_title, stream.intro_subtitle, len(stream)
                 )
 
         with iio.imopen(uri, "w", extension=extension) as buf:
             for i, stream in enumerate(streams):
                 stream.client = client
                 resources, renderer_iterables = (
-                    stream._subset_resources_renderer_iterables(
+                    _utils.subset_resources_renderer_iterables(
                         stream.resources, stream.renderer_iterables, stream.max_frames
                     )
                 )
                 images = stream._render_images(
                     resources,
                     stream.renderer,
                     renderer_iterables,
```

### Comparing `streamjoy-0.0.2/streamjoy/wrappers.py` & `streamjoy-0.0.3/streamjoy/wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from __future__ import annotations
 
 from functools import wraps
 from io import BytesIO
 from pathlib import Path
-from typing import Callable
+from typing import Any, Callable
 
 from . import _utils
 from .models import Paused
 from .settings import config
 
 
 def wrap_matplotlib(
-    in_memory: bool = False, scratch_dir: str | Path | None = None
+    in_memory: bool = False,
+    scratch_dir: str | Path | None = None,
+    fsspec_fs: Any | None = None,
 ) -> Callable:
     """
     Wraps a function used to render a matplotlib figure so that
     it automatically saves the figure and closes it.
 
     Args:
         in_memory: Whether to render the figure in-memory.
         scratch_dir: The scratch directory to use.
+        fsspec_fs: The fsspec filesystem to use.
 
     Returns:
         The wrapped function.
     """
 
     def wrapper(renderer):
         @wraps(renderer)
@@ -48,28 +51,38 @@
             elif not isinstance(fig, plt.Figure):
                 raise ValueError("Renderer must return a Figure or Axes object.")
 
             uri = _utils.resolve_uri(
                 file_name=f"{hash(fig)}.jpg",
                 scratch_dir=scratch_dir,
                 in_memory=in_memory,
+                fsspec_fs=fsspec_fs,
             )
-            fig.savefig(uri, format="jpg")
+            if fsspec_fs:
+                with fsspec_fs.open(uri, "wb") as f:
+                    buf = BytesIO()
+                    fig.savefig(buf, format="jpg")
+                    buf.seek(0)
+                    f.write(buf.read())
+            else:
+                fig.savefig(uri, format="jpg")
             plt.close(fig)
             return (
                 uri if not return_paused else Paused(output=uri, seconds=output.seconds)
             )
 
         return wrapped
 
     return wrapper
 
 
 def wrap_holoviews(
-    in_memory: bool = False, scratch_dir: str | Path | None = None
+    in_memory: bool = False,
+    scratch_dir: str | Path | None = None,
+    fsspec_fs: Any | None = None,
 ) -> Callable:
     """
     Wraps a function used to render a holoviews object so that
     it automatically saves the object.
 
     Args:
         in_memory: Whether to render the object in-memory.
@@ -82,29 +95,30 @@
         raise ValueError("Holoviews renderer does not support in-memory rendering.")
 
     def wrapper(renderer):
         @wraps(renderer)
         def wrapped(*args, **kwargs) -> Path | BytesIO:
             import holoviews as hv
 
-            backend = kwargs.get("backend", hv.Store.current_backend)
+            backend = kwargs.get("backend", "bokeh")
             hv.extension(backend)
 
             output = renderer(*args, **kwargs)
 
             hv_obj = output
             return_paused = False
             if isinstance(output, Paused):
                 return_paused = True
                 hv_obj = output.output
 
             uri = _utils.resolve_uri(
                 file_name=f"{hash(hv_obj)}.png",
                 scratch_dir=scratch_dir,
                 in_memory=in_memory,
+                fsspec_fs=fsspec_fs,
             )
             if backend == "bokeh":
                 from bokeh.io.export import export_png
                 from selenium.webdriver.chrome.options import Options
                 from selenium.webdriver.chrome.webdriver import Service, WebDriver
                 from webdriver_manager.chrome import ChromeDriverManager
 
@@ -116,15 +130,22 @@
                 ) as webdriver:
                     export_png(
                         hv.render(hv_obj, backend="bokeh"),
                         filename=uri,
                         webdriver=webdriver,
                     )
             else:
-                hv.save(hv_obj, uri, fmt="png")
+                if fsspec_fs:
+                    with fsspec_fs.open(uri, "wb") as f:
+                        buf = BytesIO()
+                        hv.save(hv_obj, buf, fmt="png")
+                        buf.seek(0)
+                        f.write(buf.read())
+                else:
+                    hv.save(hv_obj, uri, fmt="png")
 
             return (
                 uri if not return_paused else Paused(output=uri, seconds=output.seconds)
             )
 
         return wrapped
```

### Comparing `streamjoy-0.0.2/streamjoy/xarray.py` & `streamjoy-0.0.3/streamjoy/xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/conftest.py` & `streamjoy-0.0.3/tests/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
 
 import hvplot.xarray  # noqa: F401
 import pandas as pd
+import polars as pl
 import pytest
 import xarray as xr
 
 from streamjoy._utils import get_distributed_client
 from streamjoy.settings import config
 
 DATA_DIR = Path(__file__).parent / "data"
@@ -22,14 +23,19 @@
 
 @pytest.fixture
 def df():
     return pd.read_parquet(PARQUET_PATH)
 
 
 @pytest.fixture
+def pl_df():
+    return pl.read_parquet(PARQUET_PATH)
+
+
+@pytest.fixture
 def dmap(ds):
     return ds.hvplot("lon", "lat", dynamic=True)
 
 
 @pytest.fixture
 def hmap(ds):
     return ds.hvplot("lon", "lat", dynamic=False)
@@ -47,7 +53,17 @@
     config["max_files"] = 2
     config["ending_pause"] = 0
 
 
 @pytest.fixture(scope="session")
 def data_dir():
     return DATA_DIR
+
+
+@pytest.fixture(scope="session")
+def fsspec_fs():
+    try:
+        import fsspec
+
+        return fsspec.filesystem("file")
+    except ImportError:
+        pytest.skip("fsspec not installed")
```

### Comparing `streamjoy-0.0.2/tests/test_core.py` & `streamjoy-0.0.3/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_models.py` & `streamjoy-0.0.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_pandas.py` & `streamjoy-0.0.3/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_renderers.py` & `streamjoy-0.0.3/tests/test_renderers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_settings.py` & `streamjoy-0.0.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_streams.py` & `streamjoy-0.0.3/tests/test_streams.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,18 @@
         props = improps(buf)
         props.n_images == 3
 
     def test_from_pandas(self, stream_cls, df):
         sj = stream_cls.from_pandas(df)
         self._assert_stream_and_props(sj, stream_cls)
 
+    def test_from_polars(self, stream_cls, pl_df):
+        sj = stream_cls.from_polars(pl_df)
+        self._assert_stream_and_props(sj, stream_cls)
+
     def test_from_xarray(self, stream_cls, ds):
         sj = stream_cls.from_xarray(ds)
         self._assert_stream_and_props(sj, stream_cls)
 
     def test_from_holoviews_hmap(self, stream_cls, hmap):
         sj = stream_cls.from_holoviews(hmap)
         self._assert_stream_and_props(sj, stream_cls)
@@ -42,14 +46,18 @@
         )
         self._assert_stream_and_props(sj, stream_cls)
 
     def test_from_directory(self, stream_cls, data_dir):
         sj = stream_cls.from_directory(data_dir, pattern="*.png")
         self._assert_stream_and_props(sj, stream_cls)
 
+    def test_fsspec_fs(self, stream_cls, df, fsspec_fs):
+        sj = stream_cls.from_pandas(df, fsspec_fs=fsspec_fs)
+        self._assert_stream_and_props(sj, stream_cls)
+
 
 class TestGifStream(AbstractTestMediaStream):
     @pytest.fixture(scope="class")
     def stream_cls(self):
         return GifStream
 
     def test_paused(self, stream_cls, df):
```

### Comparing `streamjoy-0.0.2/tests/test_wrappers.py` & `streamjoy-0.0.3/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/test_xarray.py` & `streamjoy-0.0.3/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png` & `streamjoy-0.0.3/tests/data/1978_10_Oct_N_19781026_conc_v3.0.png`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png` & `streamjoy-0.0.3/tests/data/1978_10_Oct_N_19781027_conc_v3.0.png`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/air.nc` & `streamjoy-0.0.3/tests/data/air.nc`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/gapminder.csv` & `streamjoy-0.0.3/tests/data/gapminder.csv`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/gapminder.parquet` & `streamjoy-0.0.3/tests/data/gapminder.parquet`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/air.zarr/.zmetadata` & `streamjoy-0.0.3/tests/data/air.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/tests/data/air.zarr/air/0.0.0` & `streamjoy-0.0.3/tests/data/air.zarr/air/0.0.0`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/.gitignore` & `streamjoy-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/LICENSE` & `streamjoy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/README.md` & `streamjoy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `streamjoy-0.0.2/pyproject.toml` & `streamjoy-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "ruff",
     "pytest",
     "pytest-cov",
     "mkdocs-material",
     "mkdocstrings[python]",
     "xarray",
     "pandas",
+    "polars",
     "zarr",
     "netcdf4",
     "matplotlib",
     "pyarrow",
     "hvplot",
     "bs4",
     "selenium",
@@ -74,12 +75,14 @@
 requires-python = ">=3.9"
 dependencies = [
     "param",
     "bokeh",
     "dask[distributed]",
     "imageio[pyav]>=2.34.0",
     "pygifsicle==1.0.5",
+    "requests",
+    "bs4",
 ]
 
 [project.urls]
 Documentation = "https://ahuang11.github.io/streamjoy/"
 Source = "https://github.com/ahuang11/streamjoy"
```

### Comparing `streamjoy-0.0.2/PKG-INFO` & `streamjoy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.3
 Name: streamjoy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Enjoy animating images into GIFs and MP4s!
 Project-URL: Documentation, https://ahuang11.github.io/streamjoy/
 Project-URL: Source, https://github.com/ahuang11/streamjoy
 Author-email: streamjoy <hey.at.py@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
 Requires-Dist: bokeh
+Requires-Dist: bs4
 Requires-Dist: dask[distributed]
 Requires-Dist: imageio[pyav]>=2.34.0
 Requires-Dist: param
 Requires-Dist: pygifsicle==1.0.5
+Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # 🌈 StreamJoy 😊
 
 ---
 
 [![build](https://github.com/ahuang11/streamjoy/workflows/Build/badge.svg)](https://github.com/ahuang11/streamjoy/actions) [![codecov](https://codecov.io/gh/ahuang11/streamjoy/branch/master/graph/badge.svg)](https://codecov.io/gh/ahuang11/streamjoy) [![PyPI version](https://badge.fury.io/py/streamjoy.svg)](https://badge.fury.io/py/streamjoy)
```

