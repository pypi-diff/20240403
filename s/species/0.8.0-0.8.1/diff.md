# Comparing `tmp/species-0.8.0.tar.gz` & `tmp/species-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "species-0.8.0.tar", last modified: Wed Mar  6 08:42:59 2024, max compression
+gzip compressed data, was "species-0.8.1.tar", last modified: Wed Apr  3 20:09:49 2024, max compression
```

## Comparing `species-0.8.0.tar` & `species-0.8.1.tar`

### file list

```diff
@@ -1,108 +1,110 @@
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.300385 species-0.8.0/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2023-09-26 09:49:21.000000 species-0.8.0/LICENSE
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4082 2024-03-06 08:42:59.300213 species-0.8.0/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3294 2024-02-16 14:11:29.000000 species-0.8.0/README.rst
--rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2024-03-06 08:42:59.300433 species-0.8.0/setup.cfg
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1324 2024-03-06 08:16:52.000000 species-0.8.0/setup.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.265326 species-0.8.0/species/
--rw-r--r--   0 tomasstolker   (501) staff       (20)      223 2024-03-06 08:16:17.000000 species-0.8.0/species/__init__.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.267664 species-0.8.0/species/core/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.0/species/core/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    14867 2023-11-19 10:12:35.000000 species-0.8.0/species/core/box.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      880 2023-11-08 06:43:57.000000 species-0.8.0/species/core/constants.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5016 2024-03-04 20:31:49.000000 species-0.8.0/species/core/species_init.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.268203 species-0.8.0/species/data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)       23 2023-11-08 20:53:44.000000 species-0.8.0/species/data/__init__.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.269517 species-0.8.0/species/data/companion_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:16.000000 species-0.8.0/species/data/companion_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2683 2024-02-17 07:17:18.000000 species-0.8.0/species/data/companion_data/companion_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   163375 2024-03-05 20:01:52.000000 species-0.8.0/species/data/database.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.269983 species-0.8.0/species/data/filter_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:26.000000 species-0.8.0/species/data/filter_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8767 2024-01-30 09:26:08.000000 species-0.8.0/species/data/filter_data/filter_data.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.273747 species-0.8.0/species/data/isochrone_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:36.000000 species-0.8.0/species/data/isochrone_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3250 2023-11-09 19:21:10.000000 species-0.8.0/species/data/isochrone_data/add_isochrone.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1425 2023-11-12 06:39:59.000000 species-0.8.0/species/data/isochrone_data/iso_ames.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4003 2023-11-12 06:41:33.000000 species-0.8.0/species/data/isochrone_data/iso_atmo.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2277 2023-11-12 06:43:13.000000 species-0.8.0/species/data/isochrone_data/iso_baraffe2015.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1116 2023-11-12 06:42:46.000000 species-0.8.0/species/data/isochrone_data/iso_btsettl.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5161 2023-11-12 06:43:39.000000 species-0.8.0/species/data/isochrone_data/iso_linder2019.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3486 2023-11-12 06:43:55.000000 species-0.8.0/species/data/isochrone_data/iso_manual.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1459 2023-11-12 06:44:16.000000 species-0.8.0/species/data/isochrone_data/iso_marleau.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1112 2023-11-12 06:44:39.000000 species-0.8.0/species/data/isochrone_data/iso_nextgen.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3737 2023-11-12 06:45:25.000000 species-0.8.0/species/data/isochrone_data/iso_saumon2008.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3674 2023-11-12 06:45:50.000000 species-0.8.0/species/data/isochrone_data/iso_sonora.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.274438 species-0.8.0/species/data/misc_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:47.000000 species-0.8.0/species/data/misc_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4193 2023-11-01 12:20:50.000000 species-0.8.0/species/data/misc_data/accretion_data.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6323 2024-02-17 08:50:04.000000 species-0.8.0/species/data/misc_data/dust_data.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.275270 species-0.8.0/species/data/model_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:57.000000 species-0.8.0/species/data/model_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    10210 2024-03-05 12:07:32.000000 species-0.8.0/species/data/model_data/custom_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    13753 2024-03-05 12:06:52.000000 species-0.8.0/species/data/model_data/model_spectra.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.276006 species-0.8.0/species/data/phot_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:06.000000 species-0.8.0/species/data/phot_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6426 2023-11-12 06:47:44.000000 species-0.8.0/species/data/phot_data/phot_leggett.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3332 2024-02-17 07:13:44.000000 species-0.8.0/species/data/phot_data/phot_vlm_plx.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.278379 species-0.8.0/species/data/spec_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:16.000000 species-0.8.0/species/data/spec_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1926 2023-11-08 18:11:34.000000 species-0.8.0/species/data/spec_data/add_spec_data.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5208 2023-11-08 10:46:04.000000 species-0.8.0/species/data/spec_data/spec_allers2013.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4183 2023-11-08 10:46:50.000000 species-0.8.0/species/data/spec_data/spec_bonnefoy2014.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6288 2023-11-08 10:46:39.000000 species-0.8.0/species/data/spec_data/spec_irtf.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2862 2023-11-08 10:46:45.000000 species-0.8.0/species/data/spec_data/spec_kesseli2017.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8403 2023-11-08 10:46:35.000000 species-0.8.0/species/data/spec_data/spec_spex.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2746 2024-02-17 07:21:56.000000 species-0.8.0/species/data/spec_data/spec_vega.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.282096 species-0.8.0/species/fit/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.0/species/fit/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    31343 2023-11-12 13:45:57.000000 species-0.8.0/species/fit/compare_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    43793 2023-11-01 12:36:23.000000 species-0.8.0/species/fit/emission_line.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    27958 2024-02-14 20:11:52.000000 species-0.8.0/species/fit/fit_evolution.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   105218 2024-03-05 19:47:11.000000 species-0.8.0/species/fit/fit_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6491 2023-11-01 12:43:51.000000 species-0.8.0/species/fit/fit_spectrum.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   163686 2024-02-16 14:08:53.000000 species-0.8.0/species/fit/retrieval.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.283031 species-0.8.0/species/phot/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-10-29 13:04:27.000000 species-0.8.0/species/phot/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    24175 2024-02-06 15:57:41.000000 species-0.8.0/species/phot/syn_phot.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.287339 species-0.8.0/species/plot/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.0/species/plot/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    62134 2024-02-20 10:49:17.000000 species-0.8.0/species/plot/plot_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    38994 2024-02-06 09:51:28.000000 species-0.8.0/species/plot/plot_comparison.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    13747 2024-02-06 09:51:28.000000 species-0.8.0/species/plot/plot_evolution.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    45840 2024-02-14 09:22:31.000000 species-0.8.0/species/plot/plot_mcmc.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    49205 2024-02-06 09:51:28.000000 species-0.8.0/species/plot/plot_retrieval.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    48179 2024-02-17 08:36:19.000000 species-0.8.0/species/plot/plot_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.293921 species-0.8.0/species/read/
--rw-r--r--   0 tomasstolker   (501) staff       (20)      195 2023-11-08 13:49:49.000000 species-0.8.0/species/read/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    12304 2024-02-20 11:54:51.000000 species-0.8.0/species/read/read_calibration.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15748 2024-02-19 09:21:28.000000 species-0.8.0/species/read/read_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6820 2023-11-12 13:30:42.000000 species-0.8.0/species/read/read_filter.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    66511 2024-02-14 20:15:05.000000 species-0.8.0/species/read/read_isochrone.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    71304 2024-02-20 10:14:52.000000 species-0.8.0/species/read/read_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8399 2024-02-20 09:48:55.000000 species-0.8.0/species/read/read_object.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15897 2024-02-20 11:57:00.000000 species-0.8.0/species/read/read_planck.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    49873 2024-02-20 09:56:36.000000 species-0.8.0/species/read/read_radtrans.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    11572 2023-11-12 13:30:01.000000 species-0.8.0/species/read/read_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.299869 species-0.8.0/species/util/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.0/species/util/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6425 2024-02-20 10:40:18.000000 species-0.8.0/species/util/box_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6815 2023-11-01 11:49:39.000000 species-0.8.0/species/util/convert_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      742 2024-02-12 19:25:19.000000 species-0.8.0/species/util/core_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    32997 2024-02-20 13:06:53.000000 species-0.8.0/species/util/data_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    20230 2024-02-17 08:34:20.000000 species-0.8.0/species/util/dust_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15679 2024-02-20 10:40:43.000000 species-0.8.0/species/util/fit_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     9903 2024-02-20 08:29:29.000000 species-0.8.0/species/util/model_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    46506 2024-02-20 12:24:28.000000 species-0.8.0/species/util/plot_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8068 2023-12-21 09:32:43.000000 species-0.8.0/species/util/query_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8595 2024-02-01 09:26:59.000000 species-0.8.0/species/util/radtrans_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    95626 2024-02-08 09:34:32.000000 species-0.8.0/species/util/retrieval_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4667 2024-03-05 11:12:15.000000 species-0.8.0/species/util/spec_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      763 2024-02-14 20:12:21.000000 species-0.8.0/species/util/test_util.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-03-06 08:42:59.266557 species-0.8.0/species.egg-info/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4082 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2823 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/SOURCES.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/dependency_links.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/not-zip-safe
--rw-r--r--   0 tomasstolker   (501) staff       (20)      407 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/requires.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2024-03-06 08:42:59.000000 species-0.8.0/species.egg-info/top_level.txt
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.604846 species-0.8.1/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2023-09-26 09:49:21.000000 species-0.8.1/LICENSE
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:09:49.604680 species-0.8.1/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3513 2024-04-03 18:12:34.000000 species-0.8.1/README.rst
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2024-04-03 20:09:49.604894 species-0.8.1/setup.cfg
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1339 2024-04-03 18:22:51.000000 species-0.8.1/setup.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.567799 species-0.8.1/species/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      223 2024-04-03 18:22:47.000000 species-0.8.1/species/__init__.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.569615 species-0.8.1/species/core/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/core/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15235 2024-03-26 09:45:01.000000 species-0.8.1/species/core/box.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      880 2023-11-08 06:43:57.000000 species-0.8.1/species/core/constants.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4863 2024-03-30 11:12:28.000000 species-0.8.1/species/core/species_init.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.570254 species-0.8.1/species/data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       23 2023-11-08 20:53:44.000000 species-0.8.1/species/data/__init__.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.573613 species-0.8.1/species/data/companion_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:16.000000 species-0.8.1/species/data/companion_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    55027 2024-01-22 08:40:35.000000 species-0.8.1/species/data/companion_data/companion_data.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1948 2023-09-26 09:49:21.000000 species-0.8.1/species/data/companion_data/companion_spectra.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2683 2024-02-17 07:17:18.000000 species-0.8.1/species/data/companion_data/companion_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   175685 2024-03-26 08:30:19.000000 species-0.8.1/species/data/database.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.574082 species-0.8.1/species/data/filter_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:26.000000 species-0.8.1/species/data/filter_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8767 2024-01-30 09:26:08.000000 species-0.8.1/species/data/filter_data/filter_data.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.577628 species-0.8.1/species/data/isochrone_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:36.000000 species-0.8.1/species/data/isochrone_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3250 2023-11-09 19:21:10.000000 species-0.8.1/species/data/isochrone_data/add_isochrone.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1425 2023-11-12 06:39:59.000000 species-0.8.1/species/data/isochrone_data/iso_ames.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4003 2023-11-12 06:41:33.000000 species-0.8.1/species/data/isochrone_data/iso_atmo.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2277 2023-11-12 06:43:13.000000 species-0.8.1/species/data/isochrone_data/iso_baraffe2015.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1116 2023-11-12 06:42:46.000000 species-0.8.1/species/data/isochrone_data/iso_btsettl.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5161 2023-11-12 06:43:39.000000 species-0.8.1/species/data/isochrone_data/iso_linder2019.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3486 2023-11-12 06:43:55.000000 species-0.8.1/species/data/isochrone_data/iso_manual.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1459 2023-11-12 06:44:16.000000 species-0.8.1/species/data/isochrone_data/iso_marleau.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1112 2023-11-12 06:44:39.000000 species-0.8.1/species/data/isochrone_data/iso_nextgen.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3737 2023-11-12 06:45:25.000000 species-0.8.1/species/data/isochrone_data/iso_saumon2008.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3674 2023-11-12 06:45:50.000000 species-0.8.1/species/data/isochrone_data/iso_sonora.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.578354 species-0.8.1/species/data/misc_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:47.000000 species-0.8.1/species/data/misc_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4193 2023-11-01 12:20:50.000000 species-0.8.1/species/data/misc_data/accretion_data.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6337 2024-03-24 14:12:36.000000 species-0.8.1/species/data/misc_data/dust_data.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.579317 species-0.8.1/species/data/model_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:57.000000 species-0.8.1/species/data/model_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    10210 2024-03-05 12:07:32.000000 species-0.8.1/species/data/model_data/custom_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    14352 2024-03-27 09:23:03.000000 species-0.8.1/species/data/model_data/model_spectra.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.580090 species-0.8.1/species/data/phot_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:06.000000 species-0.8.1/species/data/phot_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6426 2023-11-12 06:47:44.000000 species-0.8.1/species/data/phot_data/phot_leggett.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3546 2024-03-15 21:22:31.000000 species-0.8.1/species/data/phot_data/phot_vlm_plx.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.582509 species-0.8.1/species/data/spec_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:16.000000 species-0.8.1/species/data/spec_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1926 2023-11-08 18:11:34.000000 species-0.8.1/species/data/spec_data/add_spec_data.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5208 2023-11-08 10:46:04.000000 species-0.8.1/species/data/spec_data/spec_allers2013.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4183 2023-11-08 10:46:50.000000 species-0.8.1/species/data/spec_data/spec_bonnefoy2014.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6288 2023-11-08 10:46:39.000000 species-0.8.1/species/data/spec_data/spec_irtf.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2862 2023-11-08 10:46:45.000000 species-0.8.1/species/data/spec_data/spec_kesseli2017.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8403 2023-11-08 10:46:35.000000 species-0.8.1/species/data/spec_data/spec_spex.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2746 2024-02-17 07:21:56.000000 species-0.8.1/species/data/spec_data/spec_vega.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.586911 species-0.8.1/species/fit/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/fit/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    31343 2023-11-12 13:45:57.000000 species-0.8.1/species/fit/compare_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    43793 2023-11-01 12:36:23.000000 species-0.8.1/species/fit/emission_line.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    27958 2024-02-14 20:11:52.000000 species-0.8.1/species/fit/fit_evolution.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   105263 2024-03-24 14:11:57.000000 species-0.8.1/species/fit/fit_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6491 2023-11-01 12:43:51.000000 species-0.8.1/species/fit/fit_spectrum.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   164928 2024-03-26 09:48:51.000000 species-0.8.1/species/fit/retrieval.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.588533 species-0.8.1/species/phot/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-10-29 13:04:27.000000 species-0.8.1/species/phot/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    24412 2024-03-30 16:08:28.000000 species-0.8.1/species/phot/syn_phot.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.593509 species-0.8.1/species/plot/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/plot/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    62134 2024-02-20 10:49:17.000000 species-0.8.1/species/plot/plot_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    38994 2024-02-06 09:51:28.000000 species-0.8.1/species/plot/plot_comparison.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    13747 2024-02-06 09:51:28.000000 species-0.8.1/species/plot/plot_evolution.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    48164 2024-03-24 14:07:32.000000 species-0.8.1/species/plot/plot_mcmc.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    49229 2024-03-24 14:08:47.000000 species-0.8.1/species/plot/plot_retrieval.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    53091 2024-03-27 09:35:07.000000 species-0.8.1/species/plot/plot_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.598394 species-0.8.1/species/read/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      195 2023-11-08 13:49:49.000000 species-0.8.1/species/read/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    12304 2024-02-20 11:54:51.000000 species-0.8.1/species/read/read_calibration.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15701 2024-03-19 13:24:36.000000 species-0.8.1/species/read/read_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     7145 2024-03-30 16:15:36.000000 species-0.8.1/species/read/read_filter.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    66511 2024-02-14 20:15:05.000000 species-0.8.1/species/read/read_isochrone.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    71397 2024-03-26 09:44:26.000000 species-0.8.1/species/read/read_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8595 2024-03-21 19:11:20.000000 species-0.8.1/species/read/read_object.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15897 2024-02-20 11:57:00.000000 species-0.8.1/species/read/read_planck.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    49839 2024-03-24 14:04:15.000000 species-0.8.1/species/read/read_radtrans.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    11572 2023-11-12 13:30:01.000000 species-0.8.1/species/read/read_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.604343 species-0.8.1/species/util/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/util/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6515 2024-03-25 20:42:03.000000 species-0.8.1/species/util/box_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6815 2023-11-01 11:49:39.000000 species-0.8.1/species/util/convert_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      742 2024-02-12 19:25:19.000000 species-0.8.1/species/util/core_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    36789 2024-03-26 13:25:02.000000 species-0.8.1/species/util/data_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    20231 2024-03-24 13:59:15.000000 species-0.8.1/species/util/dust_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15678 2024-03-24 13:59:15.000000 species-0.8.1/species/util/fit_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    10146 2024-03-27 08:20:31.000000 species-0.8.1/species/util/model_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    44468 2024-03-27 09:39:35.000000 species-0.8.1/species/util/plot_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8068 2023-12-21 09:32:43.000000 species-0.8.1/species/util/query_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8626 2024-03-24 13:59:15.000000 species-0.8.1/species/util/radtrans_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    95994 2024-03-26 09:34:14.000000 species-0.8.1/species/util/retrieval_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5124 2024-03-11 09:49:58.000000 species-0.8.1/species/util/spec_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      763 2024-02-14 20:12:21.000000 species-0.8.1/species/util/test_util.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.568744 species-0.8.1/species.egg-info/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2922 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/SOURCES.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/dependency_links.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/not-zip-safe
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      444 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/requires.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/top_level.txt
```

### Comparing `species-0.8.0/LICENSE` & `species-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `species-0.8.0/PKG-INFO` & `species-0.8.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,15 @@
-Metadata-Version: 2.1
-Name: species
-Version: 0.8.0
-Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
-Home-page: https://github.com/tomasstolker/species
-Author: Tomas Stolker
-Author-email: stolker@strw.leidenuniv.nl
-License: MIT
-Project-URL: Documentation, https://species.readthedocs.io
-Keywords: species
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Astronomy
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 *species*
 =========
 
 **spe**\ctral **c**\ haracterization and **i**\ nference for **e**\ xoplanet **s**\ cience
 
-.. image:: https://img.shields.io/pypi/v/species
-   :target: https://pypi.python.org/pypi/species
-
-.. image:: https://img.shields.io/pypi/pyversions/species
-   :target: https://pypi.python.org/pypi/species
-
-.. image:: https://github.com/tomasstolker/species/workflows/CI/badge.svg?branch=main
-   :target: https://github.com/tomasstolker/species/actions
-
-.. image:: https://img.shields.io/readthedocs/species
-   :target: http://species.readthedocs.io
-
-.. image:: https://codecov.io/gh/tomasstolker/species/branch/main/graph/badge.svg?token=LSSCPMJ5JH
-   :target: https://codecov.io/gh/tomasstolker/species
+.. container::
 
-.. image:: https://img.shields.io/codefactor/grade/github/tomasstolker/species
-   :target: https://www.codefactor.io/repository/github/tomasstolker/species
-
-.. image:: https://img.shields.io/github/license/tomasstolker/species
-   :target: https://github.com/tomasstolker/species/blob/main/LICENSE
+    |PyPI Status| |Python Versions| |CI Status| |Docs Status| |Code Coverage| |Code Quality| |License|
 
 *species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources.
 
 There are tools available for grid and free retrievals using Bayesian inference, synthetic photometry, interpolating a variety atmospheric and evolutionary model grids (including the possibility to add a custom grid), color-magnitude and color-color diagrams, empirical spectral analysis, spectral and photometric calibration, and analysis of emission lines. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on `Github <https://github.com/tomasstolker/species>`_.
 
 **Important:** Importing the *species* package had become slow because of the many classes and functions that were implicitly imported. The initialization of the package has therefore been adjusted. Any functionalities should now be explicitly imported from the modules that they are part of.
 
@@ -73,7 +35,28 @@
 
 License
 -------
 
 Copyright 2018-2024 Tomas Stolker
 
 *species* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/species/blob/main/LICENSE>`_ for the terms and conditions.
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/v/species
+   :target: https://pypi.python.org/pypi/species
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/species
+   :target: https://pypi.python.org/pypi/species
+
+.. |CI Status| image:: https://github.com/tomasstolker/species/workflows/CI/badge.svg?branch=main
+   :target: https://github.com/tomasstolker/species/actions
+
+.. |Docs Status| image:: https://img.shields.io/readthedocs/species
+   :target: http://species.readthedocs.io
+
+.. |Code Coverage| image:: https://codecov.io/gh/tomasstolker/species/branch/main/graph/badge.svg?token=LSSCPMJ5JH
+   :target: https://codecov.io/gh/tomasstolker/species
+
+.. |Code Quality| image:: https://img.shields.io/codefactor/grade/github/tomasstolker/species
+   :target: https://www.codefactor.io/repository/github/tomasstolker/species
+
+.. |License| image:: https://img.shields.io/github/license/tomasstolker/species
+   :target: https://github.com/tomasstolker/species/blob/main/LICENSE
```

