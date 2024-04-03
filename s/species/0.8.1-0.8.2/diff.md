# Comparing `tmp/species-0.8.1.tar.gz` & `tmp/species-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "species-0.8.1.tar", last modified: Wed Apr  3 20:09:49 2024, max compression
+gzip compressed data, was "species-0.8.2.tar", last modified: Wed Apr  3 20:50:00 2024, max compression
```

## Comparing `species-0.8.1.tar` & `species-0.8.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.604846 species-0.8.1/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2023-09-26 09:49:21.000000 species-0.8.1/LICENSE
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:09:49.604680 species-0.8.1/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3513 2024-04-03 18:12:34.000000 species-0.8.1/README.rst
--rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2024-04-03 20:09:49.604894 species-0.8.1/setup.cfg
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1339 2024-04-03 18:22:51.000000 species-0.8.1/setup.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.567799 species-0.8.1/species/
--rw-r--r--   0 tomasstolker   (501) staff       (20)      223 2024-04-03 18:22:47.000000 species-0.8.1/species/__init__.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.569615 species-0.8.1/species/core/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/core/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15235 2024-03-26 09:45:01.000000 species-0.8.1/species/core/box.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      880 2023-11-08 06:43:57.000000 species-0.8.1/species/core/constants.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4863 2024-03-30 11:12:28.000000 species-0.8.1/species/core/species_init.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.570254 species-0.8.1/species/data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)       23 2023-11-08 20:53:44.000000 species-0.8.1/species/data/__init__.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.573613 species-0.8.1/species/data/companion_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:16.000000 species-0.8.1/species/data/companion_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    55027 2024-01-22 08:40:35.000000 species-0.8.1/species/data/companion_data/companion_data.json
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1948 2023-09-26 09:49:21.000000 species-0.8.1/species/data/companion_data/companion_spectra.json
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2683 2024-02-17 07:17:18.000000 species-0.8.1/species/data/companion_data/companion_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   175685 2024-03-26 08:30:19.000000 species-0.8.1/species/data/database.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.574082 species-0.8.1/species/data/filter_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:26.000000 species-0.8.1/species/data/filter_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8767 2024-01-30 09:26:08.000000 species-0.8.1/species/data/filter_data/filter_data.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.577628 species-0.8.1/species/data/isochrone_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:36.000000 species-0.8.1/species/data/isochrone_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3250 2023-11-09 19:21:10.000000 species-0.8.1/species/data/isochrone_data/add_isochrone.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1425 2023-11-12 06:39:59.000000 species-0.8.1/species/data/isochrone_data/iso_ames.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4003 2023-11-12 06:41:33.000000 species-0.8.1/species/data/isochrone_data/iso_atmo.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2277 2023-11-12 06:43:13.000000 species-0.8.1/species/data/isochrone_data/iso_baraffe2015.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1116 2023-11-12 06:42:46.000000 species-0.8.1/species/data/isochrone_data/iso_btsettl.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5161 2023-11-12 06:43:39.000000 species-0.8.1/species/data/isochrone_data/iso_linder2019.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3486 2023-11-12 06:43:55.000000 species-0.8.1/species/data/isochrone_data/iso_manual.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1459 2023-11-12 06:44:16.000000 species-0.8.1/species/data/isochrone_data/iso_marleau.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1112 2023-11-12 06:44:39.000000 species-0.8.1/species/data/isochrone_data/iso_nextgen.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3737 2023-11-12 06:45:25.000000 species-0.8.1/species/data/isochrone_data/iso_saumon2008.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3674 2023-11-12 06:45:50.000000 species-0.8.1/species/data/isochrone_data/iso_sonora.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.578354 species-0.8.1/species/data/misc_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:47.000000 species-0.8.1/species/data/misc_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4193 2023-11-01 12:20:50.000000 species-0.8.1/species/data/misc_data/accretion_data.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6337 2024-03-24 14:12:36.000000 species-0.8.1/species/data/misc_data/dust_data.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.579317 species-0.8.1/species/data/model_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:57.000000 species-0.8.1/species/data/model_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    10210 2024-03-05 12:07:32.000000 species-0.8.1/species/data/model_data/custom_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    14352 2024-03-27 09:23:03.000000 species-0.8.1/species/data/model_data/model_spectra.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.580090 species-0.8.1/species/data/phot_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:06.000000 species-0.8.1/species/data/phot_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6426 2023-11-12 06:47:44.000000 species-0.8.1/species/data/phot_data/phot_leggett.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     3546 2024-03-15 21:22:31.000000 species-0.8.1/species/data/phot_data/phot_vlm_plx.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.582509 species-0.8.1/species/data/spec_data/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:16.000000 species-0.8.1/species/data/spec_data/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     1926 2023-11-08 18:11:34.000000 species-0.8.1/species/data/spec_data/add_spec_data.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5208 2023-11-08 10:46:04.000000 species-0.8.1/species/data/spec_data/spec_allers2013.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4183 2023-11-08 10:46:50.000000 species-0.8.1/species/data/spec_data/spec_bonnefoy2014.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6288 2023-11-08 10:46:39.000000 species-0.8.1/species/data/spec_data/spec_irtf.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2862 2023-11-08 10:46:45.000000 species-0.8.1/species/data/spec_data/spec_kesseli2017.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8403 2023-11-08 10:46:35.000000 species-0.8.1/species/data/spec_data/spec_spex.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2746 2024-02-17 07:21:56.000000 species-0.8.1/species/data/spec_data/spec_vega.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.586911 species-0.8.1/species/fit/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/fit/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    31343 2023-11-12 13:45:57.000000 species-0.8.1/species/fit/compare_spectra.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    43793 2023-11-01 12:36:23.000000 species-0.8.1/species/fit/emission_line.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    27958 2024-02-14 20:11:52.000000 species-0.8.1/species/fit/fit_evolution.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   105263 2024-03-24 14:11:57.000000 species-0.8.1/species/fit/fit_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6491 2023-11-01 12:43:51.000000 species-0.8.1/species/fit/fit_spectrum.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)   164928 2024-03-26 09:48:51.000000 species-0.8.1/species/fit/retrieval.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.588533 species-0.8.1/species/phot/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-10-29 13:04:27.000000 species-0.8.1/species/phot/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    24412 2024-03-30 16:08:28.000000 species-0.8.1/species/phot/syn_phot.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.593509 species-0.8.1/species/plot/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/plot/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    62134 2024-02-20 10:49:17.000000 species-0.8.1/species/plot/plot_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    38994 2024-02-06 09:51:28.000000 species-0.8.1/species/plot/plot_comparison.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    13747 2024-02-06 09:51:28.000000 species-0.8.1/species/plot/plot_evolution.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    48164 2024-03-24 14:07:32.000000 species-0.8.1/species/plot/plot_mcmc.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    49229 2024-03-24 14:08:47.000000 species-0.8.1/species/plot/plot_retrieval.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    53091 2024-03-27 09:35:07.000000 species-0.8.1/species/plot/plot_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.598394 species-0.8.1/species/read/
--rw-r--r--   0 tomasstolker   (501) staff       (20)      195 2023-11-08 13:49:49.000000 species-0.8.1/species/read/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    12304 2024-02-20 11:54:51.000000 species-0.8.1/species/read/read_calibration.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15701 2024-03-19 13:24:36.000000 species-0.8.1/species/read/read_color.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     7145 2024-03-30 16:15:36.000000 species-0.8.1/species/read/read_filter.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    66511 2024-02-14 20:15:05.000000 species-0.8.1/species/read/read_isochrone.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    71397 2024-03-26 09:44:26.000000 species-0.8.1/species/read/read_model.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8595 2024-03-21 19:11:20.000000 species-0.8.1/species/read/read_object.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15897 2024-02-20 11:57:00.000000 species-0.8.1/species/read/read_planck.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    49839 2024-03-24 14:04:15.000000 species-0.8.1/species/read/read_radtrans.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    11572 2023-11-12 13:30:01.000000 species-0.8.1/species/read/read_spectrum.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.604343 species-0.8.1/species/util/
--rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.1/species/util/__init__.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6515 2024-03-25 20:42:03.000000 species-0.8.1/species/util/box_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     6815 2023-11-01 11:49:39.000000 species-0.8.1/species/util/convert_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      742 2024-02-12 19:25:19.000000 species-0.8.1/species/util/core_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    36789 2024-03-26 13:25:02.000000 species-0.8.1/species/util/data_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    20231 2024-03-24 13:59:15.000000 species-0.8.1/species/util/dust_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    15678 2024-03-24 13:59:15.000000 species-0.8.1/species/util/fit_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    10146 2024-03-27 08:20:31.000000 species-0.8.1/species/util/model_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    44468 2024-03-27 09:39:35.000000 species-0.8.1/species/util/plot_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8068 2023-12-21 09:32:43.000000 species-0.8.1/species/util/query_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     8626 2024-03-24 13:59:15.000000 species-0.8.1/species/util/radtrans_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)    95994 2024-03-26 09:34:14.000000 species-0.8.1/species/util/retrieval_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)     5124 2024-03-11 09:49:58.000000 species-0.8.1/species/util/spec_util.py
--rw-r--r--   0 tomasstolker   (501) staff       (20)      763 2024-02-14 20:12:21.000000 species-0.8.1/species/util/test_util.py
-drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:09:49.568744 species-0.8.1/species.egg-info/
--rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/PKG-INFO
--rw-r--r--   0 tomasstolker   (501) staff       (20)     2922 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/SOURCES.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/dependency_links.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/not-zip-safe
--rw-r--r--   0 tomasstolker   (501) staff       (20)      444 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/requires.txt
--rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2024-04-03 20:09:49.000000 species-0.8.1/species.egg-info/top_level.txt
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.822435 species-0.8.2/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1075 2023-09-26 09:49:21.000000 species-0.8.2/LICENSE
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:50:00.822280 species-0.8.2/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3513 2024-04-03 18:12:34.000000 species-0.8.2/README.rst
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       38 2024-04-03 20:50:00.822480 species-0.8.2/setup.cfg
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1380 2024-04-03 20:44:10.000000 species-0.8.2/setup.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.788339 species-0.8.2/species/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      223 2024-04-03 20:44:07.000000 species-0.8.2/species/__init__.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.790556 species-0.8.2/species/core/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.2/species/core/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15235 2024-03-26 09:45:01.000000 species-0.8.2/species/core/box.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      880 2023-11-08 06:43:57.000000 species-0.8.2/species/core/constants.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4863 2024-03-30 11:12:28.000000 species-0.8.2/species/core/species_init.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.791227 species-0.8.2/species/data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)       23 2023-11-08 20:53:44.000000 species-0.8.2/species/data/__init__.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.794597 species-0.8.2/species/data/companion_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:16.000000 species-0.8.2/species/data/companion_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    55027 2024-01-22 08:40:35.000000 species-0.8.2/species/data/companion_data/companion_data.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1948 2023-09-26 09:49:21.000000 species-0.8.2/species/data/companion_data/companion_spectra.json
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2683 2024-02-17 07:17:18.000000 species-0.8.2/species/data/companion_data/companion_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   175685 2024-03-26 08:30:19.000000 species-0.8.2/species/data/database.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.795056 species-0.8.2/species/data/filter_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:26.000000 species-0.8.2/species/data/filter_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8767 2024-01-30 09:26:08.000000 species-0.8.2/species/data/filter_data/filter_data.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.798592 species-0.8.2/species/data/isochrone_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:36.000000 species-0.8.2/species/data/isochrone_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3250 2023-11-09 19:21:10.000000 species-0.8.2/species/data/isochrone_data/add_isochrone.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1425 2023-11-12 06:39:59.000000 species-0.8.2/species/data/isochrone_data/iso_ames.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4003 2023-11-12 06:41:33.000000 species-0.8.2/species/data/isochrone_data/iso_atmo.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2277 2023-11-12 06:43:13.000000 species-0.8.2/species/data/isochrone_data/iso_baraffe2015.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1116 2023-11-12 06:42:46.000000 species-0.8.2/species/data/isochrone_data/iso_btsettl.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5161 2023-11-12 06:43:39.000000 species-0.8.2/species/data/isochrone_data/iso_linder2019.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3486 2023-11-12 06:43:55.000000 species-0.8.2/species/data/isochrone_data/iso_manual.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1459 2023-11-12 06:44:16.000000 species-0.8.2/species/data/isochrone_data/iso_marleau.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1112 2023-11-12 06:44:39.000000 species-0.8.2/species/data/isochrone_data/iso_nextgen.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3737 2023-11-12 06:45:25.000000 species-0.8.2/species/data/isochrone_data/iso_saumon2008.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3674 2023-11-12 06:45:50.000000 species-0.8.2/species/data/isochrone_data/iso_sonora.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.799203 species-0.8.2/species/data/misc_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:47.000000 species-0.8.2/species/data/misc_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4193 2023-11-01 12:20:50.000000 species-0.8.2/species/data/misc_data/accretion_data.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6337 2024-03-24 14:12:36.000000 species-0.8.2/species/data/misc_data/dust_data.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.800084 species-0.8.2/species/data/model_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:52:57.000000 species-0.8.2/species/data/model_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    10210 2024-03-05 12:07:32.000000 species-0.8.2/species/data/model_data/custom_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    14352 2024-03-27 09:23:03.000000 species-0.8.2/species/data/model_data/model_spectra.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.800856 species-0.8.2/species/data/phot_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:06.000000 species-0.8.2/species/data/phot_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6426 2023-11-12 06:47:44.000000 species-0.8.2/species/data/phot_data/phot_leggett.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     3546 2024-03-15 21:22:31.000000 species-0.8.2/species/data/phot_data/phot_vlm_plx.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.803205 species-0.8.2/species/data/spec_data/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-11-08 20:53:16.000000 species-0.8.2/species/data/spec_data/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     1926 2023-11-08 18:11:34.000000 species-0.8.2/species/data/spec_data/add_spec_data.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5208 2023-11-08 10:46:04.000000 species-0.8.2/species/data/spec_data/spec_allers2013.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4183 2023-11-08 10:46:50.000000 species-0.8.2/species/data/spec_data/spec_bonnefoy2014.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6288 2023-11-08 10:46:39.000000 species-0.8.2/species/data/spec_data/spec_irtf.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2862 2023-11-08 10:46:45.000000 species-0.8.2/species/data/spec_data/spec_kesseli2017.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8403 2023-11-08 10:46:35.000000 species-0.8.2/species/data/spec_data/spec_spex.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2746 2024-02-17 07:21:56.000000 species-0.8.2/species/data/spec_data/spec_vega.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.806503 species-0.8.2/species/fit/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.2/species/fit/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    31343 2023-11-12 13:45:57.000000 species-0.8.2/species/fit/compare_spectra.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    43793 2023-11-01 12:36:23.000000 species-0.8.2/species/fit/emission_line.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    27958 2024-02-14 20:11:52.000000 species-0.8.2/species/fit/fit_evolution.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   105263 2024-03-24 14:11:57.000000 species-0.8.2/species/fit/fit_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6491 2023-11-01 12:43:51.000000 species-0.8.2/species/fit/fit_spectrum.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)   164928 2024-03-26 09:48:51.000000 species-0.8.2/species/fit/retrieval.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.807474 species-0.8.2/species/phot/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2023-10-29 13:04:27.000000 species-0.8.2/species/phot/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    24412 2024-03-30 16:08:28.000000 species-0.8.2/species/phot/syn_phot.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.811497 species-0.8.2/species/plot/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.2/species/plot/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    62134 2024-02-20 10:49:17.000000 species-0.8.2/species/plot/plot_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    38994 2024-02-06 09:51:28.000000 species-0.8.2/species/plot/plot_comparison.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    13747 2024-02-06 09:51:28.000000 species-0.8.2/species/plot/plot_evolution.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    48164 2024-03-24 14:07:32.000000 species-0.8.2/species/plot/plot_mcmc.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    49229 2024-03-24 14:08:47.000000 species-0.8.2/species/plot/plot_retrieval.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    53091 2024-03-27 09:35:07.000000 species-0.8.2/species/plot/plot_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.816043 species-0.8.2/species/read/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      195 2023-11-08 13:49:49.000000 species-0.8.2/species/read/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    12304 2024-02-20 11:54:51.000000 species-0.8.2/species/read/read_calibration.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15701 2024-03-19 13:24:36.000000 species-0.8.2/species/read/read_color.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     7145 2024-03-30 16:15:36.000000 species-0.8.2/species/read/read_filter.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    66511 2024-02-14 20:15:05.000000 species-0.8.2/species/read/read_isochrone.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    71397 2024-03-26 09:44:26.000000 species-0.8.2/species/read/read_model.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8595 2024-03-21 19:11:20.000000 species-0.8.2/species/read/read_object.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15897 2024-02-20 11:57:00.000000 species-0.8.2/species/read/read_planck.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    49839 2024-03-24 14:04:15.000000 species-0.8.2/species/read/read_radtrans.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    11572 2023-11-12 13:30:01.000000 species-0.8.2/species/read/read_spectrum.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.821941 species-0.8.2/species/util/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        0 2021-02-06 22:03:48.000000 species-0.8.2/species/util/__init__.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6515 2024-03-25 20:42:03.000000 species-0.8.2/species/util/box_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     6815 2023-11-01 11:49:39.000000 species-0.8.2/species/util/convert_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      742 2024-02-12 19:25:19.000000 species-0.8.2/species/util/core_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    36789 2024-03-26 13:25:02.000000 species-0.8.2/species/util/data_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    20231 2024-03-24 13:59:15.000000 species-0.8.2/species/util/dust_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    15678 2024-03-24 13:59:15.000000 species-0.8.2/species/util/fit_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    10146 2024-03-27 08:20:31.000000 species-0.8.2/species/util/model_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    44468 2024-03-27 09:39:35.000000 species-0.8.2/species/util/plot_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8068 2023-12-21 09:32:43.000000 species-0.8.2/species/util/query_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     8626 2024-03-24 13:59:15.000000 species-0.8.2/species/util/radtrans_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)    95994 2024-03-26 09:34:14.000000 species-0.8.2/species/util/retrieval_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     5124 2024-03-11 09:49:58.000000 species-0.8.2/species/util/spec_util.py
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      763 2024-02-14 20:12:21.000000 species-0.8.2/species/util/test_util.py
+drwxr-xr-x   0 tomasstolker   (501) staff       (20)        0 2024-04-03 20:50:00.789163 species-0.8.2/species.egg-info/
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     4301 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/PKG-INFO
+-rw-r--r--   0 tomasstolker   (501) staff       (20)     2922 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/SOURCES.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/dependency_links.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        1 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/not-zip-safe
+-rw-r--r--   0 tomasstolker   (501) staff       (20)      444 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/requires.txt
+-rw-r--r--   0 tomasstolker   (501) staff       (20)        8 2024-04-03 20:50:00.000000 species-0.8.2/species.egg-info/top_level.txt
```

### Comparing `species-0.8.1/LICENSE` & `species-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `species-0.8.1/PKG-INFO` & `species-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: species
-Version: 0.8.1
+Version: 0.8.2
 Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
 Home-page: https://github.com/tomasstolker/species
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://species.readthedocs.io
 Keywords: species
```