### Comparing `species-0.8.0/setup.py` & `species-0.8.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,24 +5,24 @@
 
 with open("requirements.txt") as req_txt:
     parse_req = pkg_resources.parse_requirements(req_txt)
     install_requires = [str(req) for req in parse_req]
 
 setuptools.setup(
     name="species",
-    version="0.8.0",
+    version="0.8.1",
     description="Toolkit for atmospheric characterization of directly imaged exoplanets",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Tomas Stolker",
     author_email="stolker@strw.leidenuniv.nl",
     url="https://github.com/tomasstolker/species",
     project_urls={"Documentation": "https://species.readthedocs.io"},
     packages=setuptools.find_packages(include=["species", "species.*"]),
-    package_data={"species": ["data/*.json"]},
+    package_data={"species": ["data/companion_data/*.json"]},
     install_requires=install_requires,
     tests_require=["pytest"],
     license="MIT",
     zip_safe=False,
     keywords="species",
     classifiers=[
         "Development Status :: 4 - Beta",
```

### Comparing `species-0.8.0/species/core/box.py` & `species-0.8.1/species/core/box.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,14 +190,15 @@
         self.type = None
         self.wavelength = None
         self.flux = None
         self.parameters = None
         self.quantity = None
         self.contribution = None
         self.bol_flux = None
+        self.spec_res = None
 
     def smooth_spectrum(self, spec_res: float) -> None:
         """
         Method for smoothing the spectrum with a Gaussian kernel to the
         instrument resolution. The method is best applied on an input
         spectrum with a logarithmic wavelength sampling (i.e. constant
         spectral resolution). Alternatively, the wavelength sampling
@@ -362,14 +363,16 @@
         self.parameters = None
         self.samples = None
         self.ln_prob = None
         self.ln_evidence = None
         self.prob_sample = None
         self.median_sample = None
         self.attributes = None
+        self.uniform_priors = None
+        self.normal_priors = None
 
 
 class SpectrumBox(Box):
     """
     Class for storing spectral data in a
     :class:`~species.core.box.Box`.
     """
@@ -502,14 +505,16 @@
         box.flux = kwargs["flux"]
         box.parameters = kwargs["parameters"]
         box.quantity = kwargs["quantity"]
         if "contribution" in kwargs:
             box.contribution = kwargs["contribution"]
         if "bol_flux" in kwargs:
             box.bol_flux = kwargs["bol_flux"]
+        if "spec_res" in kwargs:
+            box.spec_res = kwargs["spec_res"]
 
     elif boxtype == "object":
         box = ObjectBox()
         box.name = kwargs["name"]
         box.filters = kwargs["filters"]
         box.mean_wavel = kwargs["mean_wavel"]
         box.magnitude = kwargs["magnitude"]
@@ -551,14 +556,18 @@
         box.parameters = kwargs["parameters"]
         box.samples = kwargs["samples"]
         box.ln_prob = kwargs["ln_prob"]
         box.ln_evidence = kwargs["ln_evidence"]
         box.prob_sample = kwargs["prob_sample"]
         box.median_sample = kwargs["median_sample"]
         box.attributes = kwargs["attributes"]
+        if "uniform_priors" in kwargs:
+            box.uniform_priors = kwargs["uniform_priors"]
+        if "normal_priors" in kwargs:
+            box.normal_priors = kwargs["normal_priors"]
 
     elif boxtype == "spectrum":
         box = SpectrumBox()
         box.spectrum = kwargs["spectrum"]
         box.wavelength = kwargs["wavelength"]
         box.flux = kwargs["flux"]
         if "error" in kwargs:
```

### Comparing `species-0.8.0/species/core/constants.py` & `species-0.8.1/species/core/constants.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/core/species_init.py` & `species-0.8.1/species/core/species_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,19 +70,16 @@
 
                 file_obj.write("; File with the HDF5 database\n")
                 file_obj.write("database = species_database.hdf5\n\n")
 
                 file_obj.write("; Folder where data will be downloaded\n")
                 file_obj.write("data_folder = ./data/\n\n")
 
-                # file_obj.write("; Method for the grid interpolation\n")
-                # file_obj.write(
-                #     "; Options: linear, nearest, slinear, " "cubic, quintic, pchip\n"
-                # )
-                # file_obj.write("interp_method = linear\n")
+                file_obj.write("; Magnitude of Vega for all filters\n")
+                file_obj.write("vega_mag = 0.03\n")
 
             print(" [DONE]")
 
         config = ConfigParser()
         config.read(config_file)
 
         if "database" in config["species"]:
```

### Comparing `species-0.8.0/species/data/companion_data/companion_spectra.py` & `species-0.8.1/species/data/companion_data/companion_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/database.py` & `species-0.8.1/species/data/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 # import urllib.error
 import warnings
 
 from configparser import ConfigParser
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+import astropy.units as u
 import h5py
 import numpy as np
+import pooch
 
+from astropy.coordinates import SkyCoord
 from astropy.io import fits
-
-# from astroquery.simbad import Simbad
+from astropy.units.quantity import Quantity
 from scipy.integrate import simps
 from tqdm.auto import tqdm
 from typeguard import typechecked
 
 from species.core import constants
 from species.core.box import ObjectBox, ModelBox, SamplesBox, SpectrumBox, create_box
 from species.util.core_util import print_section
@@ -196,15 +198,15 @@
 
             else:
                 print(planet_name)
 
         return comp_names
 
     @typechecked
-    def available_models(self, verbose: bool = False) -> Dict:
+    def available_models(self, verbose: bool = True) -> Dict:
         """
         Function for printing an overview of the available model grids
         that can be downloaded and added to the database with
         :class:`~species.data.database.Database.add_model`.
 
         Parameters
         ----------
@@ -827,27 +829,34 @@
         parallax: Optional[Tuple[float, float]] = None,
         distance: Optional[Tuple[float, float]] = None,
         app_mag: Optional[
             Dict[str, Union[Tuple[float, float], List[Tuple[float, float]]]]
         ] = None,
         flux_density: Optional[Dict[str, Tuple[float, float]]] = None,
         spectrum: Optional[
-            Dict[str, Tuple[str, Optional[str], Optional[float]]]
+            Dict[
+                str,
+                Tuple[
+                    Union[str, np.ndarray],
+                    Optional[Union[str, np.ndarray]],
+                    Optional[float],
+                ],
+            ]
         ] = None,
         deredden: Optional[Union[Dict[str, float], float]] = None,
         verbose: bool = True,
         units: Optional[Dict[str, Union[str, Tuple[str, str]]]] = None,
     ) -> None:
         """
         Function for adding the photometry and/or spectra
         of an object to the database.
 
         Parameters
         ----------
-        object_name: str
+        object_name : str
             Object name that will be used as label in the database.
         parallax : tuple(float, float), None
             Parallax and uncertainty (mas). Not stored if the argument
             is set to ``None``.
         distance : tuple(float, float), None
             Distance and uncertainty (pc). Not stored if the argument
             is set to ``None``. This parameter is deprecated and will
@@ -873,28 +882,32 @@
             ``flux_density`` can be used in case the magnitudes and/or
             filter profiles are not available. In that case, the fluxes
             can still be selected with ``inc_phot`` in
             :class:`~species.fit.fit_model.FitModel`. The argument
             of ``flux_density`` is ignored if set to ``None``.
         spectrum : dict, None
             Dictionary with the spectrum, optional covariance matrix,
-            and spectral resolution for each instrument. The input data
-            can either have a FITS or ASCII format. The spectra should
-            have 3 columns with wavelength (um), flux (W m-2 um-1), and
-            uncertainty (W m-2 um-1), or setting the ``units``
-            parameter allows for reading in data with different
-            wavelength and/or flux units. The covariance matrix should
-            be 2D with the same number of wavelength points as the
-            spectrum. For example, ``{'SPHERE': ('spectrum.dat',
-            'covariance.fits', 50.)}``. No covariance data is stored
-            if set to ``None``, for example, ``{'SPHERE':
-            ('spectrum.dat', None, 50.)}``. The ``spectrum`` parameter
-            is ignored if set to ``None``. For GRAVITY data, the same
-            FITS file can be provided as spectrum and covariance
-            matrix.
+            and resolving power of the instrument. The input data
+            can either be a FITS or ASCII file, or as NumPy array
+            directly. The spectra should have 3 columns, so the array
+            shape should be (n_wavelengths, 3), with wavelength (um),
+            flux (W m-2 um-1), and uncertainty (W m-2 um-1). The
+            ``units`` parameter can be set for reading in data with
+            different wavelength and/or flux units. The covariance
+            matrix should be 2D with the same number of wavelength
+            points as the spectrum, so the shape is (n_wavelengths,
+            n_wavelengths). Like the spectrum, the covariance matrix
+            can be provided as FITS or ASCII file, or as NumPy array
+            directly. For example, when providing the input as files,
+            ``{'SPHERE': ('spectrum.dat', 'covariance.fits', 50.)}``.
+            No covariance data is stored if set to ``None``, for
+            example, ``{'SPHERE': ('spectrum.dat', None, 50.)}``. The
+            ``spectrum`` parameter is ignored if set to ``None``.
+            For VLTI/GRAVITY data, the same FITS file can be provided
+            as spectrum and covariance matrix.
         deredden : dict, float, None
             Dictionary with ``spectrum`` and ``app_mag`` names that
             will be dereddened with the provided :math:`A_V`. For
             example, ``deredden={'SPHERE': 1.5, 'Keck/NIRC2.J': 1.5}``
             will deredden the provided spectrum named 'SPHERE' and
             the Keck/NIRC2 J-band photometry with a visual extinction
             of 1.5. For photometric fluxes, the filter-averaged
@@ -1222,15 +1235,17 @@
                         ]
                     )
 
                     if flux_item in units:
                         from species.util.data_util import convert_units
 
                         flux_in = np.array([[mean_wavel, data[2], data[3]]])
-                        flux_out = convert_units(flux_in, ("um", units[flux_item]))
+                        flux_out = convert_units(
+                            flux_in, ("um", units[flux_item]), convert_from=True
+                        )
 
                         data = [np.nan, np.nan, flux_out[0, 1], flux_out[0, 2]]
 
                     if verbose:
                         print(f"   - {flux_item}:")
                         print(f"      - Mean wavelength (um) = {mean_wavel:.4e}")
                         print(
@@ -1255,89 +1270,105 @@
 
             spec_nan = {}
 
             for spec_item, spec_value in spectrum.items():
                 if f"objects/{object_name}/spectrum/{spec_item}" in hdf5_file:
                     del hdf5_file[f"objects/{object_name}/spectrum/{spec_item}"]
 
-                if spec_value[0].endswith(".fits") or spec_value[0].endswith(".fit"):
-                    with fits.open(spec_value[0]) as hdulist:
-                        if (
-                            "INSTRU" in hdulist[0].header
-                            and hdulist[0].header["INSTRU"] == "GRAVITY"
-                        ):
-                            # Read data from a FITS file with the GRAVITY format
-                            gravity_object = hdulist[0].header["OBJECT"]
-
-                            if verbose:
-                                print("   - GRAVITY spectrum:")
-                                print(f"      - Object: {gravity_object}")
-
-                            wavelength = hdulist[1].data["WAVELENGTH"]  # (um)
-                            flux = hdulist[1].data["FLUX"]  # (W m-2 um-1)
-                            covariance = hdulist[1].data["COVARIANCE"]  # (W m-2 um-1)^2
-                            error = np.sqrt(np.diag(covariance))  # (W m-2 um-1)
-
-                            read_spec[spec_item] = np.column_stack(
-                                [wavelength, flux, error]
-                            )
+                if isinstance(spec_value[0], str):
+                    if spec_value[0].endswith(".fits") or spec_value[0].endswith(
+                        ".fit"
+                    ):
+                        with fits.open(spec_value[0]) as hdulist:
+                            if (
+                                "INSTRU" in hdulist[0].header
+                                and hdulist[0].header["INSTRU"] == "GRAVITY"
+                            ):
+                                # Read data from a FITS file with the GRAVITY format
+                                gravity_object = hdulist[0].header["OBJECT"]
+
+                                if verbose:
+                                    print("   - GRAVITY spectrum:")
+                                    print(f"      - Object: {gravity_object}")
+
+                                wavelength = hdulist[1].data["WAVELENGTH"]  # (um)
+                                flux = hdulist[1].data["FLUX"]  # (W m-2 um-1)
+                                covariance = hdulist[1].data[
+                                    "COVARIANCE"
+                                ]  # (W m-2 um-1)^2
+                                error = np.sqrt(np.diag(covariance))  # (W m-2 um-1)
 
-                        else:
-                            # Otherwise try to read a 2D dataset with 3 columns
-                            if verbose:
-                                print("   - Spectrum:")
-
-                            for i, hdu_item in enumerate(hdulist):
-                                data = np.asarray(hdu_item.data)
-
-                                if (
-                                    data.ndim == 2
-                                    and 3 in data.shape
-                                    and spec_item not in read_spec
-                                ):
-                                    if spec_item in units:
-                                        from species.util.data_util import convert_units
-
-                                        data = convert_units(data, units[spec_item])
-
-                                    read_spec[spec_item] = data
-
-                            if spec_item not in read_spec:
-                                raise ValueError(
-                                    f"The spectrum data from {spec_value[0]} can not "
-                                    f"be read. The data format should be 2D with "
-                                    f"3 columns."
+                                read_spec[spec_item] = np.column_stack(
+                                    [wavelength, flux, error]
                                 )
 
-                else:
-                    try:
-                        data = np.loadtxt(spec_value[0])
+                            else:
+                                # Otherwise try to read a 2D dataset with 3 columns
+                                if verbose:
+                                    print("   - Spectrum:")
+
+                                for i, hdu_item in enumerate(hdulist):
+                                    data = np.asarray(hdu_item.data)
+
+                                    if (
+                                        data.ndim == 2
+                                        and 3 in data.shape
+                                        and spec_item not in read_spec
+                                    ):
+                                        if spec_item in units:
+                                            from species.util.data_util import (
+                                                convert_units,
+                                            )
+
+                                            data = convert_units(
+                                                data,
+                                                units[spec_item],
+                                                convert_from=True,
+                                            )
+
+                                        read_spec[spec_item] = data
+
+                                if spec_item not in read_spec:
+                                    raise ValueError(
+                                        f"The spectrum data from {spec_value[0]} can not "
+                                        f"be read. The data format should be 2D with "
+                                        f"3 columns."
+                                    )
 
-                    except UnicodeDecodeError:
-                        raise ValueError(
-                            f"The spectrum data from {spec_value[0]} can not "
-                            "be read. Please provide a FITS or ASCII file."
-                        )
+                    else:
+                        try:
+                            data = np.loadtxt(spec_value[0])
 
-                    if data.ndim != 2 or 3 not in data.shape:
-                        raise ValueError(
-                            f"The spectrum data from {spec_value[0]} "
-                            "can not be read. The data format "
-                            "should be 2D with 3 columns."
-                        )
+                        except UnicodeDecodeError:
+                            raise ValueError(
+                                f"The spectrum data from {spec_value[0]} can not "
+                                "be read. Please provide a FITS or ASCII file."
+                            )
 
-                    if verbose:
-                        print("   - Spectrum:")
+                        if data.ndim != 2 or 3 not in data.shape:
+                            raise ValueError(
+                                f"The spectrum data from {spec_value[0]} "
+                                "can not be read. The data format "
+                                "should be 2D with 3 columns."
+                            )
 
-                    if spec_item in units:
-                        from species.util.data_util import convert_units
+                        if verbose:
+                            print("   - Spectrum:")
+
+                        if spec_item in units:
+                            from species.util.data_util import convert_units
+
+                            data = convert_units(
+                                data, units[spec_item], convert_from=True
+                            )
 
-                        data = convert_units(data, units[spec_item])
+                        read_spec[spec_item] = data
 
-                    read_spec[spec_item] = data
+                else:
+                    read_spec[spec_item] = spec_value[0]
 
                 if isinstance(deredden, float):
                     from species.util.dust_util import ism_extinction
 
                     ext_mag = ism_extinction(deredden, 3.1, read_spec[spec_item][:, 0])
                     read_spec[spec_item][:, 1] *= 10.0 ** (0.4 * ext_mag)
 
@@ -1378,15 +1409,16 @@
 
                 wavelength = read_spec[spec_item][:, 0]
                 flux = read_spec[spec_item][:, 1]
                 error = read_spec[spec_item][:, 2]
 
                 if verbose:
                     print(f"      - Database tag: {spec_item}")
-                    print(f"      - Filename: {spec_value[0]}")
+                    if isinstance(spec_value[0], str):
+                        print(f"      - Filename: {spec_value[0]}")
                     print(f"      - Data shape: {read_spec[spec_item].shape}")
                     print(
                         f"      - Wavelength range (um): {wavelength[0]:.2f} - {wavelength[-1]:.2f}"
                     )
                     print(f"      - Mean flux (W m-2 um-1): {np.nanmean(flux):.2e}")
                     print(f"      - Mean error (W m-2 um-1): {np.nanmean(error):.2e}")
 
@@ -1398,135 +1430,140 @@
 
             # Read covariance matrix
 
             for spec_item, spec_value in spectrum.items():
                 if spec_value[1] is None:
                     read_cov[spec_item] = None
 
-                elif spec_value[1].endswith(".fits") or spec_value[1].endswith(".fit"):
-                    with fits.open(spec_value[1]) as hdulist:
-                        if (
-                            "INSTRU" in hdulist[0].header
-                            and hdulist[0].header["INSTRU"] == "GRAVITY"
-                        ):
-                            # Read data from a FITS file with the GRAVITY format
-                            gravity_object = hdulist[0].header["OBJECT"]
-
-                            if verbose:
-                                print("   - GRAVITY covariance matrix:")
-                                print(f"      - Object: {gravity_object}")
-
-                            read_cov[spec_item] = hdulist[1].data[
-                                "COVARIANCE"
-                            ]  # (W m-2 um-1)^2
-
-                        else:
-                            if spec_item in units:
-                                warnings.warn(
-                                    "The unit conversion has not been "
-                                    "implemented for covariance matrices. "
-                                    "Please open an issue on the Github "
-                                    "page if such functionality is required "
-                                    "or provide the file with covariances "
-                                    "in (W m-2 um-1)^2."
-                                )
+                elif isinstance(spec_value[1], str):
+                    if spec_value[1].endswith(".fits") or spec_value[1].endswith(".fit"):
+                        with fits.open(spec_value[1]) as hdulist:
+                            if (
+                                "INSTRU" in hdulist[0].header
+                                and hdulist[0].header["INSTRU"] == "GRAVITY"
+                            ):
+                                # Read data from a FITS file with the GRAVITY format
+                                gravity_object = hdulist[0].header["OBJECT"]
+
+                                if verbose:
+                                    print("   - GRAVITY covariance matrix:")
+                                    print(f"      - Object: {gravity_object}")
+
+                                read_cov[spec_item] = hdulist[1].data[
+                                    "COVARIANCE"
+                                ]  # (W m-2 um-1)^2
+
+                            else:
+                                if spec_item in units:
+                                    warnings.warn(
+                                        "The unit conversion has not been "
+                                        "implemented for covariance matrices. "
+                                        "Please open an issue on the Github "
+                                        "page if such functionality is required "
+                                        "or provide the file with covariances "
+                                        "in (W m-2 um-1)^2."
+                                    )
+
+                                # Otherwise try to read a square, 2D dataset
+                                if verbose:
+                                    print("   - Covariance matrix:")
+
+                                for i, hdu_item in enumerate(hdulist):
+                                    data = np.asarray(hdu_item.data)
+
+                                    corr_warn = (
+                                        f"The matrix from {spec_value[1]} contains "
+                                        f"ones along the diagonal. Converting this "
+                                        f"correlation matrix into a covariance matrix."
+                                    )
+
+                                    from species.util.data_util import (
+                                        correlation_to_covariance,
+                                    )
+
+                                    if data.ndim == 2 and data.shape[0] == data.shape[1]:
+                                        if spec_item not in read_cov:
+                                            if (
+                                                data.shape[0]
+                                                == read_spec[spec_item].shape[0]
+                                            ):
+                                                if np.all(np.diag(data) == 1.0):
+                                                    warnings.warn(corr_warn)
+
+                                                    read_cov[
+                                                        spec_item
+                                                    ] = correlation_to_covariance(
+                                                        data, read_spec[spec_item][:, 2]
+                                                    )
+
+                                                else:
+                                                    read_cov[spec_item] = data
+
+                                if spec_item not in read_cov:
+                                    raise ValueError(
+                                        f"The covariance matrix from {spec_value[1]} can not "
+                                        f"be read. The data format should be 2D with the "
+                                        f"same number of wavelength points as the "
+                                        f"spectrum."
+                                    )
 
-                            # Otherwise try to read a square, 2D dataset
-                            if verbose:
-                                print("   - Covariance matrix:")
-
-                            for i, hdu_item in enumerate(hdulist):
-                                data = np.asarray(hdu_item.data)
-
-                                corr_warn = (
-                                    f"The matrix from {spec_value[1]} contains "
-                                    f"ones along the diagonal. Converting this "
-                                    f"correlation matrix into a covariance matrix."
-                                )
-
-                                from species.util.data_util import (
-                                    correlation_to_covariance,
-                                )
-
-                                if data.ndim == 2 and data.shape[0] == data.shape[1]:
-                                    if spec_item not in read_cov:
-                                        if (
-                                            data.shape[0]
-                                            == read_spec[spec_item].shape[0]
-                                        ):
-                                            if np.all(np.diag(data) == 1.0):
-                                                warnings.warn(corr_warn)
-
-                                                read_cov[
-                                                    spec_item
-                                                ] = correlation_to_covariance(
-                                                    data, read_spec[spec_item][:, 2]
-                                                )
-
-                                            else:
-                                                read_cov[spec_item] = data
-
-                            if spec_item not in read_cov:
-                                raise ValueError(
-                                    f"The covariance matrix from {spec_value[1]} can not "
-                                    f"be read. The data format should be 2D with the "
-                                    f"same number of wavelength points as the "
-                                    f"spectrum."
-                                )
+                    else:
+                        try:
+                            data = np.loadtxt(spec_value[1])
+                        except UnicodeDecodeError:
+                            raise ValueError(
+                                f"The covariance matrix from {spec_value[1]} "
+                                f"can not be read. Please provide a "
+                                f"FITS or ASCII file."
+                            )
 
-                else:
-                    try:
-                        data = np.loadtxt(spec_value[1])
-                    except UnicodeDecodeError:
-                        raise ValueError(
-                            f"The covariance matrix from {spec_value[1]} "
-                            f"can not be read. Please provide a "
-                            f"FITS or ASCII file."
-                        )
+                        if data.ndim != 2 or data.shape[0] != data.shape[1]:
+                            raise ValueError(
+                                f"The covariance matrix from {spec_value[1]} "
+                                f"can not be read. The data format "
+                                f"should be 2D with the same number of "
+                                f"wavelength points as the spectrum."
+                            )
 
-                    if data.ndim != 2 or data.shape[0] != data.shape[1]:
-                        raise ValueError(
-                            f"The covariance matrix from {spec_value[1]} "
-                            f"can not be read. The data format "
-                            f"should be 2D with the same number of "
-                            f"wavelength points as the spectrum."
-                        )
+                        if verbose:
+                            print("   - Covariance matrix:")
 
-                    if verbose:
-                        print("   - Covariance matrix:")
+                        if np.all(np.diag(data) == 1.0):
+                            warnings.warn(
+                                f"The matrix from {spec_value[1]} contains "
+                                f"ones on the diagonal. Converting this "
+                                f" correlation matrix into a covariance "
+                                f"matrix."
+                            )
 
-                    if np.all(np.diag(data) == 1.0):
-                        warnings.warn(
-                            f"The matrix from {spec_value[1]} contains "
-                            f"ones on the diagonal. Converting this "
-                            f" correlation matrix into a covariance "
-                            f"matrix."
-                        )
+                            from species.util.data_util import correlation_to_covariance
 
-                        from species.util.data_util import correlation_to_covariance
+                            read_cov[spec_item] = correlation_to_covariance(
+                                data, read_spec[spec_item][:, 2]
+                            )
 
-                        read_cov[spec_item] = correlation_to_covariance(
-                            data, read_spec[spec_item][:, 2]
-                        )
+                        else:
+                            read_cov[spec_item] = data
 
-                    else:
-                        read_cov[spec_item] = data
+                else:
+                    read_cov[spec_item] = spec_value[1]
 
                 if read_cov[spec_item] is not None:
                     # Remove the wavelengths for which the flux is NaN
                     read_cov[spec_item] = read_cov[spec_item][~spec_nan[spec_item], :]
                     read_cov[spec_item] = read_cov[spec_item][:, ~spec_nan[spec_item]]
 
                 if verbose and read_cov[spec_item] is not None:
                     print(f"      - Database tag: {spec_item}")
-                    print(f"      - Filename: {spec_value[1]}")
+                    if isinstance(spec_value[1], str):
+                        print(f"      - Filename: {spec_value[1]}")
                     print(f"      - Data shape: {read_cov[spec_item].shape}")
 
             if verbose:
-                print("   - Resolution:")
+                print("   - Instrument resolution:")
 
             for spec_item, spec_value in spectrum.items():
                 hdf5_file.create_dataset(
                     f"objects/{object_name}/spectrum/{spec_item}/spectrum",
                     data=read_spec[spec_item],
                 )
 
@@ -1552,14 +1589,301 @@
                     if verbose:
                         print(f"      - {spec_item}: {spec_value[2]:.1f}")
                     dset.attrs["specres"] = spec_value[2]
 
         hdf5_file.close()
 
     @typechecked
+    def add_simple_object(
+        self,
+        object_name: str,
+        simple_database: Optional[str] = None,
+    ) -> None:
+        """
+        Function for retrieving data of an individual object from
+        the `SIMPLE database <https://simple-bd-archive.org>`_ and
+        adding the data to the ``species`` database. This function
+        includes code that has been adapted from `SEDkitSIMPLE
+        <https://github.com/dr-rodriguez/SEDkitSIMPLE>`_.
+
+        Parameters
+        ----------
+        object_name : str
+            Object name that will be used for the query and also used
+            as label by which the data will be stored in the database.
+        simple_database : str, None
+            Path to the ``SIMPLE`` database file `SIMPLE.db`. The
+            binary file is automatically  downloaded from the `Github
+            page <https://github.com/SIMPLE-AstroDB/SIMPLE-binary>`_
+            of ``SIMPLE`` when the argument is set to ``None``.
+
+        Returns
+        -------
+        NoneType
+            None
+        """
+
+        print_section("Add SIMPLE object")
+
+        from astrodbkit2.astrodb import Database as astro_db
+        from sqlalchemy import and_
+
+        if simple_database is None:
+            simple_database = os.path.join(self.data_folder, "SIMPLE.db")
+            url = (
+                "https://github.com/SIMPLE-AstroDB/" "SIMPLE-binary/raw/main/SIMPLE.db"
+            )
+
+            if not os.path.isfile(simple_database):
+                pooch.retrieve(
+                    url=url,
+                    known_hash=None,
+                    fname="SIMPLE.db",
+                    path=self.data_folder,
+                    progressbar=True,
+                )
+
+        print(f"SIMPLE database: {simple_database}")
+
+        simple_db = astro_db(f"sqlite:///{simple_database}")
+
+        def _fetch_bibcode(ref: str) -> Optional[str]:
+            """
+            Internal function for fetching a reference
+            from the SIMPLE database
+
+            Parameters
+            ----------
+            ref : str
+                Reference for which the `bibcode` should be retrieved.
+
+            Returns
+            -------
+            NoneType
+                Bibcode of the reference. Returns a ``None`` in
+                case the bibcode is not available.
+            """
+
+            bibcode = None
+
+            if hasattr(simple_db.Publications.c, "bibcode"):
+                if hasattr(simple_db.Publications.c, "reference"):
+                    simple_query = simple_db.query(simple_db.Publications.c.bibcode)
+
+                    simple_result = simple_query.filter(
+                        simple_db.Publications.c.reference == ref
+                    )
+
+                    bibcode = simple_result.table()["bibcode"][0]
+
+            return bibcode
+
+        # Get SIMPLE name of object
+
+        print(f"\nObject name: {object_name}")
+
+        sources = simple_db.search_object(object_name)
+
+        if len(sources) > 0:
+            if len(sources) > 1:
+                warnings.warn(
+                    "Multiple sources found in the SIMPLE "
+                    f"database for {object_name}. The first "
+                    "retrieved source will be selected."
+                )
+
+            simple_id = sources["source"][0]
+
+        else:
+            raise ValueError(
+                f"The requested source, {object_name}, is "
+                "not found in the SIMPLE database."
+            )
+
+        print(f"Retrieved name: {simple_id}")
+
+        # Get inventory of the queried object
+
+        inventory = simple_db.inventory(simple_id, pretty_print=False)
+
+        # Get coordinates
+
+        coordinates = None
+
+        if "Sources" in inventory:
+            if len(inventory["Sources"]) == 1:
+                data = inventory["Sources"][0]
+                coordinates = SkyCoord(ra=data["ra"] * u.deg, dec=data["dec"] * u.deg)
+
+        if coordinates is None:
+            print("Coordinates: None")
+
+        else:
+            coord_str = coordinates.to_string(
+                "hmsdms", alwayssign=True, precision=2, pad=True
+            )
+            print(f"Coordinates: {coord_str}")
+
+        # Get parallax
+
+        parallax = None
+
+        if "Parallaxes" in inventory:
+            for row in inventory["Parallaxes"]:
+                value = Quantity(row["parallax"], unit=u.mas)
+                error = Quantity(row["parallax_error"], unit=u.mas)
+                bibcode = _fetch_bibcode(row["reference"])
+                parallax = (value.value, error.value)
+
+                if row["adopted"]:
+                    break
+
+        if parallax is None:
+            print("Parallax: None")
+
+        else:
+            print(
+                f"Parallax: {(parallax)[0]:.2f} +/- "
+                f"{(parallax)[1]:.2f} mas (bibcode: {bibcode})"
+            )
+
+        # Get spectral type
+
+        spectral_type = None
+
+        if "SpectralTypes" in inventory:
+            for row in inventory["SpectralTypes"]:
+                bibcode = _fetch_bibcode(row["reference"])
+                spectral_type = row["spectral_type_string"]
+
+                if row["adopted"]:
+                    break
+
+        if spectral_type is None:
+            print("Spectral type: None")
+
+        else:
+            print(f"Spectral type: {spectral_type} (bibcode: {bibcode})")
+
+        # Get photometry
+
+        app_mag = None
+
+        if "Photometry" in inventory:
+            app_mag = {}
+            bibcode = {}
+
+            for row in inventory["Photometry"]:
+                filter_name = None
+
+                if row["band"].split(".")[0] == "GAIA3":
+                    filter_name = "GAIA/" + row["band"]
+                elif row["band"].split(".")[0] == "2MASS":
+                    filter_name = "2MASS/" + row["band"]
+                elif row["band"].split(".")[0] == "WISE":
+                    filter_name = "WISE/" + row["band"]
+                elif row["band"].split(".")[0] == "WISE":
+                    filter_name = "WISE/" + row["band"]
+
+                if filter_name is not None and row["magnitude_error"] is not None:
+                    bibcode[filter_name] = _fetch_bibcode(row["reference"])
+                    app_mag[filter_name] = (row["magnitude"], row["magnitude_error"])
+
+        if app_mag is None:
+            print("Magnitudes: None")
+
+        else:
+            print("\nMagnitudes:")
+            for key, value in app_mag.items():
+                if value[1] > 1e-2:
+                    print(
+                        f"   - {key} = {value[0]:.2f} +/- {value[1]:.2f} (bibcode: {bibcode[key]})"
+                    )
+                elif value[1] < 1e-2 and value[1] > 1e-3:
+                    print(
+                        f"   - {key} = {value[0]:.3f} +/- {value[1]:.3f} (bibcode: {bibcode[key]})"
+                    )
+                elif value[1] < 1e-3 and value[1] > 1e-4:
+                    print(
+                        f"   - {key} = {value[0]:.4f} +/- {value[1]:.4f} (bibcode: {bibcode[key]})"
+                    )
+                else:
+                    print(
+                        f"   - {key} = {value[0]:.5f} +/- {value[1]:.5f} (bibcode: {bibcode[key]})"
+                    )
+
+        # Get spectra
+
+        spectrum = None
+
+        if "Spectra" in inventory:
+            spectrum = {}
+            bibcode = {}
+
+            for row in inventory["Spectra"]:
+                spec_tag = f"{row['telescope']} {row['instrument']}"
+                if row["mode"] != "Missing":
+                    spec_tag += f" {row['mode']}"
+
+                simple_query = simple_db.query(simple_db.Spectra)
+
+                spec_table = simple_query.filter(
+                    and_(
+                        simple_db.Spectra.c.source == simple_id,
+                        simple_db.Spectra.c.regime == row["regime"],
+                        simple_db.Spectra.c.reference == row["reference"],
+                        simple_db.Spectra.c.observation_date == row["observation_date"],
+                    )
+                ).astropy(spectra="spectrum", spectra_format=None)
+
+                wavel = spec_table["spectrum"][0].wavelength
+                flux = spec_table["spectrum"][0].flux
+
+                wavel = wavel.to(u.micron).value
+                flux = flux.to(u.W / u.m**2 / u.um).value
+
+                if spec_table["spectrum"][0].uncertainty is not None:
+                    error = spec_table["spectrum"][0].uncertainty.quantity
+                    error = error.to(u.W / u.m**2 / u.um).value
+                else:
+                    error = np.full(wavel.size, np.nan)
+
+                spec_data = np.column_stack([wavel, flux, error])
+
+                spec_res = input(
+                    "Please provide the resolving power, "
+                    f"R = lambda/Delta_lambda, for '{spec_tag}': "
+                )
+
+                bibcode[spec_tag] = _fetch_bibcode(row["reference"])
+                spectrum[spec_tag] = (spec_data, np.diag(spec_data[:, 2]**2), float(spec_res))
+
+        if spectrum is None:
+            if app_mag is not None:
+                print()
+
+            print("Spectra: None")
+
+        else:
+            print("\nSpectra:")
+            for key, value in spectrum.items():
+                print(f"   - {key}")
+                print(f"      - Array shape: {value[0].shape}")
+                print(f"      - lambda/d_lambda: {value[2]}")
+                print(f"      - bibcode: {bibcode[key]}")
+
+        self.add_object(
+            object_name=object_name,
+            parallax=parallax,
+            app_mag=app_mag,
+            spectrum=spectrum,
+            verbose=False,
+        )
+
+    @typechecked
     def add_photometry(self, phot_library: str) -> None:
         """
         Parameters
         ----------
         phot_library : str
             Photometric library ('vlm-plx' or 'leggett').
 
@@ -2830,14 +3154,17 @@
                 param.append(dset.attrs[f"parameter{i}"])
                 print(f"   - {param[-1]}")
 
             # Printing uniform and normal priors
             # Check if attributes are present for
             # backward compatibility
 
+            uniform_priors = {}
+            normal_priors = {}
+
             if "n_bounds" in attributes and attributes["n_bounds"] > 0:
                 dset_bounds = hdf5_file[f"results/fit/{tag}/bounds"]
                 print("\nUniform priors (min, max):")
 
                 for bound_item in dset_bounds:
                     group_path = f"results/fit/{tag}/bounds/{bound_item}"
 
@@ -2847,31 +3174,38 @@
                             # of the photometric fluxes. Since the SVO
                             # filter names contain a slash which introduces
                             # a subgroup in the HDF5 database
                             prior_bound = np.array(
                                 hdf5_file[f"{group_path}/{filter_item}"]
                             )
                             print(
-                                f"   - {bound_item}/{filter_item} = ({prior_bound[0]}, {prior_bound[1]})"
+                                f"   - {bound_item}/{filter_item} = "
+                                f"({prior_bound[0]}, {prior_bound[1]})"
+                            )
+                            uniform_priors[f"{bound_item}/{filter_item}"] = (
+                                prior_bound[0],
+                                prior_bound[1],
                             )
 
                     else:
                         prior_bound = np.array(hdf5_file[group_path])
                         print(
                             f"   - {bound_item} = ({prior_bound[0]}, {prior_bound[1]})"
                         )
+                        uniform_priors[bound_item] = (prior_bound[0], prior_bound[1])
 
             if "n_normal_prior" in attributes and attributes["n_normal_prior"] > 0:
                 dset_prior = hdf5_file[f"results/fit/{tag}/normal_prior"]
                 print("\nNormal priors (mean, sigma):")
 
                 for prior_item in dset_prior:
                     group_path = f"results/fit/{tag}/normal_prior/{prior_item}"
                     norm_prior = np.array(hdf5_file[group_path])
                     print(f"   - {prior_item} = ({norm_prior[0]}, {norm_prior[1]})")
+                    normal_priors[prior_item] = (norm_prior[0], norm_prior[1])
 
         median_sample = self.get_median_sample(tag, burnin, verbose=False)
         prob_sample = self.get_probable_sample(tag, burnin, verbose=False)
 
         if json_file is not None:
             samples_dict = {}
 
@@ -2889,14 +3223,16 @@
             parameters=param,
             samples=samples,
             ln_prob=ln_prob,
             ln_evidence=ln_evidence,
             prob_sample=prob_sample,
             median_sample=median_sample,
             attributes=attributes,
+            uniform_priors=uniform_priors,
+            normal_priors=normal_priors,
         )
 
     @typechecked
     def get_evidence(self, tag: str) -> Tuple[float, float]:
         """
         Function for returning the log-evidence (i.e.
         marginalized likelihood) that was computed by
```

### Comparing `species-0.8.0/species/data/filter_data/filter_data.py` & `species-0.8.1/species/data/filter_data/filter_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/add_isochrone.py` & `species-0.8.1/species/data/isochrone_data/add_isochrone.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_ames.py` & `species-0.8.1/species/data/isochrone_data/iso_ames.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_atmo.py` & `species-0.8.1/species/data/isochrone_data/iso_atmo.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_baraffe2015.py` & `species-0.8.1/species/data/isochrone_data/iso_baraffe2015.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_btsettl.py` & `species-0.8.1/species/data/isochrone_data/iso_btsettl.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_linder2019.py` & `species-0.8.1/species/data/isochrone_data/iso_linder2019.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_manual.py` & `species-0.8.1/species/data/isochrone_data/iso_manual.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_marleau.py` & `species-0.8.1/species/data/isochrone_data/iso_marleau.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_nextgen.py` & `species-0.8.1/species/data/isochrone_data/iso_nextgen.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_saumon2008.py` & `species-0.8.1/species/data/isochrone_data/iso_saumon2008.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/isochrone_data/iso_sonora.py` & `species-0.8.1/species/data/isochrone_data/iso_sonora.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/misc_data/accretion_data.py` & `species-0.8.1/species/data/misc_data/accretion_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/misc_data/dust_data.py` & `species-0.8.1/species/data/misc_data/dust_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,17 @@
     if not os.path.exists(input_path):
         os.makedirs(input_path)
 
     url = "https://home.strw.leidenuniv.nl/~stolker/species/lognorm_mgsio3_c_ext.fits"
 
     data_file = os.path.join(input_path, "lognorm_mgsio3_c_ext.fits")
 
-    print("\nDownloading log-normal dust cross sections (231 kB)...", end="", flush=True)
+    print(
+        "\nDownloading log-normal dust cross sections (231 kB)...", end="", flush=True
+    )
     urllib.request.urlretrieve(url, data_file)
     print(" [DONE]")
 
     print("\nAdding log-normal dust cross sections:")
 
     with fits.open(os.path.join(input_path, "lognorm_mgsio3_c_ext.fits")) as hdu_list:
         database.create_dataset(
```

### Comparing `species-0.8.0/species/data/model_data/custom_model.py` & `species-0.8.1/species/data/model_data/custom_model.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/model_data/model_spectra.py` & `species-0.8.1/species/data/model_data/model_spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,22 +116,31 @@
             "The Exo-Rem grid has been updated to the latest version "
             "from https://lesia.obspm.fr/exorem/YGP_grids/. Please "
             "consider removing the grid from the 'data_folder' if "
             "needed such that the latest version of the grid will "
             "be downloaded and added to the HDF5 database."
         )
 
-    elif model_tag == "exo-rem-highres" and teff_range is None:
-        warnings.warn(
-            "Adding the full high-resolution grid of Exo-Rem to the "
-            "HDF5 database may not be feasible since it requires "
-            "a large amount of memory. Please consider using the "
-            "'teff_range' parameter to only add a small "
-            "Teff range of model spectra to the database."
-        )
+    elif model_tag == "exo-rem-highres":
+        if teff_range is None:
+            warnings.warn(
+                "Adding the full high-resolution grid of Exo-Rem to the "
+                "HDF5 database may not be feasible since it requires "
+                "a large amount of memory. Please consider using the "
+                "'teff_range' parameter to only add a subset of the "
+                "model spectra to the database."
+            )
+
+        if wavel_range is None:
+            warnings.warn(
+                "Adding the full high-resolution grid of Exo-Rem to the "
+                "HDF5 database may not be feasible since it requires "
+                "a large amount of memory. Please consider using the "
+                "'wavel_range' parameter to reduce the data size."
+            )
 
     if wavel_sampling is not None and wavel_range is None:
         warnings.warn(
             "The 'wavel_sampling' parameter can only be "
             "used in combination with the 'wavel_range' "
             "parameter. The model spectra are therefore "
             "not resampled."
@@ -286,17 +295,17 @@
     else:
         print(f"Teff range (K) = {teff_range[0]} - {teff_range[1]}")
 
     print()
     print_message = ""
 
     for _, _, file_list in os.walk(data_folder):
-        for filename in sorted(file_list):
-            if filename[: len(model_tag)] == model_tag:
-                file_split = filename.split("_")
+        for file_name in sorted(file_list):
+            if file_name[: len(model_tag)] == model_tag:
+                file_split = file_name.split("_")
 
                 param_index = file_split.index("teff") + 1
                 teff_val = float(file_split[param_index])
 
                 if teff_range is not None:
                     if teff_val < teff_range[0] or teff_val > teff_range[1]:
                         continue
@@ -327,21 +336,28 @@
                     param_index = file_split.index("adindex") + 1
                     ad_index.append(float(file_split[param_index]))
 
                 empty_message = len(print_message) * " "
                 print(f"\r{empty_message}", end="")
 
                 print_message = (
-                    f"Adding {model_info['name']} model spectra... {filename}"
+                    f"Adding {model_info['name']} model spectra... {file_name}"
                 )
                 print(f"\r{print_message}", end="", flush=True)
 
-                data_wavel, data_flux = np.loadtxt(
-                    os.path.join(data_folder, filename), unpack=True
-                )
+                spec_file = os.path.join(data_folder, file_name)
+
+                if file_name[-4:] == ".dat":
+                    data_wavel, data_flux = np.loadtxt(spec_file, unpack=True)
+
+                else:
+                    data = np.load(spec_file)
+
+                    data_wavel = data[:, 0]
+                    data_flux = data[:, 1]
 
                 if wavel_range is None:
                     if wavelength is None:
                         wavelength = np.copy(data_wavel)  # (um)
 
                         if np.all(np.diff(wavelength) < 0):
                             raise ValueError(
```

### Comparing `species-0.8.0/species/data/phot_data/phot_leggett.py` & `species-0.8.1/species/data/phot_data/phot_leggett.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/phot_data/phot_vlm_plx.py` & `species-0.8.1/species/data/phot_data/phot_vlm_plx.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
-Module for the photometric data and parallaxes
-from the Database of Ultracool Parallaxes.
+Module for the photometric data and parallaxes from the
+Database of Ultracool Parallaxes.
 """
 
 import os
 import urllib.request
 
 import h5py
 import numpy as np
@@ -13,16 +13,19 @@
 from astropy.io import fits
 
 from species.util.data_util import update_sptype
 
 
 def add_vlm_plx(input_path, database):
     """
-    Function for adding the Database of Ultracool
-    Parallaxes to the database.
+    Function for adding the Database of Ultracool Parallaxes to the
+    database. The FITS file with data was originally downloaded from
+    http://www.as.utexas.edu/~tdupuy/plx/Database_of_Ultracool_Parallaxes_files/vlm-plx-all.fits
+    but that website has been taken offline, probably because of the
+    new table at http://bit.ly/UltracoolSheet.
 
     Parameters
     ----------
     input_path : str
         Data folder.
     database : h5py._hl.files.File
         HDF5 database.
@@ -31,18 +34,15 @@
     -------
     NoneType
         None
     """
 
     data_file = os.path.join(input_path, "vlm-plx-all.fits")
 
-    url = (
-        "http://www.as.utexas.edu/~tdupuy/plx/"
-        "Database_of_Ultracool_Parallaxes_files/vlm-plx-all.fits"
-    )
+    url = "https://home.strw.leidenuniv.nl/~stolker/species/vlm-plx-all.fits"
 
     if not os.path.isfile(data_file):
         pooch.retrieve(
             url=url,
             known_hash="d31bb3162d7de890c09ebf9f0497d51159889b5f5e7c4da1ddf01f24d0c2b36f",
             fname="vlm-plx-all.fits",
             path=input_path,
```

### Comparing `species-0.8.0/species/data/spec_data/add_spec_data.py` & `species-0.8.1/species/data/spec_data/add_spec_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_allers2013.py` & `species-0.8.1/species/data/spec_data/spec_allers2013.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_bonnefoy2014.py` & `species-0.8.1/species/data/spec_data/spec_bonnefoy2014.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_irtf.py` & `species-0.8.1/species/data/spec_data/spec_irtf.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_kesseli2017.py` & `species-0.8.1/species/data/spec_data/spec_kesseli2017.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_spex.py` & `species-0.8.1/species/data/spec_data/spec_spex.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/data/spec_data/spec_vega.py` & `species-0.8.1/species/data/spec_data/spec_vega.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/fit/compare_spectra.py` & `species-0.8.1/species/fit/compare_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/fit/emission_line.py` & `species-0.8.1/species/fit/emission_line.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/fit/fit_evolution.py` & `species-0.8.1/species/fit/fit_evolution.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/fit/fit_model.py` & `species-0.8.1/species/fit/fit_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -667,15 +667,15 @@
                     self.bounds["spec_weight"] = (0.0, 1.0)
 
         # Select filters and spectra
 
         if isinstance(inc_phot, bool):
             if inc_phot:
                 # Select all filters if inc_phot=True
-                inc_phot = self.object.list_filters()
+                inc_phot = self.object.list_filters(verbose=False)
 
             else:
                 inc_phot = []
 
         if isinstance(inc_spec, bool):
             if inc_spec:
                 # Select all spectra if inc_spec=True
@@ -979,30 +979,30 @@
 
         for key, value in self.bounds.items():
             if value[0] == value[1] and value[0] is not None and value[1] is not None:
                 self.fix_param[key] = value[0]
                 del_param.append(key)
 
         if del_param:
-            print(f"Fixing {len(del_param)} parameters:")
+            print(f"\nFixing {len(del_param)} parameters:")
 
             for item in del_param:
                 print(f"   - {item} = {self.fix_param[item]}")
 
                 self.modelpar.remove(item)
                 del self.bounds[item]
 
         print(f"\nFitting {len(self.modelpar)} parameters:")
 
         for item in self.modelpar:
             print(f"   - {item}")
 
         # Add parallax to dictionary with Gaussian priors
 
-        if "parallax" in self.modelpar:
+        if "parallax" in self.modelpar and "parallax" not in self.fix_param:
             self.normal_prior["parallax"] = (self.parallax[0], self.parallax[1])
 
         # Printing uniform and normal priors
 
         print("\nUniform priors (min, max):")
 
         for key, value in self.bounds.items():
@@ -1246,14 +1246,16 @@
 
         # Add the parallax manually because it should
         # not be provided in the bounds dictionary
 
         if self.model != "powerlaw":
             if "parallax" in self.cube_index:
                 parallax = params[self.cube_index["parallax"]]
+            elif "parallax" in self.fix_param:
+                parallax = self.fix_param["parallax"]
             else:
                 parallax = None
 
         for item in self.fix_param:
             # Add the fixed parameters to their dictionaries
 
             if item[:8] == "scaling_" and item[8:] in self.spectrum:
@@ -2586,17 +2588,15 @@
             else:
                 if dynamic:
                     if resume:
                         dsampler = dynesty.DynamicNestedSampler.restore(
                             fname=out_basename + "dynesty.save"
                         )
 
-                        print(
-                            f"Resumed a Dynesty run from {out_basename}dynesty.save"
-                        )
+                        print(f"Resumed a Dynesty run from {out_basename}dynesty.save")
 
                     else:
                         dsampler = dynesty.DynamicNestedSampler(
                             loglikelihood=self._lnlike_func,
                             prior_transform=self._prior_transform,
                             ndim=len(self.modelpar),
                             ptform_args=[self.bounds, self.cube_index],
@@ -2613,17 +2613,15 @@
 
                 else:
                     if resume:
                         dsampler = dynesty.NestedSampler.restore(
                             fname=out_basename + "dynesty.save"
                         )
 
-                        print(
-                            f"Resumed a Dynesty run from {out_basename}dynesty.save"
-                        )
+                        print(f"Resumed a Dynesty run from {out_basename}dynesty.save")
 
                     else:
                         dsampler = dynesty.NestedSampler(
                             loglikelihood=self._lnlike_func,
                             prior_transform=self._prior_transform,
                             ndim=len(self.modelpar),
                             ptform_args=[self.bounds, self.cube_index],
```

### Comparing `species-0.8.0/species/fit/fit_spectrum.py` & `species-0.8.1/species/fit/fit_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/fit/retrieval.py` & `species-0.8.1/species/fit/retrieval.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,22 +688,27 @@
             self.parameters.append("log_kappa_gray")
             self.parameters.append("log_cloud_top")
 
             if "albedo" in bounds:
                 self.parameters.append("albedo")
 
         elif len(self.cloud_species) > 0:
-            self.parameters.append("fsed")
+            if self.global_fsed:
+                self.parameters.append("fsed")
+
             self.parameters.append("log_kzz")
             self.parameters.append("sigma_lnorm")
 
             for item in self.cloud_species:
                 if "log_p_base" in bounds:
                     self.parameters.append(f"log_p_base_{item}")
 
+                if not self.global_fsed:
+                    self.parameters.append(f"fsed_{item}")
+
                 cloud_lower = item[:-3].lower()
 
                 if f"{cloud_lower}_tau" in bounds:
                     self.parameters.append(f"{cloud_lower}_tau")
 
                 elif "log_tau_cloud" not in bounds:
                     if self.chemistry == "equilibrium":
@@ -1471,24 +1476,41 @@
                 cube[cube_index["albedo"]] = albedo
 
         elif len(self.cloud_species) > 0:
             # Sedimentation parameter: ratio of the settling and
             # mixing velocities of the cloud particles
             # (used in Eq. 3 of Mollière et al. 2020)
 
-            if "fsed" in bounds:
-                fsed = (
-                    bounds["fsed"][0]
-                    + (bounds["fsed"][1] - bounds["fsed"][0]) * cube[cube_index["fsed"]]
-                )
+            if self.global_fsed:
+                if "fsed" in bounds:
+                    fsed = (
+                        bounds["fsed"][0]
+                        + (bounds["fsed"][1] - bounds["fsed"][0])
+                        * cube[cube_index["fsed"]]
+                    )
+                else:
+                    # Default: 0 - 10
+                    fsed = 10.0 * cube[cube_index["fsed"]]
+
+                cube[cube_index["fsed"]] = fsed
+
             else:
-                # Default: 0 - 10
-                fsed = 10.0 * cube[cube_index["fsed"]]
+                for item in self.cloud_species:
+                    if "fsed" in bounds:
+                        fsed = (
+                            bounds["fsed"][0]
+                            + (bounds["fsed"][1] - bounds["fsed"][0])
+                            * cube[cube_index[f"fsed_{item}"]]
+                        )
 
-            cube[cube_index["fsed"]] = fsed
+                    else:
+                        # Default: 0 - 10
+                        fsed = 10.0 * cube[cube_index[f"fsed_{item}"]]
+
+                    cube[cube_index[f"fsed_{item}"]] = fsed
 
             # Log10 of the eddy diffusion coefficient (cm2 s-1)
 
             if "log_kzz" in bounds:
                 log_kzz = (
                     bounds["log_kzz"][0]
                     + (bounds["log_kzz"][1] - bounds["log_kzz"][0])
@@ -2179,15 +2201,15 @@
                 else:
                     log_x_base = {}
                     for item in self.cloud_species:
                         log_x_base[item[:-3]] = cube[cube_index[item]]
 
             # Create dictionary with cloud parameters
 
-            if "fsed" in self.parameters:
+            if "log_kzz" in self.parameters:
                 cloud_param = [
                     "fsed",
                     "log_kzz",
                     "sigma_lnorm",
                     "log_kappa_0",
                     "opa_index",
                     "log_p_base",
@@ -2200,23 +2222,23 @@
                 ]
 
                 cloud_dict = {}
                 for item in cloud_param:
                     if item in self.parameters:
                         cloud_dict[item] = cube[cube_index[item]]
 
-                    # elif item in ['log_kzz', 'sigma_lnorm']:
-                    #     cloud_dict[item] = None
-
                 for item in self.cloud_species:
                     if f"log_p_base_{item}" in self.parameters:
                         cloud_dict[f"log_p_base_{item}"] = cube[
                             cube_index[f"log_p_base_{item}"]
                         ]
 
+                    if f"fsed_{item}" in self.parameters:
+                        cloud_dict[f"fsed_{item}"] = cube[cube_index[f"fsed_{item}"]]
+
             elif "fsed_1" in self.parameters and "fsed_2" in self.parameters:
                 cloud_param_1 = [
                     "fsed_1",
                     "log_kzz",
                     "sigma_lnorm",
                     "log_kappa_0",
                     "opa_index",
@@ -3122,14 +3144,15 @@
         check_flux: Optional[float] = None,
         temp_nodes: Optional[int] = None,
         abund_nodes: Optional[int] = None,
         prior: Optional[Dict[str, Tuple[float, float]]] = None,
         check_phot_press: Optional[float] = None,
         apply_rad_vel: Optional[List[str]] = None,
         apply_vsini: Optional[List[str]] = None,
+        global_fsed: bool = True,
     ) -> None:
         """
         Function for running the atmospheric retrieval. The parameter
         estimation and computation of the marginalized likelihood (i.e.
         model evidence), is done with ``PyMultiNest`` wrapper of the
         ``MultiNest`` sampler. While ``PyMultiNest`` can be installed
         with ``pip`` from the PyPI repository, ``MultiNest`` has to to
@@ -3372,14 +3395,19 @@
             the spectra (i.e. excluding low-resolution spectra for
             which the broadening will not matter), the computation
             will be a bit faster. This parameter is only used when
             the ``vsini`` model parameter has been include in
             ``bounds``. The :math:`v \\sin(i)` is applied to all
             spectra by setting the argument of ``apply_vsini``
             to ``None``.
+        global_fsed : bool
+            Retrieve a global ``fsed`` parameter when set to ``True``
+            or retrieve the ``fsed`` parameter for each cloud species
+            individually in the ``cloud_species`` list when set to
+            ``False``.
 
         Returns
         -------
         NoneType
             None
         """
 
@@ -3394,14 +3422,15 @@
         self.prior = prior
         self.check_isothermal = check_isothermal
         self.check_flux = check_flux
         self.check_phot_press = check_phot_press
         self.cross_corr = cross_corr
         self.apply_rad_vel = apply_rad_vel
         self.apply_vsini = apply_vsini
+        self.global_fsed = global_fsed
 
         print(f"P-T profile: {self.pt_profile}")
         print(f"Chemistry: {self.chemistry}")
         print(f"Quenching: {self.quenching}")
 
         print(f"\nFit covariances: {self.fit_corr}")
 
@@ -3948,14 +3977,15 @@
             pt_smooth = kwargs.get("pt_smooth", 0.3)
             abund_smooth = kwargs.get("abund_smooth", 0.3)
             check_flux = kwargs.get("check_flux", None)
             temp_nodes = kwargs.get("temp_nodes", None)
             abund_nodes = kwargs.get("abund_nodes", None)
             prior = kwargs.get("prior", None)
             check_phot_press = kwargs.get("check_phot_press", None)
+            global_fsed = kwargs.get("global_fsed", None)
 
             self.setup_retrieval(
                 bounds=kwargs["bounds"],
                 chemistry=chemistry,
                 quenching=quenching,
                 pt_profile=pt_profile,
                 fit_corr=fit_corr,
@@ -3964,14 +3994,15 @@
                 pt_smooth=pt_smooth,
                 abund_smooth=abund_smooth,
                 check_flux=check_flux,
                 temp_nodes=temp_nodes,
                 abund_nodes=abund_nodes,
                 prior=prior,
                 check_phot_press=check_phot_press,
+                global_fsed=global_fsed,
             )
 
         @typechecked
         def _lnprior_multinest(cube, n_dim: int, n_param: int) -> None:
             """
             Function to transform the unit cube into the parameter
             cube. It is not clear how to pass additional arguments
```

### Comparing `species-0.8.0/species/phot/syn_phot.py` & `species-0.8.1/species/phot/syn_phot.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,19 +110,26 @@
             :math:`\\mathrm{m}^{-2}` :math:`\\mu\\mathrm{m}^{-1}`).
         """
 
         if self.wavel_range is None:
             read_filt = ReadFilter(self.filter_name)
             self.wavel_range = read_filt.wavelength_range()
 
-        with h5py.File(self.database, "a") as h5_file:
-            if "spectra/calibration/vega" not in h5_file:
-                add_vega(self.data_folder, h5_file)
+        with h5py.File(self.database, "r") as hdf5_file:
+            if "spectra/calibration/vega" in hdf5_file:
+                vega_found = True
+            else:
+                vega_found = False
 
-            vega_spec = np.array(h5_file["spectra/calibration/vega"])
+        if not vega_found:
+            with h5py.File(self.database, "a") as hdf5_file:
+                add_vega(self.data_folder, hdf5_file)
+
+        with h5py.File(self.database, "r") as hdf5_file:
+            vega_spec = np.array(hdf5_file["spectra/calibration/vega"])
 
         wavelength = vega_spec[0,]
         flux = vega_spec[1,]
 
         wavelength_crop = wavelength[
             (wavelength > self.wavel_range[0]) & (wavelength < self.wavel_range[1])
         ]
```

### Comparing `species-0.8.0/species/plot/plot_color.py` & `species-0.8.1/species/plot/plot_color.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/plot/plot_comparison.py` & `species-0.8.1/species/plot/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/plot/plot_evolution.py` & `species-0.8.1/species/plot/plot_evolution.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/plot/plot_mcmc.py` & `species-0.8.1/species/plot/plot_mcmc.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 from typeguard import typechecked
 from matplotlib.ticker import ScalarFormatter
 from scipy.interpolate import RegularGridInterpolator
+from scipy.stats import norm
 
 from species.core import constants
 from species.util.convert_util import logg_to_mass
 from species.util.core_util import print_section
 from species.util.plot_util import update_labels
 from species.util.dust_util import (
     check_dust_database,
@@ -214,14 +215,15 @@
     inc_log_mass: bool = False,
     inc_pt_param: bool = False,
     inc_loglike: bool = False,
     inc_abund: bool = True,
     output: Optional[str] = None,
     object_type: str = "planet",
     param_inc: Optional[List[str]] = None,
+    show_priors: bool = False,
 ) -> mpl.figure.Figure:
     """
     Function to plot the posterior distribution
     of the fitted parameters.
 
     Parameters
     ----------
@@ -279,14 +281,21 @@
         and mass are expressed in Jupiter units. With 'star', the
         radius and mass are expressed in solar units.
     param_inc : list(str), None
         List with subset of parameters that will be included in the
         posterior plot. This parameter can also be used to change the
         order of the parameters in the posterior plot. All parameters
         will be included if the argument is set to ``None``.
+    show_priors : bool
+        Plot the normal priors in the diagonal panels together with the
+        1D marginalized posterior distributions. This will only show
+        the priors that had a normal distribution, so those that were
+        set with the ``normal_prior`` parameter in
+        :class:`~species.fit.fit_model.FitModel` and
+        :class:`~species.fit.retrieval.AtmosphericRetrieval.setup_retrieval`.
 
     Returns
     -------
     matplotlib.figure.Figure
         The ``Figure`` object that can be used for further
         customization of the plot.
     """
@@ -468,39 +477,25 @@
         samples[:, param_index] *= 1e3  # (um) -> (nm)
 
     if "gauss_sigma" in box.parameters:
         param_index = np.argwhere(np.array(box.parameters) == "gauss_sigma")[0]
         samples[:, param_index] *= 1e3  # (um) -> (nm)
 
     if box.prob_sample is not None:
-        par_val = tuple(box.prob_sample.values())
-
         print("\nSample with highest probability:")
         for key, value in box.prob_sample.items():
             print(f"   - {key} = {value:.2e}")
 
     for item in box.parameters:
         if item[0:11] == "wavelength_":
             param_index = box.parameters.index(item)
 
             # (um) -> (nm)
             box.samples[:, param_index] *= 1e3
 
-    # Include a subset of parameters
-
-    if param_inc is not None:
-        param_new = np.zeros((samples.shape[0], len(param_inc)))
-        for i, item in enumerate(param_inc):
-            param_index = box.parameters.index(item)
-            param_new[:, i] = samples[:, param_index]
-
-        box.parameters = param_inc
-        ndim = len(param_inc)
-        samples = param_new
-
     # Add [C/H], [O/H], and C/O if free abundances were retrieved
 
     if box.attributes["abund_nodes"] == "None":
         for param_item in box.parameters:
             if param_item.split("_")[0] == "H2O":
                 samples = np.column_stack((samples, c_h_ratio, o_h_ratio, c_o_ratio))
                 break
@@ -538,14 +533,28 @@
                 box.parameters.append("luminosity")
                 ndim += 1
 
                 samples = np.append(samples, lum_disk / lum_planet, axis=-1)
                 box.parameters.append("luminosity_disk_planet")
                 ndim += 1
 
+                radius_bb = np.sqrt(
+                    lum_planet
+                    * constants.L_SUN
+                    / (
+                        16.0
+                        * np.pi
+                        * constants.SIGMA_SB
+                        * samples[..., teff_index] ** 4
+                    )
+                )
+                samples = np.append(samples, radius_bb / constants.R_JUP, axis=-1)
+                box.parameters.append("radius_bb")
+                ndim += 1
+
             else:
                 samples = np.append(samples, np.log10(lum_planet), axis=-1)
                 box.parameters.append("luminosity")
                 ndim += 1
 
         elif "teff_0" in box.parameters and "radius_0" in box.parameters:
             luminosity = 0.0
@@ -672,14 +681,24 @@
     if "log_mass" in box.parameters:
         mass_index = np.argwhere(np.array(box.parameters) == "log_mass")[0]
         if object_type == "star":
             samples[:, mass_index] = np.log10(
                 10.0 ** samples[:, mass_index] * constants.M_JUP / constants.M_SUN
             )
 
+    if "disk_radius" in box.parameters:
+        radius_index = np.argwhere(np.array(box.parameters) == "disk_radius")[0]
+        if object_type == "star":
+            samples[:, radius_index] *= constants.R_JUP / constants.AU
+
+    if "radius_bb" in box.parameters:
+        radius_index = np.argwhere(np.array(box.parameters) == "radius_bb")[0]
+        if object_type == "star":
+            samples[:, radius_index] *= constants.R_JUP / constants.AU
+
     # Include the log-likelihood
 
     if inc_loglike:
         # Get ln(L) of the samples
         ln_prob = box.ln_prob[..., np.newaxis]
 
         # Normalized by the maximum ln(L)
@@ -696,15 +715,19 @@
 
         samples = np.append(samples, np.log10(prob), axis=-1)
         box.parameters.append("log_prob")
         ndim += 1
 
     # Remove abundances
 
-    if not inc_abund and box.attributes["chemistry"] == "free":
+    if (
+        not inc_abund
+        and "chemistry" in box.attributes
+        and box.attributes["chemistry"] == "free"
+    ):
         index_del = []
         item_del = []
 
         if box.attributes["abund_nodes"] == "None":
             for line_item in line_species:
                 param_index = np.argwhere(np.array(box.parameters) == line_item)[0]
                 index_del.append(param_index)
@@ -721,16 +744,30 @@
 
         samples = np.delete(samples, index_del, axis=1)
         ndim -= len(index_del)
 
         for item in item_del:
             box.parameters.remove(item)
 
+    # Include a subset of parameters
+
+    if param_inc is not None:
+        param_new = np.zeros((samples.shape[0], len(param_inc)))
+        for i, item in enumerate(param_inc):
+            if item in box.parameters:
+                param_index = box.parameters.index(item)
+                param_new[:, i] = samples[:, param_index]
+
+        box.parameters = param_inc
+        ndim = len(param_inc)
+        samples = param_new
+
     # Update axes labels
 
+    box_param = box.parameters.copy()
     labels = update_labels(box.parameters, object_type=object_type)
 
     # Check if parameter values were fixed
 
     index_sel = []
     index_del = []
 
@@ -745,14 +782,20 @@
     for i in range(len(index_del) - 1, -1, -1):
         del labels[index_del[i]]
 
     ndim -= len(index_del)
 
     samples = samples.reshape((-1, ndim))
 
+    # Get parameter values of maximum likelihood
+
+    if max_prob:
+        max_idx = np.argmax(box.ln_prob)
+        max_sample = samples[max_idx, :]
+
     if isinstance(title_fmt, list) and len(title_fmt) != ndim:
         raise ValueError(
             f"The number of items in the list of 'title_fmt' ({len(title_fmt)}) is "
             f"not equal to the number of dimensions of the samples ({ndim})."
         )
 
     hist_titles = []
@@ -800,17 +843,36 @@
         title_kwargs={"fontsize": 12},
     )
 
     axes = np.array(fig.axes).reshape((ndim, ndim))
 
     for i in range(ndim):
         for j in range(ndim):
-            if i >= j:
-                ax = axes[i, j]
+            ax = axes[i, j]
+
+            if show_priors and i == j and box_param[i] in box.normal_priors:
+                norm_param = box.normal_priors[box_param[i]]
 
+                x_norm = np.linspace(
+                    norm_param[0] - 5.0 * norm_param[1],
+                    norm_param[0] + 5.0 * norm_param[1],
+                    200,
+                )
+
+                y_norm = norm.pdf(x_norm, norm_param[0], norm_param[1])
+
+                ax.plot(
+                    x_norm,
+                    0.9 * ax.get_ylim()[1] * y_norm / np.amax(y_norm),
+                    ls=":",
+                    lw=2.0,
+                    color="dodgerblue",
+                )
+
+            if i >= j:
                 ax.xaxis.set_major_formatter(ScalarFormatter(useOffset=False))
                 ax.yaxis.set_major_formatter(ScalarFormatter(useOffset=False))
 
                 labelleft = j == 0 and i != 0
                 labelbottom = i == ndim - 1
 
                 ax.tick_params(
@@ -851,20 +913,20 @@
                     labeltop=False,
                 )
 
                 if limits is not None:
                     ax.set_xlim(limits[j])
 
                 if max_prob:
-                    ax.axvline(par_val[j], color="tomato")
+                    ax.axvline(max_sample[j], color="tomato")
 
                 if i > j:
                     if max_prob:
-                        ax.axhline(par_val[i], color="tomato")
-                        ax.plot(par_val[j], par_val[i], "s", color="tomato")
+                        ax.axhline(max_sample[i], color="tomato")
+                        ax.plot(max_sample[j], max_sample[i], "s", color="tomato")
 
                     if limits is not None:
                         ax.set_ylim(limits[i])
 
                 if offset is not None:
                     ax.get_xaxis().set_label_coords(0.5, offset[0])
                     ax.get_yaxis().set_label_coords(offset[1], 0.5)
```

### Comparing `species-0.8.0/species/plot/plot_retrieval.py` & `species-0.8.1/species/plot/plot_retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     pressure = np.logspace(-6.0, np.log10(max_press), 180)
 
     if "tint" in parameters and "log_delta" in parameters and "alpha" in parameters:
         pt_profile = "molliere"
 
     elif "tint" in parameters and "log_delta" in parameters:
         pt_profile = "eddington"
-    
+
     elif "T_bottom" in parameters and "PTslope_1" in parameters:
         pt_profile = "gradient"
 
     else:
         pt_profile = "free"
 
         temp_index = []
@@ -296,32 +296,37 @@
             )
 
         elif pt_profile == "eddington":
             tau = pressure * 1e6 * 10.0 ** item[param_index["log_delta"]]
             temp = (0.75 * item[param_index["tint"]] ** 4.0 * (2.0 / 3.0 + tau)) ** 0.25
 
         elif pt_profile == "gradient":
-            num_layer = 6 # could make a variable in the future
+            num_layer = 6  # could make a variable in the future
             layer_pt_slopes = np.ones(num_layer) * np.nan
             for index in range(num_layer):
-                layer_pt_slopes[index] = item[param_index[f'PTslope_{num_layer - index}']]
+                layer_pt_slopes[index] = item[
+                    param_index[f"PTslope_{num_layer - index}"]
+                ]
 
             try:
                 from petitRADTRANS.physics import dTdP_temperature_profile
-            except ImportError as e:
+            except ImportError as import_error:
                 raise ImportError(
-                    """Can\'t import the dTdP profile function from petitRADTRANS,
-                    check that your version of pRT includes this function in   
-                    petitRADTRANS.physics""", e
+                    "Can't import the dTdP profile function from "
+                    "petitRADTRANS, check that your version of pRT "
+                    "includes this function in petitRADTRANS.physics",
+                    import_error,
                 )
 
-            temp = dTdP_temperature_profile(pressure,
-                                            num_layer, # could change in the future
-                                            layer_pt_slopes,
-                                            item[param_index["T_bottom"]])
+            temp = dTdP_temperature_profile(
+                pressure,
+                num_layer,  # could change in the future
+                layer_pt_slopes,
+                item[param_index["T_bottom"]],
+            )
 
         elif pt_profile == "free":
             knot_temp = []
             for j in range(temp_nodes):
                 knot_temp.append(item[temp_index[j]])
 
             knot_temp = np.asarray(knot_temp)
```

### Comparing `species-0.8.0/species/plot/plot_spectrum.py` & `species-0.8.1/species/plot/plot_spectrum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 """
 Module with a function for plotting a spectral energy distribution
 that includes photometric and/or spectral data and/or models.
 """
 
 import math
-import warnings
 
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 
 from typeguard import typechecked
-from matplotlib.ticker import AutoMinorLocator, ScalarFormatter
+from matplotlib.ticker import AutoMinorLocator
 
 from species.core.box import (
     ModelBox,
     ObjectBox,
     PhotometryBox,
     ResidualsBox,
     SpectrumBox,
     SynphotBox,
 )
 from species.read.read_filter import ReadFilter
 from species.util.core_util import print_section
+from species.util.data_util import convert_units
 from species.util.plot_util import create_model_label
 
 
 @typechecked
 def plot_spectrum(
     boxes: list,
     filters: Optional[List[str]] = None,
@@ -118,16 +118,17 @@
         if set to ``None``.
     scale : tuple(str, str), None
         Scale of the x and y axes ('linear' or 'log').
         The scale is set to ``('linear', 'linear')`` if
         set to ``None``.
     title : str
         Title.
-    offset : tuple(float, float)
-        Offset for the label of the x- and y-axis.
+    offset : tuple(float, float), None
+        Offset for the label of the x- and y-axis. Default offset is
+        used when the argument is set to ``None``.
     legend : str, tuple, dict, list(dict, dict), None
         Location of the legend (str or tuple(float, float))
         or a dictionary with the ``**kwargs`` of
         ``matplotlib.pyplot.legend``, for example
         ``{'loc': 'upper left', 'fontsize: 12.}``. Alternatively,
         a list with two values can be provided to separate the
         model and data handles in two legends. Each of these two
@@ -164,16 +165,18 @@
     grid_hspace : float
         The relative height spacing between subplots, expressed
         as a fraction of the average axis height. The default
         value is set to 0.1.
     inc_model_name : bool
         Include the model name in the legend of any
         :class:`~species.core.box.ModelBox`.
-    units : tuple(str, str)
-        This parameter has not yet been implemented.
+    units : tuple(str, str), None
+        Tuple with the wavelength and flux units. Supported
+        units can be found in the docstring of
+        :func:`~species.util.data_util.convert_units`.
 
     Returns
     -------
     matplotlib.figure.Figure
         The ``Figure`` object that can be used for further
         customization of the plot.
     """
@@ -186,14 +189,15 @@
             item_type = item[0].__class__.__name__
             print(f"   - List with {len(item)} x {item_type}")
         else:
             print(f"   - {item.__class__.__name__}")
 
     print(f"\nObject type: {object_type}")
     print(f"Quantity: {quantity}")
+    print(f"Units: {units}")
     print(f"Filter profiles: {filters}")
 
     print(f"\nFigure size: {figsize}")
     print(f"Legend parameters: {leg_param}")
     print(f"Include model name: {inc_model_name}")
 
     plt.rcParams["font.family"] = "serif"
@@ -225,14 +229,15 @@
 
     param_add = [
         "radius",
         "logg",
         "feh",
         "metallicity",
         "fsed",
+        "log_kzz",
         "distance",
         "parallax",
         "mass",
         "ism_ext",
         "lognorm_ext",
         "powerlaw_ext",
         "log_flux_scaling",
@@ -416,79 +421,97 @@
         if scale[0] == "linear":
             ax2.xaxis.set_minor_locator(AutoMinorLocator(5))
 
     if residuals is not None:
         if scale[0] == "linear":
             ax3.xaxis.set_minor_locator(AutoMinorLocator(5))
 
+    if units[0] in ["um", "µm"]:
+        x_label = "Wavelength (µm)"
+    elif units[0] in ["angstrom", "A", "AA", "Å"]:
+        x_label = r"Wavelength ($\AA$)"
+    elif units[0] == "Hz":
+        x_label = "Frequency (Hz)"
+    elif units[0] == "GHz":
+        x_label = "Frequency (GHz)"
+    else:
+        x_label = f"Wavelength ({units[0]})"
+
+    if units[1] in ["W m-2 um-1", "W m-2 µm-1"]:
+        y_unit = "W m$^{-2}$ µm$^{-1}$"
+    elif units[1] == "W m-2 m-1":
+        y_unit = r"W m$^{-2}$ m$^{-1}$"
+    elif units[1] == "W m-2 Hz-1":
+        y_unit = r"W m$^{-2}$ Hz$^{-1}$"
+    elif units[1] in [
+        "erg s-1 cm-2 angstrom-1",
+        "erg s-1 cm-2 A-1",
+        "erg s-1 cm-2 AA-1",
+        "erg s-1 cm-2 Å-1",
+    ]:
+        y_unit = r"erg s$^{-2}$ cm$^{-2}$ $\AA$$^{-1}$"
+    elif units[1] == "erg s-1 cm-2 Hz-1":
+        y_unit = r"erg s$^{-2}$ cm$^{-2}$ Hz$^{-1}$"
+    else:
+        y_unit = units[1]
+
     if residuals is not None and filters is not None:
         ax1.set_xlabel("")
         ax2.set_xlabel("")
-        ax3.set_xlabel("Wavelength (\N{GREEK SMALL LETTER MU}m)", fontsize=13)
+        ax3.set_xlabel(x_label, fontsize=11)
 
     elif residuals is not None:
         ax1.set_xlabel("")
-        ax3.set_xlabel("Wavelength (\N{GREEK SMALL LETTER MU}m)", fontsize=11)
+        ax3.set_xlabel(x_label, fontsize=11)
 
     elif filters is not None:
-        ax1.set_xlabel("Wavelength (\N{GREEK SMALL LETTER MU}m)", fontsize=13)
+        ax1.set_xlabel(x_label, fontsize=11)
         ax2.set_xlabel("")
 
     else:
-        ax1.set_xlabel("Wavelength (\N{GREEK SMALL LETTER MU}m)", fontsize=13)
+        ax1.set_xlabel(x_label, fontsize=11)
 
     if filters is not None:
-        ax2.set_ylabel(r"$T_\lambda$", fontsize=13)
+        ax2.set_ylabel(r"$T_\lambda$", fontsize=11)
 
     if residuals is not None:
         if quantity == "flux density":
             ax3.set_ylabel(r"$\Delta$$F_\lambda$ ($\sigma$)", fontsize=11)
 
         elif quantity == "flux":
             ax3.set_ylabel(r"$\Delta$$F_\lambda$ ($\sigma$)", fontsize=11)
 
-    if xlim is None:
-        ax1.set_xlim(0.5, 5.0)
-    else:
-        ax1.set_xlim(xlim[0], xlim[1])
-
     if quantity == "magnitude":
         scaling = 1.0
-        ax1.set_ylabel("Contrast (mag)", fontsize=13)
+        ax1.set_ylabel("Contrast (mag)", fontsize=11)
 
-        if ylim:
+        if ylim is not None:
             ax1.set_ylim(ylim[0], ylim[1])
 
     else:
-        if ylim:
+        if ylim is not None:
             ax1.set_ylim(ylim[0], ylim[1])
 
             ylim = ax1.get_ylim()
 
             if scale[1] == "linear":
                 exponent = math.floor(math.log10(ylim[1]))
                 scaling = 10.0**exponent
 
             else:
                 exponent = None
                 scaling = 1.0
 
             if quantity == "flux density":
                 if exponent is None:
-                    ylabel = (
-                        r"$F_\lambda$ (W m$^{-2}$ "
-                        + "\N{GREEK SMALL LETTER MU}m$^{-1}$)"
-                    )
+                    ylabel = rf"$F_\lambda$ ({y_unit})"
 
                 else:
                     ylabel = (
-                        r"$F_\lambda$ (10$^{"
-                        + str(exponent)
-                        + r"}$"
-                        + " W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)"
+                        r"$F_\lambda$ (10$^{" + str(exponent) + r"}$" + f" {y_unit})"
                     )
 
             elif quantity == "flux":
                 if exponent is None:
                     ylabel = r"$\lambda$$F_\lambda$ (W m$^{-2}$)"
 
                 else:
@@ -505,32 +528,23 @@
                 ax1.axhline(
                     0.0, ls="--", lw=0.7, color="gray", dashes=(2, 4), zorder=0.5
                 )
 
         else:
             if quantity == "flux density":
                 ax1.set_ylabel(
-                    r"$F_\lambda$" + " (W m$^{-2}$ \N{GREEK SMALL LETTER MU}m$^{-1}$)",
+                    rf"$F_\lambda$ ({y_unit})",
                     fontsize=11,
                 )
 
             elif quantity == "flux":
                 ax1.set_ylabel(r"$\lambda$$F_\lambda$ (W m$^{-2}$)", fontsize=11)
 
             scaling = 1.0
 
-    xlim = ax1.get_xlim()
-
-    if filters is not None:
-        ax2.set_xlim(xlim[0], xlim[1])
-        ax2.set_ylim(0.0, 1.0)
-
-    if residuals is not None:
-        ax3.set_xlim(xlim[0], xlim[1])
-
     if offset is not None and residuals is not None and filters is not None:
         ax3.get_xaxis().set_label_coords(0.5, offset[0])
 
         ax1.get_yaxis().set_label_coords(offset[1], 0.5)
         ax2.get_yaxis().set_label_coords(offset[1], 0.5)
         ax3.get_yaxis().set_label_coords(offset[1], 0.5)
 
@@ -546,31 +560,35 @@
         ax1.get_yaxis().set_label_coords(offset[1], 0.5)
         ax3.get_yaxis().set_label_coords(offset[1], 0.5)
 
     elif offset is not None:
         ax1.get_xaxis().set_label_coords(0.5, offset[0])
         ax1.get_yaxis().set_label_coords(offset[1], 0.5)
 
-    # else:
-    #     ax1.get_xaxis().set_label_coords(0.5, -0.12)
-    #     ax1.get_yaxis().set_label_coords(-0.1, 0.5)
+    data_labels = []
 
     for j, box_item in enumerate(boxes):
         flux_scaling = 1.0
 
         if j < len(boxes):
             plot_kwargs.append(None)
 
         if isinstance(box_item, (SpectrumBox, ModelBox)):
             wavelength = box_item.wavelength
             flux = box_item.flux
 
+            data_in = np.column_stack([wavelength, flux])
+            data_out = convert_units(data_in, units, convert_from=False)
+
+            wavelength = data_out[:, 0]
+            flux = data_out[:, 1]
+
             if isinstance(wavelength[0], (np.float32, np.float64)):
                 data = np.array(flux, dtype=np.float64)
-                masked = np.ma.array(data, mask=np.isnan(data))
+                flux_masked = np.ma.array(data, mask=np.isnan(data))
 
                 if isinstance(box_item, ModelBox):
                     param = box_item.parameters.copy()
 
                     label = create_model_label(
                         model_param=param,
                         object_type=object_type,
@@ -598,80 +616,88 @@
                         flux_scaling = wavelength
 
                     if "zorder" not in kwargs_copy:
                         kwargs_copy["zorder"] = 2.0
 
                     ax1.plot(
                         wavelength,
-                        flux_scaling * masked / scaling,
+                        flux_scaling * flux_masked / scaling,
                         label=label,
                         **kwargs_copy,
                     )
 
                 else:
                     if quantity == "flux":
                         flux_scaling = wavelength
 
                     ax1.plot(
                         wavelength,
-                        flux_scaling * masked / scaling,
+                        flux_scaling * flux_masked / scaling,
                         lw=0.5,
                         label=label,
                         zorder=2,
                     )
 
             elif isinstance(wavelength[0], (np.ndarray)):
                 for i, item in enumerate(wavelength):
                     data = np.array(flux[i], dtype=np.float64)
-                    masked = np.ma.array(data, mask=np.isnan(data))
+                    flux_masked = np.ma.array(data, mask=np.isnan(data))
 
                     if isinstance(box_item.name[i], bytes):
                         label = box_item.name[i].decode("utf-8")
                     else:
                         label = box_item.name[i]
 
                     if quantity == "flux":
                         flux_scaling = item
 
-                    ax1.plot(item, flux_scaling * masked / scaling, lw=0.5, label=label)
+                    ax1.plot(
+                        item, flux_scaling * flux_masked / scaling, lw=0.5, label=label
+                    )
 
         elif isinstance(box_item, list):
             if envelope:
                 spec_list = np.zeros((len(box_item), box_item[0].flux.size))
             else:
                 spec_list = None
 
             for i, item in enumerate(box_item):
                 wavelength = item.wavelength
                 flux = item.flux
 
+                data_in = np.column_stack([wavelength, flux])
+                data_out = convert_units(data_in, units, convert_from=False)
+
+                wavelength = data_out[:, 0]
+                flux = data_out[:, 1]
+
                 # data = np.array(flux, dtype=np.float64)
                 data = flux.astype(np.float64)
-                masked = np.ma.array(data, mask=np.isnan(data))
+                flux_masked = np.ma.array(data, mask=np.isnan(data))
 
                 if quantity == "flux":
                     flux_scaling = wavelength
 
                 if envelope:
                     spec_list[i] = flux
 
                 else:
                     if plot_kwargs[j]:
                         if "zorder" not in plot_kwargs[j]:
                             plot_kwargs[j]["zorder"] = 1.0
 
                         ax1.plot(
                             wavelength,
-                            flux_scaling * masked / scaling,
+                            flux_scaling * flux_masked / scaling,
                             **plot_kwargs[j],
                         )
                     else:
                         ax1.plot(
                             wavelength,
-                            flux_scaling * masked / scaling,
+                            flux_scaling * flux_masked / scaling,
                             color="gray",
                             lw=0.2,
                             alpha=0.5,
                             zorder=1,
                         )
 
             if envelope:
@@ -804,182 +830,238 @@
 
                 sort_index = np.argsort(wavel_list)
                 spec_sort = []
 
                 for i in range(sort_index.size):
                     spec_sort.append(spec_list[sort_index[i]])
 
-                for key in spec_sort:
+                for spec_key in spec_sort:
                     masked = np.ma.array(
-                        box_item.spectrum[key][0],
-                        mask=np.isnan(box_item.spectrum[key][0]),
+                        box_item.spectrum[spec_key][0],
+                        mask=np.isnan(box_item.spectrum[spec_key][0]),
                     )
 
+                    masked = convert_units(masked, units, convert_from=False)
+
                     if quantity == "flux":
                         flux_scaling = masked[:, 0]
 
-                    if not plot_kwargs[j] or key not in plot_kwargs[j]:
+                    if plot_kwargs[j] and spec_key in plot_kwargs[j]:
+                        if "label" in plot_kwargs[j][spec_key]:
+                            data_labels.append(plot_kwargs[j][spec_key]["label"])
+
+                    if not plot_kwargs[j] or spec_key not in plot_kwargs[j]:
                         plot_obj = ax1.errorbar(
                             masked[:, 0],
                             flux_scaling * masked[:, 1] / scaling,
                             yerr=flux_scaling * masked[:, 2] / scaling,
                             ms=2,
                             marker="s",
                             zorder=2.5,
                             ls="none",
                         )
 
                         if plot_kwargs[j] is None:
                             plot_kwargs[j] = {}
 
-                        plot_kwargs[j][key] = {
+                        plot_kwargs[j][spec_key] = {
                             "marker": "s",
                             "ms": 2.0,
                             "ls": "none",
                             "color": plot_obj[0].get_color(),
                         }
 
-                    elif "marker" not in plot_kwargs[j][key]:
+                    elif (
+                        "marker" not in plot_kwargs[j][spec_key]
+                        or plot_kwargs[j][spec_key]["marker"] == "none"
+                    ):
                         # Plot the spectrum as a line without error bars
                         # (e.g. when the spectrum has a high spectral resolution)
                         plot_obj = ax1.plot(
                             masked[:, 0],
                             flux_scaling * masked[:, 1] / scaling,
-                            **plot_kwargs[j][key],
+                            **plot_kwargs[j][spec_key],
                         )
 
                     else:
-                        if "zorder" not in plot_kwargs[j][key]:
-                            plot_kwargs[j][key]["zorder"] = 2.5
+                        if "zorder" not in plot_kwargs[j][spec_key]:
+                            plot_kwargs[j][spec_key]["zorder"] = 2.5
 
                         ax1.errorbar(
                             masked[:, 0],
                             flux_scaling * masked[:, 1] / scaling,
                             yerr=flux_scaling * masked[:, 2] / scaling,
-                            **plot_kwargs[j][key],
+                            xerr=None,
+                            **plot_kwargs[j][spec_key],
                         )
 
             if box_item.flux is not None:
                 filter_list = []
                 wavel_list = []
 
-                for item in box_item.flux:
-                    read_filt = ReadFilter(item)
-                    filter_list.append(item)
+                for filter_item in box_item.flux:
+                    read_filt = ReadFilter(filter_item)
+                    filter_list.append(filter_item)
                     wavel_list.append(read_filt.mean_wavelength())
 
                 sort_index = np.argsort(wavel_list)
                 filter_sort = []
 
                 for i in range(sort_index.size):
                     filter_sort.append(filter_list[sort_index[i]])
 
-                for item in filter_sort:
-                    transmission = ReadFilter(item)
-                    wavelength = transmission.mean_wavelength()
-                    fwhm = transmission.filter_fwhm()
+                for filter_item in filter_sort:
+                    transmission = ReadFilter(filter_item)
+                    wavel_micron = transmission.mean_wavelength()
+                    fwhm_micron = transmission.filter_fwhm()
+
+                    if isinstance(box_item.flux[filter_item][0], np.ndarray):
+                        raise NotImplementedError(
+                            "Unit conversion has not yet been implemented! "
+                            "Please open an issue on Github."
+                        )
+
+                    else:
+                        data_in = np.column_stack(
+                            [
+                                [wavel_micron],
+                                [box_item.flux[filter_item][0]],
+                                [box_item.flux[filter_item][1]],
+                            ]
+                        )
+                        data_out = convert_units(data_in, units, convert_from=False)
 
-                    if not plot_kwargs[j] or item not in plot_kwargs[j]:
+                        wavelength = data_out[:, 0]
+                        flux_conv = data_out[:, 1]
+                        sigma_conv = data_out[:, 2]
+
+                    # Convert FWHM of filter to requested units
+                    data_in = np.column_stack(
+                        [[wavel_micron + fwhm_micron / 2.0], [1.0]]
+                    )
+                    data_out = convert_units(data_in, units, convert_from=False)
+
+                    # Absolute value because could be negative when frequency
+                    fwhm_up = np.abs(data_out[0, 0] - wavelength[0])
+
+                    # Convert FWHM of filter to requested units
+                    data_in = np.column_stack(
+                        [[wavel_micron - fwhm_micron / 2.0], [1.0]]
+                    )
+                    data_out = convert_units(data_in, units, convert_from=False)
+
+                    # Absolute value because could be negative when frequency
+                    fwhm_down = np.abs(data_out[0, 0] - wavelength[0])
+
+                    # Calculate the average, which will be identical
+                    # to fwhm_up and fwhm_down when working with
+                    # wavelengths but fwhm_up and fwhm_down will
+                    # be different when convertin a FWHM from
+                    # wavelength to frequency
+                    fwhm = (fwhm_up + fwhm_down) / 2.0
+
+                    if plot_kwargs[j] and filter_item in plot_kwargs[j]:
+                        if "label" in plot_kwargs[j][filter_item]:
+                            data_labels.append(plot_kwargs[j][filter_item]["label"])
+
+                    if not plot_kwargs[j] or filter_item not in plot_kwargs[j]:
                         if not plot_kwargs[j]:
                             plot_kwargs[j] = {}
 
                         if quantity == "flux":
                             flux_scaling = wavelength
 
                         scale_tmp = flux_scaling / scaling
 
-                        if isinstance(box_item.flux[item][0], np.ndarray):
-                            for i in range(box_item.flux[item].shape[1]):
+                        if isinstance(box_item.flux[filter_item][0], np.ndarray):
+                            for i in range(box_item.flux[filter_item].shape[1]):
                                 plot_obj = ax1.errorbar(
                                     wavelength,
-                                    scale_tmp * box_item.flux[item][0, i],
+                                    scale_tmp * box_item.flux[filter_item][0, i],
                                     xerr=fwhm / 2.0,
-                                    yerr=scale_tmp * box_item.flux[item][1, i],
+                                    yerr=scale_tmp * box_item.flux[filter_item][1, i],
                                     marker="s",
                                     ms=5,
                                     zorder=3,
                                     color="black",
                                 )
 
                         else:
                             plot_obj = ax1.errorbar(
                                 wavelength,
-                                scale_tmp * box_item.flux[item][0],
+                                scale_tmp * flux_conv,
                                 xerr=fwhm / 2.0,
-                                yerr=scale_tmp * box_item.flux[item][1],
+                                yerr=scale_tmp * sigma_conv,
                                 marker="s",
                                 ms=5,
                                 zorder=3,
                                 color="black",
                             )
 
-                        plot_kwargs[j][item] = {
+                        plot_kwargs[j][filter_item] = {
                             "marker": "s",
                             "ms": 5.0,
                             "color": plot_obj[0].get_color(),
                         }
 
                     else:
                         if quantity == "flux":
                             flux_scaling = wavelength
 
-                        if isinstance(box_item.flux[item][0], np.ndarray):
-                            if not isinstance(plot_kwargs[j][item], list):
+                        if isinstance(box_item.flux[filter_item][0], np.ndarray):
+                            if not isinstance(plot_kwargs[j][filter_item], list):
                                 raise ValueError(
-                                    f"A list with {box_item.flux[item].shape[1]} "
+                                    f"A list with {box_item.flux[filter_item].shape[1]} "
                                     f"dictionaries are required because the filter "
-                                    f"{item} has {box_item.flux[item].shape[1]} "
+                                    f"{filter_item} has {box_item.flux[filter_item].shape[1]} "
                                     f"values."
                                 )
 
-                            for i in range(box_item.flux[item].shape[1]):
-                                if "zorder" not in plot_kwargs[j][item][i]:
-                                    plot_kwargs[j][item][i]["zorder"] = 3.0
+                            for i in range(box_item.flux[filter_item].shape[1]):
+                                if "zorder" not in plot_kwargs[j][filter_item][i]:
+                                    plot_kwargs[j][filter_item][i]["zorder"] = 3.0
 
                                 ax1.errorbar(
                                     wavelength,
-                                    flux_scaling * box_item.flux[item][0, i] / scaling,
+                                    flux_scaling
+                                    * box_item.flux[filter_item][0, i]
+                                    / scaling,
                                     xerr=fwhm / 2.0,
                                     yerr=flux_scaling
-                                    * box_item.flux[item][1, i]
+                                    * box_item.flux[filter_item][1, i]
                                     / scaling,
-                                    **plot_kwargs[j][item][i],
+                                    **plot_kwargs[j][filter_item][i],
                                 )
 
                         else:
-                            if box_item.flux[item][1] == 0.0:
-                                if "zorder" not in plot_kwargs[j][item]:
-                                    plot_kwargs[j][item]["zorder"] = 3.0
+                            if box_item.flux[filter_item][1] == 0.0:
+                                if "zorder" not in plot_kwargs[j][filter_item]:
+                                    plot_kwargs[j][filter_item]["zorder"] = 3.0
 
                                 ax1.errorbar(
                                     wavelength,
-                                    flux_scaling * box_item.flux[item][0] / scaling,
+                                    flux_scaling * flux_conv / scaling,
                                     xerr=fwhm / 2.0,
-                                    yerr=0.5
-                                    * flux_scaling
-                                    * box_item.flux[item][0]
-                                    / scaling,
+                                    yerr=0.5 * flux_scaling * sigma_conv / scaling,
                                     uplims=True,
                                     capsize=2.0,
                                     capthick=0.0,
-                                    **plot_kwargs[j][item],
+                                    **plot_kwargs[j][filter_item],
                                 )
 
                             else:
-                                if "zorder" not in plot_kwargs[j][item]:
-                                    plot_kwargs[j][item]["zorder"] = 3.0
+                                if "zorder" not in plot_kwargs[j][filter_item]:
+                                    plot_kwargs[j][filter_item]["zorder"] = 3.0
 
                                 ax1.errorbar(
                                     wavelength,
-                                    flux_scaling * box_item.flux[item][0] / scaling,
+                                    flux_scaling * flux_conv / scaling,
                                     xerr=fwhm / 2.0,
-                                    yerr=flux_scaling
-                                    * box_item.flux[item][1]
-                                    / scaling,
-                                    **plot_kwargs[j][item],
+                                    yerr=flux_scaling * sigma_conv / scaling,
+                                    **plot_kwargs[j][filter_item],
                                 )
 
         elif isinstance(box_item, SynphotBox):
             obj_index = None
 
             for i, find_item in enumerate(boxes):
                 if isinstance(find_item, ObjectBox):
@@ -1023,16 +1105,17 @@
                         ms=5,
                         zorder=4,
                         mfc="white",
                     )
 
                 else:
                     if isinstance(plot_kwargs[obj_index][item], list):
-                        # In case of multiple photometry values for the same filter, use the
-                        # plot_kwargs of the first data point
+                        # In case of multiple photometry values for the
+                        # same filter, use the plot_kwargs of the first
+                        # data point
 
                         kwargs_copy = plot_kwargs[obj_index][item][0].copy()
 
                         if "label" in kwargs_copy:
                             del kwargs_copy["label"]
 
                         if "zorder" not in kwargs_copy:
@@ -1069,14 +1152,20 @@
                         )
 
     if filters is not None:
         for i, item in enumerate(filters):
             transmission = ReadFilter(item)
             data = transmission.get_filter()
 
+            data_in = np.ones(data.shape)
+            data_in[:, 0] = data[:, 0]
+
+            data_out = convert_units(data_in, units, convert_from=False)
+            data[:, 0] = data_out[:, 0]
+
             ax2.plot(data[:, 0], data[:, 1], "-", lw=0.7, color="tab:gray", zorder=1)
 
     if residuals is not None:
         obj_index = None
 
         for i, find_item in enumerate(boxes):
             if isinstance(find_item, ObjectBox):
@@ -1090,14 +1179,20 @@
                 "the list of boxes."
             )
 
         res_max = 0.0
 
         if residuals.photometry is not None:
             for item in residuals.photometry:
+                data_in = np.array(
+                    [[residuals.photometry[item][0], residuals.photometry[item][1]]]
+                )
+                data_out = convert_units(data_in, units, convert_from=False)
+                residuals.photometry[item][0] = data_out[0, 0]
+
                 if not plot_kwargs[obj_index] or item not in plot_kwargs[obj_index]:
                     ax3.plot(
                         residuals.photometry[item][0],
                         residuals.photometry[item][1],
                         marker="s",
                         ms=5,
                         linestyle="none",
@@ -1141,37 +1236,48 @@
 
                 max_tmp = np.max(np.abs(residuals.photometry[item][1][finite]))
 
                 if max_tmp > res_max:
                     res_max = max_tmp
 
         if residuals.spectrum is not None:
-            for key, value in residuals.spectrum.items():
-                if not plot_kwargs[obj_index] or key not in plot_kwargs[obj_index]:
+            for spec_key, spec_val in residuals.spectrum.items():
+                data_out = convert_units(spec_val, units, convert_from=False)
+                spec_val[:, 0] = data_out[:, 0]
+
+                if not plot_kwargs[obj_index] or spec_key not in plot_kwargs[obj_index]:
                     ax3.errorbar(
-                        value[:, 0], value[:, 1], marker="o", ms=2, ls="none", zorder=1
+                        spec_val[:, 0],
+                        spec_val[:, 1],
+                        marker="o",
+                        ms=2,
+                        ls="none",
+                        zorder=1,
                     )
 
                 else:
-                    if "zorder" not in plot_kwargs[obj_index][key]:
-                        plot_kwargs[obj_index][key]["zorder"] = 1.0
+                    if "zorder" not in plot_kwargs[obj_index][spec_key]:
+                        plot_kwargs[obj_index][spec_key]["zorder"] = 1.0
 
                     ax3.errorbar(
-                        value[:, 0],
-                        value[:, 1],
-                        **plot_kwargs[obj_index][key],
+                        spec_val[:, 0],
+                        spec_val[:, 1],
+                        **plot_kwargs[obj_index][spec_key],
                     )
 
-                max_tmp = np.nanmax(np.abs(value[:, 1]))
+                max_tmp = np.nanmax(np.abs(spec_val[:, 1]))
 
                 if max_tmp > res_max:
                     res_max = max_tmp
 
         res_lim = math.ceil(1.1 * res_max)
 
+        if res_lim == 0.0:
+            res_lim = 5.0
+
         if res_lim > 10.0:
             res_lim = 5.0
 
         ax3.axhline(0.0, ls="--", lw=0.7, color="gray", dashes=(2, 4), zorder=0.5)
 
         if res_lim > 5.0 or (
             ylim_res is not None and ylim_res[0] < -5.0 and ylim_res[1] > 5.0
@@ -1196,31 +1302,23 @@
 
     handles, labels = ax1.get_legend_handles_labels()
 
     if handles and legend is not None:
         if isinstance(legend, list):
             model_handles = []
             data_handles = []
-
             model_labels = []
-            data_labels = []
-
-            for i, item in enumerate(handles):
-                if isinstance(item, mpl.lines.Line2D):
-                    model_handles.append(item)
-                    model_labels.append(labels[i])
-
-                elif isinstance(item, mpl.container.ErrorbarContainer):
-                    data_handles.append(item)
-                    data_labels.append(labels[i])
+            # data_labels = []
 
+            for handle_idx, handle_item in enumerate(handles):
+                if labels[handle_idx] in data_labels:
+                    data_handles.append(handle_item)
                 else:
-                    warnings.warn(
-                        f"The object type {item} is not implemented for the legend."
-                    )
+                    model_handles.append(handle_item)
+                    model_labels.append(labels[handle_idx])
 
             if legend[0] is not None:
                 if isinstance(legend[0], (str, tuple)):
                     leg_1 = ax1.legend(
                         model_handles,
                         model_labels,
                         loc=legend[0],
@@ -1250,22 +1348,43 @@
 
         elif isinstance(legend, (str, tuple)):
             ax1.legend(loc=legend, fontsize=8, frameon=False)
 
         else:
             ax1.legend(**legend)
 
-    if scale[0] == "log":
-        ax1.xaxis.set_major_formatter(ScalarFormatter())
+    # if scale[0] == "log":
+    #     ax1.xaxis.set_major_formatter(ScalarFormatter())
+    #
+    #     if ax2 is not None:
+    #         ax2.xaxis.set_major_formatter(ScalarFormatter())
+    #
+    #     if ax3 is not None:
+    #         ax3.xaxis.set_major_formatter(ScalarFormatter())
+
+    if units[0] in ["Hz", "GHz"] and xlim is None:
+        ax1.invert_xaxis()
+
+        if filters is not None:
+            ax2.invert_xaxis()
+
+        if residuals is not None:
+            ax3.invert_xaxis()
+
+    if xlim is None:
+        xlim = ax1.get_xlim()
+    else:
+        ax1.set_xlim(xlim[0], xlim[1])
 
-        if ax2 is not None:
-            ax2.xaxis.set_major_formatter(ScalarFormatter())
+    if filters is not None:
+        ax2.set_xlim(xlim[0], xlim[1])
+        ax2.set_ylim(0.0, 1.0)
 
-        if ax3 is not None:
-            ax3.xaxis.set_major_formatter(ScalarFormatter())
+    if residuals is not None:
+        ax3.set_xlim(xlim[0], xlim[1])
 
     # if scale[1] == "log":
     #     ax1.yaxis.set_major_locator()
 
     # filters = ['Paranal/SPHERE.ZIMPOL_N_Ha',
     #            'MUSE/Hbeta',
     #            'ALMA/855']
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `species-0.8.0/species/read/read_calibration.py` & `species-0.8.1/species/read/read_calibration.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/read/read_color.py` & `species-0.8.1/species/read/read_color.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,16 +229,14 @@
                 filter_mag=self.filter_mag,
                 color=color[indices],
                 magnitude=mag[indices],
                 sptype=sptype[indices],
                 names=obj_names[indices],
             )
 
-            n_objects = sptype[indices].size 
-
         elif self.lib_type == "spec_lib":
             read_spec_0 = ReadSpectrum(
                 spec_library=self.library, filter_name=self.filters_color[0]
             )
 
             read_spec_1 = ReadSpectrum(
                 spec_library=self.library, filter_name=self.filters_color[1]
@@ -260,15 +258,15 @@
                 filter_mag=self.filter_mag,
                 color=phot_box_0.app_mag[:, 0] - phot_box_1.app_mag[:, 0],
                 magnitude=phot_box_2.abs_mag[:, 0],
                 sptype=phot_box_0.sptype,
                 names=None,
             )
 
-        n_objects = colormag_box.sptype.size
+        n_objects = len(colormag_box.sptype)
         print(f"Returning ColorMagBox with {n_objects} objects")
 
         return colormag_box
 
 
 class ReadColorColor:
     """
@@ -443,11 +441,11 @@
                 filters=self.filters_colors,
                 color1=phot_box_0.app_mag[:, 0] - phot_box_1.app_mag[:, 0],
                 color2=phot_box_2.app_mag[:, 0] - phot_box_3.app_mag[:, 0],
                 sptype=phot_box_0.sptype,
                 names=None,
             )
 
-        n_objects = colorbox.sptype.size
+        n_objects = len(colorbox.sptype)
         print(f"Returning ColorColorBox with {n_objects} objects")
 
         return colorbox
```

### Comparing `species-0.8.0/species/read/read_filter.py` & `species-0.8.1/species/read/read_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,25 @@
 
         config = ConfigParser()
         config.read(config_file)
 
         self.database = config["species"]["database"]
         self.data_folder = config["species"]["data_folder"]
 
-        with h5py.File(self.database, "a") as hdf5_file:
-            if f"filters/{self.filter_name}" not in hdf5_file:
+        with h5py.File(self.database, "r") as hdf5_file:
+            # Check if the filter is found in 'r' mode
+            # because the 'a' mode is not possible when
+            # using multiprocessing
+            if f"filters/{self.filter_name}" in hdf5_file:
+                filter_found = True
+            else:
+                filter_found = False
+
+        if not filter_found:
+            with h5py.File(self.database, "a") as hdf5_file:
                 add_filter_profile(self.data_folder, hdf5_file, self.filter_name)
 
     @typechecked
     def get_filter(self) -> np.ndarray:
         """
         Select a filter profile from the database.
```

### Comparing `species-0.8.0/species/read/read_isochrone.py` & `species-0.8.1/species/read/read_isochrone.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/read/read_model.py` & `species-0.8.1/species/read/read_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -916,14 +916,15 @@
         model_box = create_box(
             boxtype="model",
             model=self.model,
             wavelength=self.wl_points,
             flux=flux,
             parameters=model_param,
             quantity="flux",
+            spec_res=spec_res,
         )
 
         # Apply rotational broadening vsin(i) in km/s
 
         if "vsini" in model_param:
             spec_interp = interp1d(
                 model_box.wavelength, model_box.flux, bounds_error=False
@@ -1367,14 +1368,15 @@
         model_box = create_box(
             boxtype="model",
             model=self.model,
             wavelength=wl_points,
             flux=flux,
             parameters=model_param,
             quantity="flux",
+            spec_res=spec_res,
         )
 
         # Apply extinction
 
         if (
             "lognorm_radius" in model_param
             and "lognorm_sigma" in model_param
@@ -1858,14 +1860,15 @@
         model_box = create_box(
             boxtype="model",
             model=self.model,
             wavelength=model_box_0.wavelength,
             flux=flux_comb,
             parameters=model_param,
             quantity="flux",
+            spec_res=spec_res,
         )
 
         return model_box
 
     @typechecked
     def integrate_spectrum(self, model_param: Dict[str, float]) -> float:
         """
```

### Comparing `species-0.8.0/species/read/read_object.py` & `species-0.8.1/species/read/read_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,44 @@
             if f"objects/{self.object_name}" not in h5_file:
                 raise ValueError(
                     f"The object '{self.object_name}' is not "
                     f"present in the database."
                 )
 
     @typechecked
-    def list_filters(self) -> List[str]:
+    def list_filters(self, verbose=True) -> List[str]:
         """
         Function for listing and returning the filter profile names for
         which there is photometric data stored in the database.
 
+        Parameters
+        ----------
+        verbose : bool
+            Print the filter names if set to ``True``.
+
         Returns
         -------
         list(str)
             List with names of the filter profiles.
         """
 
         filter_list = []
 
-        print(f"Available photometric data for {self.object_name}:")
+        if verbose:
+            print(f"Available photometric data for {self.object_name}:")
 
         with h5py.File(self.database, "r") as h5_file:
             for tel_item in h5_file[f"objects/{self.object_name}"]:
                 if tel_item not in ["parallax", "distance", "spectrum"]:
                     for filt_item in h5_file[f"objects/{self.object_name}/{tel_item}"]:
-                        print(f"   - {tel_item}/{filt_item}")
                         filter_list.append(f"{tel_item}/{filt_item}")
 
+                        if verbose:
+                            print(f"   - {tel_item}/{filt_item}")
+
         return filter_list
 
     @typechecked
     def get_photometry(self, filter_name: str) -> np.ndarray:
         """
         Function for reading photometric data of the object
         for a specified filter name.
```

### Comparing `species-0.8.0/species/read/read_planck.py` & `species-0.8.1/species/read/read_planck.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/read/read_radtrans.py` & `species-0.8.1/species/read/read_radtrans.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,35 +629,36 @@
                 c_o_ratio,
             )
 
         elif "tint" in model_param and "log_delta" in model_param:
             tau = self.pressure * 1e6 * 10.0 ** model_param["log_delta"]
             temp = (0.75 * model_param["tint"] ** 4.0 * (2.0 / 3.0 + tau)) ** 0.25
 
-        elif (
-            "PTslope_1" in model_param
-        ):
-            num_layer = 6 # could make a variable in the future
+        elif "PTslope_1" in model_param:
+            num_layer = 6  # could make a variable in the future
             layer_pt_slopes = np.ones(num_layer) * np.nan
             for index in range(num_layer):
-                layer_pt_slopes[index] = model_param[f'PTslope_{num_layer - index}']
+                layer_pt_slopes[index] = model_param[f"PTslope_{num_layer - index}"]
 
             try:
                 from petitRADTRANS.physics import dTdP_temperature_profile
-            except ImportError as e:
+            except ImportError as import_error:
                 raise ImportError(
-                    """Can\'t import the dTdP profile function from petitRADTRANS,
-                    check that your version of pRT includes this function in   
-                    petitRADTRANS.physics""", e
+                    "Can't import the dTdP profile function from "
+                    "petitRADTRANS, check that your version of pRT "
+                    "includes this function in petitRADTRANS.physics",
+                    import_error,
                 )
 
-            temp = dTdP_temperature_profile(self.pressure,
-                                            num_layer, # could change in the future
-                                            layer_pt_slopes,
-                                            model_param["T_bottom"])
+            temp = dTdP_temperature_profile(
+                self.pressure,
+                num_layer,  # could change in the future
+                layer_pt_slopes,
+                model_param["T_bottom"],
+            )
 
         else:
             if temp_nodes is None:
                 temp_nodes = 0
 
                 for temp_idx in range(100):
                     if f"t{temp_idx}" in model_param:
```

### Comparing `species-0.8.0/species/read/read_spectrum.py` & `species-0.8.1/species/read/read_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/util/box_util.py` & `species-0.8.1/species/util/box_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import numpy as np
 
 from typeguard import typechecked
 
 from species.core import constants
 from species.core.box import ObjectBox
 from species.read.read_model import ReadModel
+from species.util.core_util import print_section
 
 
 @typechecked
 def update_objectbox(
     objectbox: ObjectBox, model_param: Dict[str, float], model: Optional[str] = None
 ) -> ObjectBox:
     """
@@ -42,14 +43,16 @@
     Returns
     -------
     species.core.box.ObjectBox
         The input box which includes the spectra with the
         scaled fluxes and/or inflated errors.
     """
 
+    print_section("Update ObjectBox")
+
     if objectbox.flux is not None:
         for key, value in objectbox.flux.items():
             instr_name = key.split(".")[0]
 
             if f"{key}_error" in model_param:
                 # Inflate the photometric uncertainty of a filter
 
@@ -102,15 +105,15 @@
                 spec_tmp[:, 1] *= model_param[f"scaling_{key}"]
                 print(" [DONE]")
 
             if f"error_{key}" in model_param:
                 if model is None:
                     warnings.warn(
                         "The dictionary with model parameters "
-                        f"contains the error inflation for {key} "
+                        f"contains the error inflation for '{key}' "
                         "but the argument of 'model' is set to "
                         "'None'. Inflation of the errors is "
                         "therefore not possible."
                     )
 
                 elif model == "petitradtrans":
                     # Increase the errors by a constant value
```

### Comparing `species-0.8.0/species/util/convert_util.py` & `species-0.8.1/species/util/convert_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/util/core_util.py` & `species-0.8.1/species/util/core_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/util/data_util.py` & `species-0.8.1/species/util/data_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Utility functions for data processing.
 """
 
 import os
 import tarfile
+import warnings
 
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import h5py
 import numpy as np
 
@@ -59,15 +60,14 @@
         @typechecked
         def safe_extract(
             tar: tarfile.TarFile,
             path: str = ".",
             member_list: Optional[List] = None,
             numeric_owner: bool = False,
         ) -> None:
-
             for member in member_list:
                 member_path = Path(path) / Path(member.name)
 
                 if not is_within_directory(path, str(member_path)):
                     raise Exception("Attempted path traversal in TAR file")
 
             tar.extractall(path, members=member_list, numeric_owner=numeric_owner)
@@ -470,19 +470,21 @@
                     elif np.isinf(np.sum(flux[i, j, ...])):
                         flux[i, j, :] = flux_int[count, :]
                         count_interp += 1
 
                     count += 1
 
             if count_missing > 0:
-                print(
-                    f"Could not interpolate {count_missing} grid points so storing "
-                    f"zeros instead. [WARNING]\nThe grid points that are missing:"
+                warnings.warn(
+                    f"Could not interpolate {count_missing} grid "
+                    "points so storing zeros instead."
                 )
 
+                print("\nThe following grid points are missing:")
+
                 for i in range(flux_int.shape[0]):
                     if np.isnan(np.sum(flux_int[i, :])):
                         print("   - ", end="")
                         print(f"{parameters[0]} = {new_points[0][i]}, ", end="")
                         print(f"{parameters[1]} = {new_points[1][i]}")
 
     elif len(parameters) == 3:
@@ -557,19 +559,21 @@
                         elif np.isinf(np.sum(flux[i, j, k, ...])):
                             flux[i, j, k, :] = flux_int[count, :]
                             count_interp += 1
 
                         count += 1
 
             if count_missing > 0:
-                print(
-                    f"Could not interpolate {count_missing} grid points so storing "
-                    f"zeros instead. [WARNING]\nThe grid points that are missing:"
+                warnings.warn(
+                    f"Could not interpolate {count_missing} grid "
+                    "points so storing zeros instead."
                 )
 
+                print("\nThe following grid points are missing:")
+
                 for i in range(flux_int.shape[0]):
                     if np.isnan(np.sum(flux_int[i, :])):
                         print("   - ", end="")
                         print(f"{parameters[0]} = {new_points[0][i]}, ", end="")
                         print(f"{parameters[1]} = {new_points[1][i]}, ", end="")
                         print(f"{parameters[2]} = {new_points[2][i]}")
 
@@ -650,19 +654,21 @@
                             elif np.isinf(np.sum(flux[i, j, k, m, ...])):
                                 flux[i, j, k, m, :] = flux_int[count, :]
                                 count_interp += 1
 
                             count += 1
 
             if count_missing > 0:
-                print(
-                    f"Could not interpolate {count_missing} grid points so storing "
-                    f"zeros instead. [WARNING]\nThe grid points that are missing:"
+                warnings.warn(
+                    f"Could not interpolate {count_missing} grid "
+                    "points so storing zeros instead."
                 )
 
+                print("\nThe following grid points are missing:")
+
                 for i in range(flux_int.shape[0]):
                     if np.isnan(np.sum(flux_int[i, :])):
                         print("   - ", end="")
                         print(f"{parameters[0]} = {new_points[0][i]}, ", end="")
                         print(f"{parameters[1]} = {new_points[1][i]}, ", end="")
                         print(f"{parameters[2]} = {new_points[2][i]}, ", end="")
                         print(f"{parameters[3]} = {new_points[3][i]}")
@@ -778,19 +784,21 @@
                                 elif np.isinf(np.sum(flux[i, j, k, m, n, ...])):
                                     flux[i, j, k, m, n, :] = flux_int[count, :]
                                     count_interp += 1
 
                                 count += 1
 
             if count_missing > 0:
-                print(
-                    f"Could not interpolate {count_missing} grid points so storing "
-                    f"zeros instead. [WARNING]\nThe grid points that are missing:"
+                warnings.warn(
+                    f"Could not interpolate {count_missing} grid "
+                    "points so storing zeros instead."
                 )
 
+                print("\nThe following grid points are missing:")
+
                 for i in range(flux_int.shape[0]):
                     if np.isnan(np.sum(flux_int[i, :])):
                         print("   - ", end="")
                         print(f"{parameters[0]} = {new_points[0][i]}, ", end="")
                         print(f"{parameters[1]} = {new_points[1][i]}, ", end="")
                         print(f"{parameters[2]} = {new_points[2][i]}, ", end="")
                         print(f"{parameters[3]} = {new_points[3][i]}, ", end="")
@@ -837,114 +845,221 @@
             if i == j:
                 assert cor_matrix[i, j] == 1.0
 
     return cov_matrix
 
 
 @typechecked
-def convert_units(flux_in: np.ndarray, units_in: Tuple[str, str]) -> np.ndarray:
+def convert_units(
+    flux_in: np.ndarray, units_in: Tuple[str, str], convert_from: bool = True
+) -> np.ndarray:
     """
-    Function for converting the wavelength units to
-    :math:`\\mu\\text{m}^{-1}` and the flux units to
+    Function for converting the wavelength units to or from
+    :math:`\\mu\\text{m}^{-1}` and the flux units to or from
     :math:`\\text{W} \\text{m}^{-2} \\mu\\text{m}^{-1}`.
 
     Parameters
     ----------
     flux_in : np.ndarray
         Array with the input wavelengths and fluxes. The shape of the
-        array should be (n_wavelengths, 3) with the columns being
-        the wavelengths, flux densities, and uncertainties. For
-        photometric fluxes, the array should also be 2D but with
-        a single row/wavelength.
+        array should be (n_wavelengths, 3) or (n_wavelengths, 2) with
+        the columns being the wavelengths, flux densities, and
+        optionally the uncertainties. For photometric fluxes, the
+        array should also be 2D but with a single row/wavelength.
     units_in : tuple(str, str)
-        Tuple with the units of the wavelength ("um", "angstrom", "A",
-        "nm", "mm", "cm", "m", "Hz") and the units of the flux density
-        ("W m-2 um-1", "W m-2 m-1", "W m-2 Hz-1", "erg s-1 cm-2 Hz-1",
-        "mJy", "Jy", "MJy").
+        Tuple with the units of the wavelength ("um", "angstrom",
+        "nm", "mm", "cm", "m", "Hz", "GHz") and the units of the
+        flux density ("W m-2 um-1", "W m-2 m-1", "W m-2 Hz-1",
+        "erg s-1 cm-2 angstrom-1" "erg s-1 cm-2 Hz-1", "mJy",
+        "Jy", "MJy"). One can use "um" or "µm" interchangeably,
+        and similarly "AA", "Å", "A", or "angstrom".
+    convert_from : bool
+        Convert from ``units_in`` to :math:`\\mu\\text{m}^{-1}` and
+        :math:`\\text{W} \\text{m}^{-2} \\mu\\text{m}^{-1}` when set to
+        ``True``. Or, convert to ``units_in`` when set to ``False``.
 
     Returns
     -------
     np.ndarray
         Array with the output in the same shape as ``flux_in``.
     """
 
     speed_light = constants.LIGHT * 1e6  # (um s-1)
 
     flux_out = np.zeros(flux_in.shape)
 
     # Convert wavelengths to micrometer (um)
 
-    wavel_units = ["um", "angstrom", "A", "nm", "mm", "cm", "m", "Hz"]
+    wavel_units = ["um", "angstrom", "nm", "mm", "cm", "m", "Hz", "GHz"]
 
-    if units_in[0] == "um":
+    if units_in[0] in ["um", "µm"]:
         flux_out[:, 0] = flux_in[:, 0].copy()
 
-    elif units_in[0] in ["angstrom", "A"]:
-        flux_out[:, 0] = flux_in[:, 0] * 1e-4
+    elif units_in[0] in ["angstrom", "A", "AA", "Å"]:
+        if convert_from:
+            flux_out[:, 0] = flux_in[:, 0] * 1e-4
+        else:
+            flux_out[:, 0] = flux_in[:, 0] * 1e4
 
     elif units_in[0] == "nm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e-3
+        if convert_from:
+            flux_out[:, 0] = flux_in[:, 0] * 1e-3
+        else:
+            flux_out[:, 0] = flux_in[:, 0] * 1e3
 
     elif units_in[0] == "mm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e3
+        if convert_from:
+            flux_out[:, 0] = flux_in[:, 0] * 1e3
+        else:
+            flux_out[:, 0] = flux_in[:, 0] * 1e-3
 
     elif units_in[0] == "cm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e4
+        if convert_from:
+            flux_out[:, 0] = flux_in[:, 0] * 1e4
+        else:
+            flux_out[:, 0] = flux_in[:, 0] * 1e-4
 
     elif units_in[0] == "m":
-        flux_out[:, 0] = flux_in[:, 0] * 1e6
+        if convert_from:
+            flux_out[:, 0] = flux_in[:, 0] * 1e6
+        else:
+            flux_out[:, 0] = flux_in[:, 0] * 1e-6
 
     elif units_in[0] == "Hz":
-        flux_out[:, 0] = speed_light / flux_in[:, 0]
+        if convert_from:
+            flux_out[:, 0] = speed_light / flux_in[:, 0]
+        else:
+            flux_out[:, 0] = speed_light / flux_in[:, 0]
+
+    elif units_in[0] == "GHz":
+        if convert_from:
+            flux_out[:, 0] = speed_light / (1e9 * flux_in[:, 0])
+        else:
+            flux_out[:, 0] = 1e-9 * speed_light / flux_in[:, 0]
 
     else:
         raise ValueError(
             f"The wavelength units '{units_in[0]}' are not supported. "
             f"Please choose from the following units: {wavel_units}"
         )
 
+    # Set wavelengths in micrometer
+
+    if convert_from:
+        wavel_micron = flux_out[:, 0].copy()
+    else:
+        wavel_micron = flux_in[:, 0].copy()
+
     # Convert flux density to W m-2 um-1
 
     flux_units = [
         "W m-2 um-1",
         "W m-2 m-1",
         "W m-2 Hz-1",
+        "erg s-1 cm-2 angstrom-1",
         "erg s-1 cm-2 Hz-1",
         "mJy",
         "Jy",
         "MJy",
     ]
 
-    if units_in[1] == "W m-2 um-1":
+    if units_in[1] in ["W m-2 um-1", "W m-2 µm-1"]:
         flux_out[:, 1] = flux_in[:, 1].copy()
-        flux_out[:, 2] = flux_in[:, 2].copy()
+
+        if flux_out.shape[1] == 3:
+            flux_out[:, 2] = flux_in[:, 2].copy()
 
     elif units_in[1] == "W m-2 m-1":
-        flux_out[:, 1] = flux_in[:, 1] * 1e-6
-        flux_out[:, 2] = flux_in[:, 2] * 1e-6
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-6
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e6
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-6
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e6
 
     elif units_in[1] == "W m-2 Hz-1":
-        flux_out[:, 1] = flux_in[:, 1] * speed_light / flux_out[:, 0] ** 2
-        flux_out[:, 2] = flux_in[:, 2] * speed_light / flux_out[:, 0] ** 2
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * speed_light / wavel_micron**2
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * wavel_micron**2 / speed_light
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * speed_light / wavel_micron**2
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * wavel_micron**2 / speed_light
 
     elif units_in[1] == "erg s-1 cm-2 Hz-1":
-        flux_out[:, 1] = flux_in[:, 1] * 1e-3 * speed_light / flux_out[:, 0] ** 2
-        flux_out[:, 2] = flux_in[:, 2] * 1e-3 * speed_light / flux_out[:, 0] ** 2
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-3 * speed_light / wavel_micron**2
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e3 * wavel_micron**2 / speed_light
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-3 * speed_light / wavel_micron**2
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e3 * wavel_micron**2 / speed_light
+
+    elif units_in[1] in [
+        "erg s-1 cm-2 angstrom-1",
+        "erg s-1 cm-2 A-1",
+        "erg s-1 cm-2 AA-1",
+        "erg s-1 cm-2 Å-1",
+    ]:
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-1
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e1
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-1
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e1
 
     elif units_in[1] == "mJy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e-29 * speed_light / flux_out[:, 0] ** 2
-        flux_out[:, 2] = flux_in[:, 2] * 1e-29 * speed_light / flux_out[:, 0] ** 2
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-29 * speed_light / wavel_micron**2
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e29 * wavel_micron**2 / speed_light
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-29 * speed_light / wavel_micron**2
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e29 * wavel_micron**2 / speed_light
 
     elif units_in[1] == "Jy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e-26 * speed_light / flux_out[:, 0] ** 2
-        flux_out[:, 2] = flux_in[:, 2] * 1e-26 * speed_light / flux_out[:, 0] ** 2
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-26 * speed_light / wavel_micron**2
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e26 * wavel_micron**2 / speed_light
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-26 * speed_light / wavel_micron**2
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e26 * wavel_micron**2 / speed_light
 
     elif units_in[1] == "MJy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e-20 * speed_light / flux_out[:, 0] ** 2
-        flux_out[:, 2] = flux_in[:, 2] * 1e-20 * speed_light / flux_out[:, 0] ** 2
+        if convert_from:
+            flux_out[:, 1] = flux_in[:, 1] * 1e-20 * speed_light / wavel_micron**2
+        else:
+            flux_out[:, 1] = flux_in[:, 1] * 1e20 * wavel_micron**2 / speed_light
+
+        if flux_out.shape[1] == 3:
+            if convert_from:
+                flux_out[:, 2] = flux_in[:, 2] * 1e-20 * speed_light / wavel_micron**2
+            else:
+                flux_out[:, 2] = flux_in[:, 2] * 1e20 * wavel_micron**2 / speed_light
 
     else:
         raise ValueError(
             f"The flux units '{units_in[1]}' are not supported. "
             f"Please choose from the following units: {flux_units}"
         )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `species-0.8.0/species/util/dust_util.py` & `species-0.8.1/species/util/dust_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     with h5py.File(database_path, "a") as hdf5_file:
         if "dust" not in hdf5_file:
             add_optical_constants(data_folder, hdf5_file)
             add_cross_sections(data_folder, hdf5_file)
 
     return database_path
 
+
 @typechecked
 def log_normal_distribution(
     radius_g: float, sigma_g: float, n_bins: int
 ) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
     """
     Function for returning a log-normal size distribution. See Eq. 9
     in Ackerman & Marley (2001).
```

### Comparing `species-0.8.0/species/util/fit_util.py` & `species-0.8.1/species/util/fit_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,14 @@
     print("\nParameters:")
     for key, value in parameters.items():
         if key == "luminosity":
             print(f"   - {key} = {value:.2e}")
         else:
             print(f"   - {key} = {value:.2f}")
 
-
     if inc_phot and objectbox.filters is not None:
         if isinstance(inc_phot, bool) and inc_phot:
             inc_phot = objectbox.filters
 
         model_phot = multi_photometry(
             datatype=datatype,
             spectrum=spectrum,
```

### Comparing `species-0.8.0/species/util/model_util.py` & `species-0.8.1/species/util/model_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 
     elif in_name == "exo-rem":
         out_name = "Exo-REM"
 
     elif in_name == "exo-rem-highres":
         out_name = "Exo-REM"
 
-    elif in_name == "planck":
+    elif in_name in ["planck", "blackbody"]:
         out_name = "Blackbody"
 
     elif in_name == "zhu2015":
         out_name = "Zhu (2015)"
 
     elif in_name == "saumon2008-clear":
         out_name = "Saumon & Marley (2008)"
@@ -119,14 +119,23 @@
 
     elif in_name == "sonora-bobcat":
         out_name = "Sonora Bobcat"
 
     elif in_name == "sonora-bobcat-co":
         out_name = "Sonora Bobcat C/O"
 
+    elif in_name == "sonora-elfowl-l":
+        out_name = "Sonora Elf Owl"
+
+    elif in_name == "sonora-elfowl-t":
+        out_name = "Sonora Elf Owl"
+
+    elif in_name == "sonora-elfowl-y":
+        out_name = "Sonora Elf Owl"
+
     elif in_name == "sphinx":
         out_name = "SPHINX"
 
     elif in_name == "petitradtrans":
         out_name = "petitRADTRANS"
 
     else:
```

### Comparing `species-0.8.0/species/util/plot_util.py` & `species-0.8.1/species/util/plot_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -197,15 +197,15 @@
 
     Returns
     -------
     list
         List with parameter labels for plots.
     """
 
-    cloud_species = ["fe", "mgsio3", "al2o3", "na2s", "kcl"]
+    cloud_species = ["Fe", "MgSiO3", "Al2O3", "Na2S", "KCl"]
 
     cloud_labels = ["Fe", r"MgSiO_{3}", r"Al_{2}O_{3}", r"Na_{2}S", "KCl"]
 
     abund_species = [
         "CO_all_iso",
         "CO_all_iso_HITEMP",
         "H2O",
@@ -477,15 +477,18 @@
 
     if "luminosity_ratio" in param:
         index = param.index("luminosity_ratio")
         param[index] = r"$\log\,L_\mathrm{1}/L_\mathrm{2}$"
 
     if "luminosity_disk_planet" in param:
         index = param.index("luminosity_disk_planet")
-        param[index] = r"$L_\mathrm{disk}/L_\mathrm{atm}$"
+        if object_type == "planet":
+            param[index] = r"$L_\mathrm{disk}/L_\mathrm{atm}$"
+        elif object_type == "star":
+            param[index] = r"$L_\mathrm{disk}/L_\ast$"
 
     if "lognorm_radius" in param:
         index = param.index("lognorm_radius")
         param[index] = r"$\log\,r_\mathrm{g}$"
 
     if "lognorm_sigma" in param:
         index = param.index("lognorm_sigma")
@@ -571,32 +574,36 @@
 
     if "kzz" in param:
         # Backward compatibility
         index = param.index("kzz")
         param[index] = r"$\log\,K_\mathrm{zz}$"
 
     for i, item in enumerate(cloud_species):
-        if f"{item}_fraction" in param:
-            index = param.index(f"{item}_fraction")
+        if f"{item.lower()}_fraction" in param:
+            index = param.index(f"{item.lower()}_fraction")
             param[
                 index
             ] = rf"$\log\,\tilde{{\mathrm{{X}}}}_\mathrm{{{cloud_labels[i]}}}$"
 
-        if f"{item}_tau" in param:
-            index = param.index(f"{item}_tau")
+        if f"{item.lower()}_tau" in param:
+            index = param.index(f"{item.lower()}_tau")
             param[index] = rf"$\bar{{\tau}}_\mathrm{{{cloud_labels[i]}}}$"
 
-        if f"log_p_base_{item}" in param:
-            index = param.index(f"log_p_base_{item}")
+        if f"log_p_base_{item}(c)" in param:
+            index = param.index(f"log_p_base_{item}(c)")
+            param[index] = rf"$\log\,P_\mathrm{{{cloud_labels[i]}}}$"
+
+        if f"fsed_{item}(c)" in param:
+            index = param.index(f"fsed_{item}(c)")
             param[index] = rf"$\log\,P_\mathrm{{{cloud_labels[i]}}}$"
 
     for i, item_i in enumerate(cloud_species):
         for j, item_j in enumerate(cloud_species):
-            if f"{item_i}_{item_j}_ratio" in param:
-                index = param.index(f"{item_i}_{item_j}_ratio")
+            if f"{item_i.lower()}_{item_j.lower()}_ratio" in param:
+                index = param.index(f"{item_i.lower()}_{item_j.lower()}_ratio")
                 param[index] = (
                     rf"$\log\,\tilde{{\mathrm{{X}}}}"
                     rf"_\mathrm{{{cloud_labels[i]}}}/"
                     rf"\mathrm{{\tilde{{X}}}}_\mathrm{{{cloud_labels[j]}}}$"
                 )
 
     for i, item in enumerate(abund_species):
@@ -681,15 +688,25 @@
 
     if "disk_teff" in param:
         index = param.index("disk_teff")
         param[index] = r"$T_\mathrm{disk}$ (K)"
 
     if "disk_radius" in param:
         index = param.index("disk_radius")
-        param[index] = r"$R_\mathrm{disk}$ ($R_\mathrm{J}$)"
+        if object_type == "planet":
+            param[index] = r"$R_\mathrm{disk}$ ($R_\mathrm{J}$)"
+        elif object_type == "star":
+            param[index] = r"$R_\mathrm{disk}$ (au)"
+
+    if "radius_bb" in param:
+        index = param.index("radius_bb")
+        if object_type == "planet":
+            param[index] = r"$R_\mathrm{bb}$ ($R_\mathrm{J}$)"
+        elif object_type == "star":
+            param[index] = r"$R_\mathrm{bb}$ (au)"
 
     if "log_powerlaw_a" in param:
         index = param.index("log_powerlaw_a")
         param[index] = r"$a_\mathrm{powerlaw}$"
 
     if "log_powerlaw_b" in param:
         index = param.index("log_powerlaw_b")
@@ -918,14 +935,19 @@
             label.append(r"$f_\mathrm{sed}$")
 
         if item == "c_o_ratio":
             quantity.append("c_o_ratio")
             unit.append(None)
             label.append("C/O")
 
+        if item == "log_kzz":
+            quantity.append("log_kzz")
+            unit.append(None)
+            label.append(r"$\log\,K_\mathrm{zz}$")
+
         if item == "ad_index":
             quantity.append("ad_index")
             unit.append(None)
             label.append(r"$\gamma_\mathrm{ad}$")
 
         if item == "radius":
             quantity.append("radius")
@@ -1022,16 +1044,19 @@
         if item == "disk_teff":
             quantity.append("disk_teff")
             unit.append("K")
             label.append(r"$T_\mathrm{disk}$")
 
         if item == "disk_radius":
             quantity.append("disk_radius")
-            unit.append(r"$R_\mathrm{J}$")
             label.append(r"$R_\mathrm{disk}$")
+            if object_type == "planet":
+                unit.append(r"$R_\mathrm{J}$")
+            elif object_type == "star":
+                unit.append("au")
 
         if item == "flux_scaling":
             quantity.append("flux_scaling")
             unit.append(None)
             label.append(r"$a_\mathrm{flux}$")
 
         if item == "log_flux_scaling":
@@ -1337,19 +1362,22 @@
     #     model_data = json.load(json_file)
     #     model_list = list(model_data.keys())
 
     # Do not include these parameters by default in the legend
 
     not_default = ["distance", "parallax", "mass", "luminosity"]
 
+    # Use the model parameters if leg_param is empty
+
     if len(leg_param) == 0:
         leg_param = list(model_param.keys())
 
         for param_item in not_default:
             if param_item in leg_param:
+                # Do not include the not_default parameters
                 leg_param.remove(param_item)
 
     # Remove parameters from the model_param dictionary
     # if they are not included in the leg_param list
 
     del_keys = []
     for param_item in model_param.keys():
@@ -1374,24 +1402,36 @@
 
     if model_name is not None and inc_model_name:
         label += convert_model_name(model_name)
 
         if len(par_key) > 0:
             label += ": "
 
-    for i, item in enumerate(par_key):
+    for item in leg_param:
+        if item in par_key:
+            param_idx = par_key.index(item)
+        else:
+            continue
+
         if item[:4] == "teff":
             value = f"{model_param[item]:{param_fmt['teff']}}"
 
         elif item[:6] == "radius":
             if object_type == "planet":
                 value = f"{model_param[item]:{param_fmt['radius']}}"
             elif object_type == "star":
                 value = f"{model_param[item]*constants.R_JUP/constants.R_SUN:{param_fmt['radius']}}"
 
+        elif item[:11] == "disk_radius":
+            if object_type == "planet":
+                value = f"{model_param[item]:{param_fmt['disk_radius']}}"
+            elif object_type == "star":
+                radius_au = model_param[item] * constants.R_JUP / constants.AU
+                value = f"{radius_au:{param_fmt['disk_radius']}}"
+
         elif item == "mass" and item in leg_param:
             if object_type == "planet":
                 value = f"{model_param[item]:{param_fmt['mass']}}"
             elif object_type == "star":
                 value = f"{model_param[item]*constants.M_JUP/constants.M_SUN:{param_fmt['mass']}}"
 
         elif item == "luminosity" and item in leg_param:
@@ -1411,131 +1451,20 @@
         else:
             continue
 
         # if len(label) > 80 and newline == False:
         #     label += '\n'
         #     newline = True
 
-        if par_unit[i] is None:
+        if par_unit[param_idx] is None:
             if len(label) > 0 and label[-2] != ":":
                 label += ", "
 
-            label += f"{par_label[i]} = {value}"
+            label += f"{par_label[param_idx]} = {value}"
 
         else:
             if len(label) > 0 and label[-2] != ":":
                 label += ", "
 
-            label += f"{par_label[i]} = {value} {par_unit[i]}"
+            label += f"{par_label[param_idx]} = {value} {par_unit[param_idx]}"
 
     return label
-
-
-@typechecked
-def convert_units_plot(flux_in: np.ndarray, units_out: Tuple[str, str]) -> np.ndarray:
-    """
-    Function for converting the wavelength units from
-    :math:`\\mu\\text{m}^{-1}` and the flux units from
-    :math:`\\text{W} \\text{m}^{-2} \\mu\\text{m}^{-1}`.
-
-    Parameters
-    ----------
-    flux_in : np.ndarray
-        Array with the input wavelengths and fluxes. The shape of the
-        array should be (n_wavelengths, 3) with the columns being
-        the wavelengths, flux densities, and uncertainties. For
-        photometric fluxes, the array should also be 2D but with
-        a single row/wavelength.
-    units_out : tuple(str, str)
-        Tuple with the units of the wavelength ("um", "angstrom", "A",
-        "nm", "mm", "cm", "m", "Hz") and the units of the flux density
-        ("W m-2 um-1", "W m-2 m-1", "W m-2 Hz-1", "erg s-1 cm-2 Hz-1",
-        "mJy", "Jy", "MJy").
-
-    Returns
-    -------
-    np.ndarray
-        Array with the output in the same shape as ``flux_in``.
-    """
-
-    speed_light = constants.LIGHT * 1e6  # (um s-1)
-
-    flux_out = np.zeros(flux_in.shape)
-
-    # Convert wavelengths from micrometer (um)
-
-    wavel_units = ["um", "angstrom", "A", "nm", "mm", "cm", "m", "Hz"]
-
-    if units_out[0] == "um":
-        flux_out[:, 0] = flux_in[:, 0].copy()
-
-    elif units_out[0] in ["angstrom", "A"]:
-        flux_out[:, 0] = flux_in[:, 0] * 1e4
-
-    elif units_out[0] == "nm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e3
-
-    elif units_out[0] == "mm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e-3
-
-    elif units_out[0] == "cm":
-        flux_out[:, 0] = flux_in[:, 0] * 1e-4
-
-    elif units_out[0] == "m":
-        flux_out[:, 0] = flux_in[:, 0] * 1e-6
-
-    elif units_out[0] == "Hz":
-        flux_out[:, 0] = speed_light / flux_in[:, 0]
-
-    else:
-        raise ValueError(
-            f"The wavelength units '{units_out[0]}' are not supported. "
-            f"Please choose from the following units: {wavel_units}"
-        )
-
-    # Convert flux density from W m-2 um-1
-
-    flux_units = [
-        "W m-2 um-1",
-        "W m-2 m-1",
-        "W m-2 Hz-1",
-        "erg s-1 cm-2 Hz-1",
-        "mJy",
-        "Jy",
-        "MJy",
-    ]
-
-    if units_out[1] == "W m-2 um-1":
-        flux_out[:, 1] = flux_in[:, 1].copy()
-        flux_out[:, 2] = flux_in[:, 2].copy()
-
-    elif units_out[1] == "W m-2 m-1":
-        flux_out[:, 1] = flux_in[:, 1] * 1e6
-        flux_out[:, 2] = flux_in[:, 2] * 1e6
-
-    elif units_out[1] == "W m-2 Hz-1":
-        flux_out[:, 1] = flux_in[:, 1] * flux_out[:, 0] ** 2 / speed_light
-        flux_out[:, 2] = flux_in[:, 2] * flux_out[:, 0] ** 2 / speed_light
-
-    elif units_out[1] == "erg s-1 cm-2 Hz-1":
-        flux_out[:, 1] = flux_in[:, 1] * 1e3 * flux_out[:, 0] ** 2 / speed_light
-        flux_out[:, 2] = flux_in[:, 2] * 1e3 * flux_out[:, 0] ** 2 / speed_light
-
-    elif units_out[1] == "mJy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e29 * flux_out[:, 0] ** 2 / speed_light
-        flux_out[:, 2] = flux_in[:, 2] * 1e29 * flux_out[:, 0] ** 2 / speed_light
-
-    elif units_out[1] == "Jy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e26 * flux_out[:, 0] ** 2 / speed_light
-        flux_out[:, 2] = flux_in[:, 2] * 1e26 * flux_out[:, 0] ** 2 / speed_light
-
-    elif units_out[1] == "MJy":
-        flux_out[:, 1] = flux_in[:, 1] * 1e20 * flux_out[:, 0] ** 2 / speed_light
-        flux_out[:, 2] = flux_in[:, 2] * 1e20 * flux_out[:, 0] ** 2 / speed_light
-
-    else:
-        raise ValueError(
-            f"The flux units '{units_out[1]}' are not supported. "
-            f"Please choose from the following units: {flux_units}"
-        )
-
-    return flux_out
```

### Comparing `species-0.8.0/species/util/query_util.py` & `species-0.8.1/species/util/query_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species/util/radtrans_util.py` & `species-0.8.1/species/util/radtrans_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,18 +107,20 @@
         model_param["t2"] = sample[indices["t2"]]
         model_param["t3"] = sample[indices["t3"]]
         model_param["log_delta"] = sample[indices["log_delta"]]
         model_param["alpha"] = sample[indices["alpha"]]
         model_param["tint"] = sample[indices["tint"]]
 
     elif pt_profile == "gradient":
-        num_layer = 6 # could make a variable in the future
+        num_layer = 6  # could make a variable in the future
         for index in range(num_layer):
-            model_param[f'PTslope_{num_layer - index}'] = sample[indices[f'PTslope_{num_layer - index}']]
-        model_param['T_bottom'] = sample[indices['T_bottom']]
+            model_param[f"PTslope_{num_layer - index}"] = sample[
+                indices[f"PTslope_{num_layer - index}"]
+            ]
+        model_param["T_bottom"] = sample[indices["T_bottom"]]
 
     elif pt_profile == "eddington":
         model_param["log_delta"] = sample[indices["log_delta"]]
         model_param["tint"] = sample[indices["tint"]]
 
     elif pt_profile in ["free", "monotonic"]:
         if temp_nodes is None:
```

### Comparing `species-0.8.0/species/util/retrieval_util.py` & `species-0.8.1/species/util/retrieval_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,25 +486,27 @@
             metallicity,
             c_o_ratio,
         )
 
     elif pt_profile == "gradient":
         num_layer = 6  # could make a variable in the future
         layer_pt_slopes = np.ones(num_layer) * np.nan
+
         for index in range(num_layer):
             layer_pt_slopes[index] = cube[cube_index[f"PTslope_{num_layer - index}"]]
 
         try:
             from petitRADTRANS.physics import dTdP_temperature_profile
-        except ImportError as e:
+
+        except ImportError as import_error:
             raise ImportError(
-                """Can\'t import the dTdP profile function from petitRADTRANS,
-                check that your version of pRT includes this function in   
-                petitRADTRANS.physics""",
-                e,
+                "Can't import the dTdP profile function from "
+                "petitRADTRANS, check that the version of pRT "
+                "includes this function in petitRADTRANS.physics",
+                import_error,
             )
 
         temp = dTdP_temperature_profile(
             pressure,
             num_layer,  # could change in the future
             layer_pt_slopes,
             cube[cube_index["T_bottom"]],
@@ -1204,18 +1206,22 @@
                     plotting=plotting,
                 )
 
             p_base[f"{cloud_item}(c)"] = p_base_item
 
             abund_in[f"{cloud_item}(c)"] = np.zeros_like(temperature)
 
+            if "fsed" in cloud_dict:
+                f_sed = cloud_dict["fsed"]
+            else:
+                f_sed = cloud_dict[f"fsed_{cloud_item}(c)"]
+
             abund_in[f"{cloud_item}(c)"][pressure < p_base_item] = (
                 10.0 ** log_x_base[cloud_item]
-                * (pressure[pressure <= p_base_item] / p_base_item)
-                ** cloud_dict["fsed"]
+                * (pressure[pressure <= p_base_item] / p_base_item) ** f_sed
             )
 
     # Adaptive pressure refinement around the cloud base
 
     if pressure_grid == "clouds":
         _, indices = make_half_pressure_better(p_base, pressure)
     else:
@@ -1231,20 +1237,22 @@
         indices=indices,
     )
 
     # Create dictionary with sedimentation parameters
     # Use the same value for all cloud species
 
     fseds = {}
-    for item in rt_object.cloud_species:
-        # The item has the form of e.g. MgSiO3(c)
-        # For parametrized cloud opacities,
-        # then number of cloud_species is zero
-        # so the fseds dictionary remains empty
-        fseds[item] = cloud_dict["fsed"]
+    for cloud_item in rt_object.cloud_species:
+        # The cloud_item has the form of e.g. MgSiO3(c). For
+        # parametrized cloud opacities, then the number of
+        # cloud_species is zero so the fseds dictionary is empty
+        if "fsed" in cloud_dict:
+            fseds[cloud_item] = cloud_dict["fsed"]
+        else:
+            fseds[cloud_item] = cloud_dict[f"fsed_{cloud_item}"]
 
     # Create an array with a constant eddy diffusion coefficient (cm2 s-1)
 
     if "log_kzz" in cloud_dict:
         Kzz_use = np.full(pressure.shape, 10.0 ** cloud_dict["log_kzz"])
     else:
         Kzz_use = None
@@ -1331,15 +1339,18 @@
             plt.axhline(p_base[f"{item}(c)"])
             plt.yscale("log")
             if np.count_nonzero(abundances[f"{item}(c)"]) > 0:
                 plt.xscale("log")
             plt.ylim(1e3, 1e-6)
             plt.xlim(1e-10, 1.0)
             log_x_base_item = log_x_base[item]
-            fsed = cloud_dict["fsed"]
+            if "fsed" in cloud_dict:
+                fsed = cloud_dict["fsed"]
+            else:
+                fsed = cloud_dict[f"fsed_{item}(c)"]
             log_kzz = cloud_dict["log_kzz"]
             plt.title(
                 f"fsed = {fsed:.2f}, log(Kzz) = {log_kzz:.2f}, "
                 + f"X_b = {log_x_base_item:.2f}"
             )
             plt.savefig(f"{item.lower()}_clouds.png", bbox_inches="tight")
             plt.clf()
@@ -2842,29 +2853,29 @@
 
     Returns
     -------
     np.ndarray
         Convolved spectrum.
     """
 
-    # delta lambda of resolution element is FWHM
-    # of the LSF's standard deviation, hence:
+    # delta_lambda of resolution element is
+    # FWHM of the LSF's standard deviation
     sigma_lsf = 1.0 / spec_res / (2.0 * np.sqrt(2.0 * np.log(2.0)))
 
     # The input spacing of petitRADTRANS is 1e3, but just compute
     # it to be sure, or more versatile in the future.
     # Also, we have a log-spaced grid, so the spacing is constant
     # as a function of wavelength
     spacing = np.mean(2.0 * np.diff(input_wavel) / (input_wavel[1:] + input_wavel[:-1]))
 
-    # Calculate the sigma to be used in the gauss filter in units
-    # of input wavelength bins
-    sigma_lsf_gauss_filter = sigma_lsf / spacing
+    # Calculate the sigma to be used with the Gaussian filter
+    # in units of the input wavelength bins
+    sigma_filter = sigma_lsf / spacing
 
-    return gaussian_filter(input_flux, sigma=sigma_lsf_gauss_filter, mode="nearest")
+    return gaussian_filter(input_flux, sigma=sigma_filter, mode="nearest")
 
 
 @typechecked
 def quench_pressure(
     pressure: np.ndarray,
     temperature: np.ndarray,
     metallicity: float,
```

### Comparing `species-0.8.0/species/util/spec_util.py` & `species-0.8.1/species/util/spec_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,32 +101,43 @@
 
         return np.asarray(kernel / sum(kernel))
 
     spacing = np.mean(2.0 * np.diff(wavelength) / (wavelength[1:] + wavelength[:-1]))
     spacing_std = np.std(2.0 * np.diff(wavelength) / (wavelength[1:] + wavelength[:-1]))
 
     if spacing_std / spacing < 1e-2 or force_smooth:
-        # see retrieval_util.convolve_spectrum
+        # delta_lambda of resolution element is
+        # FWHM of the LSF's standard deviation
         sigma_lsf = 1.0 / spec_res / (2.0 * np.sqrt(2.0 * np.log(2.0)))
-        flux_smooth = gaussian_filter(flux, sigma=sigma_lsf / spacing, mode="nearest")
+
+        # Calculate the sigma to be used with the Gaussian filter
+        # in units of the input wavelength bins
+        sigma_filter = sigma_lsf / spacing
+
+        flux_smooth = gaussian_filter(flux, sigma=sigma_filter, mode="nearest")
 
     else:
         if size % 2 == 0:
             raise ValueError("The kernel size should be an odd number.")
 
         flux_smooth = np.zeros(flux.shape)  # (W m-2 um-1)
 
         spacing = np.mean(np.diff(wavelength))  # (um)
         spacing_std = np.std(np.diff(wavelength))  # (um)
 
         if spacing_std / spacing > 1e-2:
             warnings.warn(
-                f"The wavelength spacing is not uniform ({spacing} +/- {spacing_std}). "
-                f"The smoothing with the Gaussian kernel requires either the spectral "
-                f"resolution or the wavelength spacing to be uniformly sampled."
+                "The wavelength spacing is not uniform "
+                f"(lambda/d_lambda = {spacing} +/- {spacing_std}). "
+                "The smoothing with the Gaussian kernel requires "
+                "either the spectral resolution or the wavelength "
+                "spacing to be uniformly sampled. This warning "
+                "should not have occurred with any of the model "
+                "grids provided by species. Please open an issue "
+                "on the Github page if help is needed."
             )
 
         for i, item in enumerate(wavelength):
             fwhm = item / spec_res  # (um)
             sigma = fwhm / (2.0 * np.sqrt(2.0 * np.log(2.0)))  # (um)
 
             size = int(
```

### Comparing `species-0.8.0/species/util/test_util.py` & `species-0.8.1/species/util/test_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.0/species.egg-info/PKG-INFO` & `species-0.8.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: species
-Version: 0.8.0
+Version: 0.8.1
 Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
 Home-page: https://github.com/tomasstolker/species
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://species.readthedocs.io
 Keywords: species
@@ -20,34 +20,17 @@
 License-File: LICENSE
 
 *species*
 =========
 
 **spe**\ctral **c**\ haracterization and **i**\ nference for **e**\ xoplanet **s**\ cience
 
-.. image:: https://img.shields.io/pypi/v/species
-   :target: https://pypi.python.org/pypi/species
-
-.. image:: https://img.shields.io/pypi/pyversions/species
-   :target: https://pypi.python.org/pypi/species
+.. container::
 
-.. image:: https://github.com/tomasstolker/species/workflows/CI/badge.svg?branch=main
-   :target: https://github.com/tomasstolker/species/actions
-
-.. image:: https://img.shields.io/readthedocs/species
-   :target: http://species.readthedocs.io
-
-.. image:: https://codecov.io/gh/tomasstolker/species/branch/main/graph/badge.svg?token=LSSCPMJ5JH
-   :target: https://codecov.io/gh/tomasstolker/species
-
-.. image:: https://img.shields.io/codefactor/grade/github/tomasstolker/species
-   :target: https://www.codefactor.io/repository/github/tomasstolker/species
-
-.. image:: https://img.shields.io/github/license/tomasstolker/species
-   :target: https://github.com/tomasstolker/species/blob/main/LICENSE
+    |PyPI Status| |Python Versions| |CI Status| |Docs Status| |Code Coverage| |Code Quality| |License|
 
 *species* is a toolkit for atmospheric characterization of directly imaged exoplanets. It provides a coherent framework for spectral and photometric analysis which builds on publicly-available data and models from various resources.
 
 There are tools available for grid and free retrievals using Bayesian inference, synthetic photometry, interpolating a variety atmospheric and evolutionary model grids (including the possibility to add a custom grid), color-magnitude and color-color diagrams, empirical spectral analysis, spectral and photometric calibration, and analysis of emission lines. The package has been released on `PyPI <https://pypi.org/project/species/>`_ and is actively developed and maintained on `Github <https://github.com/tomasstolker/species>`_.
 
 **Important:** Importing the *species* package had become slow because of the many classes and functions that were implicitly imported. The initialization of the package has therefore been adjusted. Any functionalities should now be explicitly imported from the modules that they are part of.
 
@@ -73,7 +56,28 @@
 
 License
 -------
 
 Copyright 2018-2024 Tomas Stolker
 
 *species* is distributed under the MIT License. See `LICENSE <https://github.com/tomasstolker/species/blob/main/LICENSE>`_ for the terms and conditions.
+
+.. |PyPI Status| image:: https://img.shields.io/pypi/v/species
+   :target: https://pypi.python.org/pypi/species
+
+.. |Python Versions| image:: https://img.shields.io/pypi/pyversions/species
+   :target: https://pypi.python.org/pypi/species
+
+.. |CI Status| image:: https://github.com/tomasstolker/species/workflows/CI/badge.svg?branch=main
+   :target: https://github.com/tomasstolker/species/actions
+
+.. |Docs Status| image:: https://img.shields.io/readthedocs/species
+   :target: http://species.readthedocs.io
+
+.. |Code Coverage| image:: https://codecov.io/gh/tomasstolker/species/branch/main/graph/badge.svg?token=LSSCPMJ5JH
+   :target: https://codecov.io/gh/tomasstolker/species
+
+.. |Code Quality| image:: https://img.shields.io/codefactor/grade/github/tomasstolker/species
+   :target: https://www.codefactor.io/repository/github/tomasstolker/species
+
+.. |License| image:: https://img.shields.io/github/license/tomasstolker/species
+   :target: https://github.com/tomasstolker/species/blob/main/LICENSE
```

### Comparing `species-0.8.0/species.egg-info/SOURCES.txt` & `species-0.8.1/species.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 species/core/__init__.py
 species/core/box.py
 species/core/constants.py
 species/core/species_init.py
 species/data/__init__.py
 species/data/database.py
 species/data/companion_data/__init__.py
+species/data/companion_data/companion_data.json
+species/data/companion_data/companion_spectra.json
 species/data/companion_data/companion_spectra.py
 species/data/filter_data/__init__.py
 species/data/filter_data/filter_data.py
 species/data/isochrone_data/__init__.py
 species/data/isochrone_data/add_isochrone.py
 species/data/isochrone_data/iso_ames.py
 species/data/isochrone_data/iso_atmo.py
```