### Comparing `species-0.8.1/README.rst` & `species-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `species-0.8.1/setup.py` & `species-0.8.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 
 with open("requirements.txt") as req_txt:
     parse_req = pkg_resources.parse_requirements(req_txt)
     install_requires = [str(req) for req in parse_req]
 
 setuptools.setup(
     name="species",
-    version="0.8.1",
+    version="0.8.2",
     description="Toolkit for atmospheric characterization of directly imaged exoplanets",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Tomas Stolker",
     author_email="stolker@strw.leidenuniv.nl",
     url="https://github.com/tomasstolker/species",
     project_urls={"Documentation": "https://species.readthedocs.io"},
     packages=setuptools.find_packages(include=["species", "species.*"]),
+    package_dir={"species:": "species"},
     package_data={"species": ["data/companion_data/*.json"]},
     install_requires=install_requires,
     tests_require=["pytest"],
     license="MIT",
     zip_safe=False,
     keywords="species",
     classifiers=[
```

### Comparing `species-0.8.1/species/core/box.py` & `species-0.8.2/species/core/box.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/core/constants.py` & `species-0.8.2/species/core/constants.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/core/species_init.py` & `species-0.8.2/species/core/species_init.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/companion_data/companion_data.json` & `species-0.8.2/species/data/companion_data/companion_data.json`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/companion_data/companion_spectra.json` & `species-0.8.2/species/data/companion_data/companion_spectra.json`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/companion_data/companion_spectra.py` & `species-0.8.2/species/data/companion_data/companion_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/database.py` & `species-0.8.2/species/data/database.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/filter_data/filter_data.py` & `species-0.8.2/species/data/filter_data/filter_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/add_isochrone.py` & `species-0.8.2/species/data/isochrone_data/add_isochrone.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_ames.py` & `species-0.8.2/species/data/isochrone_data/iso_ames.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_atmo.py` & `species-0.8.2/species/data/isochrone_data/iso_atmo.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_baraffe2015.py` & `species-0.8.2/species/data/isochrone_data/iso_baraffe2015.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_btsettl.py` & `species-0.8.2/species/data/isochrone_data/iso_btsettl.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_linder2019.py` & `species-0.8.2/species/data/isochrone_data/iso_linder2019.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_manual.py` & `species-0.8.2/species/data/isochrone_data/iso_manual.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_marleau.py` & `species-0.8.2/species/data/isochrone_data/iso_marleau.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_nextgen.py` & `species-0.8.2/species/data/isochrone_data/iso_nextgen.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_saumon2008.py` & `species-0.8.2/species/data/isochrone_data/iso_saumon2008.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/isochrone_data/iso_sonora.py` & `species-0.8.2/species/data/isochrone_data/iso_sonora.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/misc_data/accretion_data.py` & `species-0.8.2/species/data/misc_data/accretion_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/misc_data/dust_data.py` & `species-0.8.2/species/data/misc_data/dust_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/model_data/custom_model.py` & `species-0.8.2/species/data/model_data/custom_model.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/model_data/model_spectra.py` & `species-0.8.2/species/data/model_data/model_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/phot_data/phot_leggett.py` & `species-0.8.2/species/data/phot_data/phot_leggett.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/phot_data/phot_vlm_plx.py` & `species-0.8.2/species/data/phot_data/phot_vlm_plx.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/add_spec_data.py` & `species-0.8.2/species/data/spec_data/add_spec_data.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_allers2013.py` & `species-0.8.2/species/data/spec_data/spec_allers2013.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_bonnefoy2014.py` & `species-0.8.2/species/data/spec_data/spec_bonnefoy2014.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_irtf.py` & `species-0.8.2/species/data/spec_data/spec_irtf.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_kesseli2017.py` & `species-0.8.2/species/data/spec_data/spec_kesseli2017.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_spex.py` & `species-0.8.2/species/data/spec_data/spec_spex.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/data/spec_data/spec_vega.py` & `species-0.8.2/species/data/spec_data/spec_vega.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/compare_spectra.py` & `species-0.8.2/species/fit/compare_spectra.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/emission_line.py` & `species-0.8.2/species/fit/emission_line.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/fit_evolution.py` & `species-0.8.2/species/fit/fit_evolution.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/fit_model.py` & `species-0.8.2/species/fit/fit_model.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/fit_spectrum.py` & `species-0.8.2/species/fit/fit_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/fit/retrieval.py` & `species-0.8.2/species/fit/retrieval.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/phot/syn_phot.py` & `species-0.8.2/species/phot/syn_phot.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_color.py` & `species-0.8.2/species/plot/plot_color.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_comparison.py` & `species-0.8.2/species/plot/plot_comparison.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_evolution.py` & `species-0.8.2/species/plot/plot_evolution.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_mcmc.py` & `species-0.8.2/species/plot/plot_mcmc.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_retrieval.py` & `species-0.8.2/species/plot/plot_retrieval.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/plot/plot_spectrum.py` & `species-0.8.2/species/plot/plot_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_calibration.py` & `species-0.8.2/species/read/read_calibration.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_color.py` & `species-0.8.2/species/read/read_color.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_filter.py` & `species-0.8.2/species/read/read_filter.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_isochrone.py` & `species-0.8.2/species/read/read_isochrone.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_model.py` & `species-0.8.2/species/read/read_model.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_object.py` & `species-0.8.2/species/read/read_object.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_planck.py` & `species-0.8.2/species/read/read_planck.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_radtrans.py` & `species-0.8.2/species/read/read_radtrans.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/read/read_spectrum.py` & `species-0.8.2/species/read/read_spectrum.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/box_util.py` & `species-0.8.2/species/util/box_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/convert_util.py` & `species-0.8.2/species/util/convert_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/core_util.py` & `species-0.8.2/species/util/core_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/data_util.py` & `species-0.8.2/species/util/data_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/dust_util.py` & `species-0.8.2/species/util/dust_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/fit_util.py` & `species-0.8.2/species/util/fit_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/model_util.py` & `species-0.8.2/species/util/model_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/plot_util.py` & `species-0.8.2/species/util/plot_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/query_util.py` & `species-0.8.2/species/util/query_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/radtrans_util.py` & `species-0.8.2/species/util/radtrans_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/retrieval_util.py` & `species-0.8.2/species/util/retrieval_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/spec_util.py` & `species-0.8.2/species/util/spec_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species/util/test_util.py` & `species-0.8.2/species/util/test_util.py`

 * *Files identical despite different names*

### Comparing `species-0.8.1/species.egg-info/PKG-INFO` & `species-0.8.2/species.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: species
-Version: 0.8.1
+Version: 0.8.2
 Summary: Toolkit for atmospheric characterization of directly imaged exoplanets
 Home-page: https://github.com/tomasstolker/species
 Author: Tomas Stolker
 Author-email: stolker@strw.leidenuniv.nl
 License: MIT
 Project-URL: Documentation, https://species.readthedocs.io
 Keywords: species
```

### Comparing `species-0.8.1/species.egg-info/SOURCES.txt` & `species-0.8.2/species.egg-info/SOURCES.txt`

 * *Files identical despite different names*

