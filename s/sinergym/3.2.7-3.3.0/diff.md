# Comparing `tmp/sinergym-3.2.7.tar.gz` & `tmp/sinergym-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sinergym-3.2.7.tar", last modified: Wed Mar 13 10:52:10 2024, max compression
+gzip compressed data, was "sinergym-3.3.0.tar", last modified: Wed Apr  3 08:18:46 2024, max compression
```

## Comparing `sinergym-3.2.7.tar` & `sinergym-3.3.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.910455 sinergym-3.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-13 10:52:06.000000 sinergym-3.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-13 10:52:06.000000 sinergym-3.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-03-13 10:52:10.910455 sinergym-3.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12724 2024-03-13 10:52:06.000000 sinergym-3.2.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-13 10:52:10.000000 sinergym-3.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-13 10:52:10.910455 sinergym-3.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-03-13 10:52:10.000000 sinergym-3.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.870455 sinergym-3.2.7/sinergym/
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym/config/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/config/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.870455 sinergym-3.2.7/sinergym/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym/data/buildings/
--rw-r--r--   0 runner    (1001) docker     (127)    66897 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   145181 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/ShopWithPVandBattery.epJSON
--rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/buildings/radiant_residential_building.epJSON
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.878455 sinergym-3.2.7/sinergym/data/default_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/ShopWithPVandBattery.json
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/default_configuration/radiant_residential_building.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/data/weather/
--rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
--rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
--rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/envs/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/envs/eplus_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.906455 sinergym-3.2.7/sinergym/simulators/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/simulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/simulators/eplus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.910455 sinergym-3.2.7/sinergym/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    15220 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/env_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/rewards.py
--rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/utils/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 10:52:10.874455 sinergym-3.2.7/sinergym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13632 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 10:52:10.000000 sinergym-3.2.7/sinergym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.696763 sinergym-3.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 08:18:42.000000 sinergym-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 08:18:42.000000 sinergym-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-03 08:18:46.696763 sinergym-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-03 08:18:42.000000 sinergym-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 08:18:46.000000 sinergym-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 08:18:46.696763 sinergym-3.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-03 08:18:46.000000 sinergym-3.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.660763 sinergym-3.3.0/sinergym/
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.660763 sinergym-3.3.0/sinergym/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29305 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/config/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.660763 sinergym-3.3.0/sinergym/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.664763 sinergym-3.3.0/sinergym/data/buildings/
+-rw-r--r--   0 runner    (1001) docker     (127)    66901 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   151242 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   145181 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   595437 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   272977 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   512302 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   245040 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/ShopWithPVandBattery.epJSON
+-rw-r--r--   0 runner    (1001) docker     (127)   389111 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/buildings/radiant_residential_building.epJSON
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.664763 sinergym-3.3.0/sinergym/data/default_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)     5047 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/5ZoneAutoDXVAV.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4499 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/ShopWithPVandBattery.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/default_configuration/radiant_residential_building.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.692763 sinergym-3.3.0/sinergym/data/weather/
+-rw-r--r--   0 runner    (1001) docker     (127)    28629 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1565086 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28503 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550279 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28704 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1621761 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28716 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1553382 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28801 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558629 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28740 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1558423 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28659 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1601571 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1550263 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29016 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1637298 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29489 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1629153 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    28793 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1639985 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29614 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1613784 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1624547 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw
+-rw-r--r--   0 runner    (1001) docker     (127)    29243 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy
+-rw-r--r--   0 runner    (1001) docker     (127)  1625209 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.696763 sinergym-3.3.0/sinergym/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26793 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/envs/eplus_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.696763 sinergym-3.3.0/sinergym/simulators/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/simulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17678 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/simulators/eplus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.696763 sinergym-3.3.0/sinergym/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22490 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15217 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6102 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5057 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10221 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/env_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14248 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19735 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/rewards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36173 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/utils/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:18:46.660763 sinergym-3.3.0/sinergym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10156 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 08:18:46.000000 sinergym-3.3.0/sinergym.egg-info/top_level.txt
```

### Comparing `sinergym-3.2.7/LICENSE` & `sinergym-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/PKG-INFO` & `sinergym-3.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.2.7
+Version: 3.3.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
@@ -68,121 +68,80 @@
 
 **Welcome to Sinergym!**
 
 <div align="center">
   <img src="images/general_blueprint.png" width=80%><br><br>
 </div>
 
-The goal of this project is to create an environment following [Gymnasium interface](https://gymnasium.farama.org/), for wrapping simulation engines for building control using **deep reinforcement learning**.
+The goal of this project is to create an environment following *Gymnasium* interface for wrapping 
+simulation engines (*EnergyPlus*) for building control using **deep reinforcement learning** 
+or any external control.
 
-For more information about Sinergym, we recommend to visit our [documentation here](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
+For more information about Sinergym, please visit our [documentation](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
 
-Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking about contributing to Sinergym.
+To report questions and issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/issues). We appreciate your feedback and contributions. Check out our [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) for more details on how to contribute.
 
-The main functionalities of *Sinergym* are the following :
+The main functionalities of *Sinergym* are the following:
 
--  **Compatibility with simulation engines**. Communication between
-   Python and [EnergyPlus](https://energyplus.net/) is established
-   using [Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html) as a middleware.
-   However, more of them (e.g.
-   [OpenModelica](https://openmodelica.org/)) could be included in
-   the backend while maintaining the Gymnasium API in the future.
-
--  **Benchmark environments**. Similarly to *Atari* or *Mujoco* environments
-   for RL community, we are designing a set of environments for
-   benchmarking and testing deep RL algorithms. These environments may
-   include different buildings, weathers, action/observation spaces, function rewards, etc.
-
--  **Customizable environments**. We aim to provide a
-   package which allows modifying experimental settings in an easy
-   manner. The user can create his own environments, combining his own
-   building model, weather, reward, observation/action space, variables, actuators, environment name, etc.
-   The user can also use these pre-configured environments available in *Sinergym* 
-   and change some aspect of it (for example, the weather) in such 
-   a way that he does not  have to make an entire definition of the 
-   environment and can start from one pre-designed by us.
-   Some parameters directly associated with the simulator can be set as **extra configuration** 
-   as well, such as people occupant, time-steps per simulation hour, run-period, etc.
-
--  **Customizable components**. *Sinergym* is easily scalable by third parties.
-   Following the structure of the implemented classes, new custom components 
-   can be created for new environments such as function rewards, wrappers,
-   controllers, etc.
-
--  **Automatic Building Model adaptation to user changes**. Many of the updates to the environment definition require changes 
-   to the building model (*epJSON* file) to adapt it to these new features before the simulation starts, which *Sinergym* will 
-   perform automatically. For example, using another weather file requires building location and design days update, using new 
-   observation variables requires to update the `Output:Variable` and `Output:Meter` fields, the same occurs with extra 
-   configuration context concerned with simulation directly, if weather variability is set, then a weather with noise 
-   will be used. These new building and weather file versions, is saved in the *Sinergym* output folder, leaving the original 
-   intact. In short, *Sinergym* automates the whole process of model adaptation so that the user 
-   only has to define what he wants for his environment.
-
--  **Automatic actuators control**. Related to the above, it will only be necessary to specify the name of the actuators to be controlled 
-   through the actions of the Gymnasium interface, and *Sinergym* will take care of everything.
-
--  **Extensive environment information**. It is important that users can get some information about *Sinergym* background components from environment interface easily.
-   From environment instance, it is possible to consult available schedulers, variables which compose an observation and action, whether simulator is running,
-   the building run period, episode length, timesteps per episode, available building zones... And much more.
-
--  **Stable Baseline 3 Integration**. Some functionalities like callbacks
-   have been customized by our team in order to test easily these environments
-   with deep reinforcement learning algorithms and logger specific information about 
-   *Sinergym* environments. 
-   However, *Sinergym* is completely agnostic to any DRL algorithm and can be used with any DRL 
-   library that works with gymnasium interface.
-
--  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
-   use your infrastructure with *Sinergym*, we tell you some details about how to do it.
-
--  **Weights & Biases tracking and visualization compatibility**. One of *Sinergym*'s objectives is to automate
-   and facilitate the training, reproducibility and comparison of agents in simulation-based 
-   building control problems, managing and monitoring model lifecycle from training to deployment. [WandB](https://wandb.ai/site)
-   is an open-source platform for the machine learning lifecycle helping us with this issue. 
-   It lets us register experiments hyperparameters, visualize data recorded in real-time, 
-   and store artifacts with experiment outputs and best obtained models. 
-
--  **Notebooks examples**. *Sinergym* develops code in notebook format with the purpose of offering use cases to 
-   the users in order to help them become familiar with the tool. They are constantly updated, along with the updates 
-   and improvements of the tool itself.
+- **Simulation Engine Compatibility**: Uses [EnergyPlus Python API](https://energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus communication. Future plans include more engines like [OpenModelica](https://openmodelica.org/).
 
--  This project is accompanied by extensive **documentation**, **unit tests** and **github actions workflows** to make 
-   *Sinergym* an efficient ecosystem for both understanding and development.
+- **Benchmark Environments**: Designs environments for benchmarking and testing deep RL algorithms or other external strategies, similar to *Atari* or *Mujoco*.
 
--  Many more!
+- **Customizable Environments**: Allows easy modification of experimental settings. Users can create their own environments or modify pre-configured ones in *Sinergym*.
+
+- **Customizable Components**: Enables creation of new custom components for new environments, making *Sinergym* scalable, such as function rewards, wrappers, controllers, etc.
+
+- **Automatic Building Model Adaptation**: *Sinergym* automates the process of adapting the building model to user changes in the environment definition.
+
+- **Automatic Actuators Control**: Controls actuators through the Gymnasium interface based on user specification, only actuators names are required and *Sinergym* will do the rest.
+
+- **Extensive Environment Information**: Provides comprehensive information about *Sinergym* background components from the environment interface.
+
+- **Stable Baseline 3 Integration**: Customizes functionalities for easy testing of environments with SB3 algorithms, such as callbacks and customizable training real-time logging. However, *Sinergym* is agnostic to any DRL algorithm.
+
+- **Google Cloud Integration**: Offers guidance on using *Sinergym* with Google Cloud infrastructure.
+
+- **Weights & Biases Compatibility**: Automates and facilitates training, reproducibility, and comparison of agents in simulation-based building control problems. [WandB](https://wandb.ai/site) assists in managing and monitoring model lifecycle.
+
+- **Notebook Examples**: Provides code in notebook format for user familiarity with the tool.
+
+- **Extensive Documentation, Unit Tests, and GitHub Actions Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and development.
+
+- And much more!
 
 _This is a project in active development. Stay tuned for upcoming releases._
 
 <div align="center">
   <img src="images/operation_diagram.png"><br><br>
 </div>
 
-## Project structure
+## Project Structure
 
-This repository is organized in the next directories:
+This repository is organized into the following directories:
 
-- `sinergym/`: Here you will find all the source code that forms *Sinergym*: environment, modeling, simulator, and tools such as wrappers, reward functions, etc.
-- `docs/`: Online documentation, generated with Sphinx and using Restructured Text (RST).
-- `examples/`: Here there are a set of notebooks written in Jupyter format. Use cases are illustrated with Sinergym.
-- `tests/`: All the unit tests of Sinergym. Fixtures and checks are defined here in order to check that the tool is in a stable state.
-- `scripts/`: This folder contains scripts in which Sinergym is used. We can find useful things for the users, such as agent training, agent loading, performance checks, etc. In addition, these scripts allow a high margin of configuration using the JSON format.
+- `sinergym/`: Contains the source code for *Sinergym*, including the environment, modeling, simulator, and tools such as wrappers and reward functions.
+- `docs/`: Online documentation generated with Sphinx and using Restructured Text (RST).
+- `examples/`: Jupyter notebooks illustrating use cases with Sinergym.
+- `tests/`: Unit tests for Sinergym to ensure stability.
+- `scripts/`: Scripts for various tasks such as agent training and performance checks, allowing configuration using JSON format.
 
-## List of available environments
+## Available Environments
 
-If you would like to see a complete and updated list of our available environments, please visit [our list](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the official *Sinergym* documentation.
+For a complete and up-to-date list of available environments, please refer to [our documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#).
 
 ## Installation
 
-Please, visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more information about Sinergym installation.
+Please visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation instructions.
 
 ## Usage example
 
+
 If you used our Dockerfile during installation, you should have the *try_env.py* file in your workspace as soon as you enter in. In case you have installed everything on your local machine directly, place it inside our cloned repository. In any case, we start from the point that you have at your disposal a terminal with the appropriate python version and *Sinergym* running correctly.
 
-*Sinergym* uses the standard Gymnasium API. So basic loop should be something like:
+*Sinergym* uses the standard Gymnasium API. So a basic loop should look like:
 
 ```python
 
 import gymnasium as gym
 import sinergym
 # Create the environment
 env = gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1')
@@ -194,17 +153,18 @@
     a = env.action_space.sample() # random action selection
     obs, reward, terminated, truncated, info = env.step(a) # get new observation and reward
     R += reward
 print('Total reward for the episode: %.4f' % R)
 env.close()
 ```
 
-Notice that a folder will be created in the working directory after creating the environment. It will contain the EnergyPlus outputs produced during the simulation.
+A folder will be created in the working directory after creating the environment. It will contain the Sinergym outputs produced during the simulation.
+
+For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
-:pencil: For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
 ## Google Cloud Platform support
 
 For more information about this functionality, please, visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud).
 
 ## Projects using Sinergym
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.2.7 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.3.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
@@ -19,127 +19,84 @@
                                    _v_e_r_s_i_o_n_]
 
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_S_u_p_p_o_r_t_e_d_%_2_0_b_y_-_V_S_C_o_d_e_%_2_0_P_o_w_e_r_%_2_0_U_s_e_r_%_2_0_%_E_2_%_8_6_%_9_2_-
            _g_r_a_y_._s_v_g_?_c_o_l_o_r_A_=_6_5_5_B_E_1_&_c_o_l_o_r_B_=_4_F_4_4_D_6_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 **Welcome to Sinergym!**
                         [images/general_blueprint.png]
 
-The goal of this project is to create an environment following [Gymnasium
-interface](https://gymnasium.farama.org/), for wrapping simulation engines for
-building control using **deep reinforcement learning**. For more information
-about Sinergym, we recommend to visit our [documentation here](https://ugr-
-sail.github.io/sinergym/compilation/main/index.html). Please, help us to
-improve by **reporting your questions and issues** [here](https://github.com/
-ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates
-(questions, bugs, improvements, etc.). More detailed info on how to report
-issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/
-creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://
-github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking
-about contributing to Sinergym. The main functionalities of *Sinergym* are the
-following : - **Compatibility with simulation engines**. Communication between
-Python and [EnergyPlus](https://energyplus.net/) is established using
-[Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html)
-as a middleware. However, more of them (e.g. [OpenModelica](https://
-openmodelica.org/)) could be included in the backend while maintaining the
-Gymnasium API in the future. - **Benchmark environments**. Similarly to *Atari*
-or *Mujoco* environments for RL community, we are designing a set of
-environments for benchmarking and testing deep RL algorithms. These
-environments may include different buildings, weathers, action/observation
-spaces, function rewards, etc. - **Customizable environments**. We aim to
-provide a package which allows modifying experimental settings in an easy
-manner. The user can create his own environments, combining his own building
-model, weather, reward, observation/action space, variables, actuators,
-environment name, etc. The user can also use these pre-configured environments
-available in *Sinergym* and change some aspect of it (for example, the weather)
-in such a way that he does not have to make an entire definition of the
-environment and can start from one pre-designed by us. Some parameters directly
-associated with the simulator can be set as **extra configuration** as well,
-such as people occupant, time-steps per simulation hour, run-period, etc. -
-**Customizable components**. *Sinergym* is easily scalable by third parties.
-Following the structure of the implemented classes, new custom components can
-be created for new environments such as function rewards, wrappers,
-controllers, etc. - **Automatic Building Model adaptation to user changes**.
-Many of the updates to the environment definition require changes to the
-building model (*epJSON* file) to adapt it to these new features before the
-simulation starts, which *Sinergym* will perform automatically. For example,
-using another weather file requires building location and design days update,
-using new observation variables requires to update the `Output:Variable` and
-`Output:Meter` fields, the same occurs with extra configuration context
-concerned with simulation directly, if weather variability is set, then a
-weather with noise will be used. These new building and weather file versions,
-is saved in the *Sinergym* output folder, leaving the original intact. In
-short, *Sinergym* automates the whole process of model adaptation so that the
-user only has to define what he wants for his environment. - **Automatic
-actuators control**. Related to the above, it will only be necessary to specify
-the name of the actuators to be controlled through the actions of the Gymnasium
-interface, and *Sinergym* will take care of everything. - **Extensive
-environment information**. It is important that users can get some information
-about *Sinergym* background components from environment interface easily. From
-environment instance, it is possible to consult available schedulers, variables
-which compose an observation and action, whether simulator is running, the
-building run period, episode length, timesteps per episode, available building
-zones... And much more. - **Stable Baseline 3 Integration**. Some
-functionalities like callbacks have been customized by our team in order to
-test easily these environments with deep reinforcement learning algorithms and
-logger specific information about *Sinergym* environments. However, *Sinergym*
-is completely agnostic to any DRL algorithm and can be used with any DRL
-library that works with gymnasium interface. - **Google Cloud Integration**.
-Whether you have a Google Cloud account and you want to use your infrastructure
-with *Sinergym*, we tell you some details about how to do it. - **Weights &
-Biases tracking and visualization compatibility**. One of *Sinergym*'s
-objectives is to automate and facilitate the training, reproducibility and
-comparison of agents in simulation-based building control problems, managing
-and monitoring model lifecycle from training to deployment. [WandB](https://
-wandb.ai/site) is an open-source platform for the machine learning lifecycle
-helping us with this issue. It lets us register experiments hyperparameters,
-visualize data recorded in real-time, and store artifacts with experiment
-outputs and best obtained models. - **Notebooks examples**. *Sinergym* develops
-code in notebook format with the purpose of offering use cases to the users in
-order to help them become familiar with the tool. They are constantly updated,
-along with the updates and improvements of the tool itself. - This project is
-accompanied by extensive **documentation**, **unit tests** and **github actions
-workflows** to make *Sinergym* an efficient ecosystem for both understanding
-and development. - Many more! _This is a project in active development. Stay
+The goal of this project is to create an environment following *Gymnasium*
+interface for wrapping simulation engines (*EnergyPlus*) for building control
+using **deep reinforcement learning** or any external control. For more
+information about Sinergym, please visit our [documentation](https://ugr-
+sail.github.io/sinergym/compilation/main/index.html). To report questions and
+issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/
+issues). We appreciate your feedback and contributions. Check out our
+[CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/
+CONTRIBUTING.md) for more details on how to contribute. The main
+functionalities of *Sinergym* are the following: - **Simulation Engine
+Compatibility**: Uses [EnergyPlus Python API](https://
+energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus
+communication. Future plans include more engines like [OpenModelica](https://
+openmodelica.org/). - **Benchmark Environments**: Designs environments for
+benchmarking and testing deep RL algorithms or other external strategies,
+similar to *Atari* or *Mujoco*. - **Customizable Environments**: Allows easy
+modification of experimental settings. Users can create their own environments
+or modify pre-configured ones in *Sinergym*. - **Customizable Components**:
+Enables creation of new custom components for new environments, making
+*Sinergym* scalable, such as function rewards, wrappers, controllers, etc. -
+**Automatic Building Model Adaptation**: *Sinergym* automates the process of
+adapting the building model to user changes in the environment definition. -
+**Automatic Actuators Control**: Controls actuators through the Gymnasium
+interface based on user specification, only actuators names are required and
+*Sinergym* will do the rest. - **Extensive Environment Information**: Provides
+comprehensive information about *Sinergym* background components from the
+environment interface. - **Stable Baseline 3 Integration**: Customizes
+functionalities for easy testing of environments with SB3 algorithms, such as
+callbacks and customizable training real-time logging. However, *Sinergym* is
+agnostic to any DRL algorithm. - **Google Cloud Integration**: Offers guidance
+on using *Sinergym* with Google Cloud infrastructure. - **Weights & Biases
+Compatibility**: Automates and facilitates training, reproducibility, and
+comparison of agents in simulation-based building control problems. [WandB]
+(https://wandb.ai/site) assists in managing and monitoring model lifecycle. -
+**Notebook Examples**: Provides code in notebook format for user familiarity
+with the tool. - **Extensive Documentation, Unit Tests, and GitHub Actions
+Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and
+development. - And much more! _This is a project in active development. Stay
 tuned for upcoming releases._
                         [images/operation_diagram.png]
 
-## Project structure This repository is organized in the next directories: -
-`sinergym/`: Here you will find all the source code that forms *Sinergym*:
-environment, modeling, simulator, and tools such as wrappers, reward functions,
-etc. - `docs/`: Online documentation, generated with Sphinx and using
-Restructured Text (RST). - `examples/`: Here there are a set of notebooks
-written in Jupyter format. Use cases are illustrated with Sinergym. - `tests/`:
-All the unit tests of Sinergym. Fixtures and checks are defined here in order
-to check that the tool is in a stable state. - `scripts/`: This folder contains
-scripts in which Sinergym is used. We can find useful things for the users,
-such as agent training, agent loading, performance checks, etc. In addition,
-these scripts allow a high margin of configuration using the JSON format. ##
-List of available environments If you would like to see a complete and updated
-list of our available environments, please visit [our list](https://ugr-
-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the
-official *Sinergym* documentation. ## Installation Please, visit [INSTALL.md]
-(https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more
-information about Sinergym installation. ## Usage example If you used our
-Dockerfile during installation, you should have the *try_env.py* file in your
-workspace as soon as you enter in. In case you have installed everything on
-your local machine directly, place it inside our cloned repository. In any
-case, we start from the point that you have at your disposal a terminal with
-the appropriate python version and *Sinergym* running correctly. *Sinergym*
-uses the standard Gymnasium API. So basic loop should be something like:
-```python import gymnasium as gym import sinergym # Create the environment env
-= gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the
-episode obs, info = env.reset() truncated = terminated = False R = 0.0 while
-not (terminated or truncated): a = env.action_space.sample() # random action
-selection obs, reward, terminated, truncated, info = env.step(a) # get new
-observation and reward R += reward print('Total reward for the episode: %.4f' %
-R) env.close() ``` Notice that a folder will be created in the working
-directory after creating the environment. It will contain the EnergyPlus
-outputs produced during the simulation. :pencil: For more examples and details,
-please visit our [usage examples](https://ugr-sail.github.io/sinergym/
-compilation/main/pages/notebooks/basic_example.html#Basic-example)
+## Project Structure This repository is organized into the following
+directories: - `sinergym/`: Contains the source code for *Sinergym*, including
+the environment, modeling, simulator, and tools such as wrappers and reward
+functions. - `docs/`: Online documentation generated with Sphinx and using
+Restructured Text (RST). - `examples/`: Jupyter notebooks illustrating use
+cases with Sinergym. - `tests/`: Unit tests for Sinergym to ensure stability. -
+`scripts/`: Scripts for various tasks such as agent training and performance
+checks, allowing configuration using JSON format. ## Available Environments For
+a complete and up-to-date list of available environments, please refer to [our
+documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/
+environments.html#). ## Installation Please visit [INSTALL.md](https://
+github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation
+instructions. ## Usage example If you used our Dockerfile during installation,
+you should have the *try_env.py* file in your workspace as soon as you enter
+in. In case you have installed everything on your local machine directly, place
+it inside our cloned repository. In any case, we start from the point that you
+have at your disposal a terminal with the appropriate python version and
+*Sinergym* running correctly. *Sinergym* uses the standard Gymnasium API. So a
+basic loop should look like: ```python import gymnasium as gym import sinergym
+# Create the environment env = gym.make('Eplus-datacenter-mixed-continuous-
+stochastic-v1') # Initialize the episode obs, info = env.reset() truncated =
+terminated = False R = 0.0 while not (terminated or truncated): a =
+env.action_space.sample() # random action selection obs, reward, terminated,
+truncated, info = env.step(a) # get new observation and reward R += reward
+print('Total reward for the episode: %.4f' % R) env.close() ``` A folder will
+be created in the working directory after creating the environment. It will
+contain the Sinergym outputs produced during the simulation. For more examples
+and details, please visit our [usage examples](https://ugr-sail.github.io/
+sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example)
 documentation section. ## Google Cloud Platform support For more information
 about this functionality, please, visit our documentation [here](https://ugr-
 sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-
 google-cloud). ## Projects using Sinergym The following are some of the
 projects benefiting from the advantages of Sinergym: - [Demosthen/ActiveRL]
 (https://github.com/Demosthen/ActiveRL) - [VectorInstitute/HV-Ai-C](https://
 github.com/VectorInstitute/HV-Ai-C) - [rdnfn/beobench](https://github.com/
```

### Comparing `sinergym-3.2.7/README.md` & `sinergym-3.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -45,121 +45,80 @@
 
 **Welcome to Sinergym!**
 
 <div align="center">
   <img src="images/general_blueprint.png" width=80%><br><br>
 </div>
 
-The goal of this project is to create an environment following [Gymnasium interface](https://gymnasium.farama.org/), for wrapping simulation engines for building control using **deep reinforcement learning**.
+The goal of this project is to create an environment following *Gymnasium* interface for wrapping 
+simulation engines (*EnergyPlus*) for building control using **deep reinforcement learning** 
+or any external control.
 
-For more information about Sinergym, we recommend to visit our [documentation here](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
+For more information about Sinergym, please visit our [documentation](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
 
-Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking about contributing to Sinergym.
+To report questions and issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/issues). We appreciate your feedback and contributions. Check out our [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) for more details on how to contribute.
 
-The main functionalities of *Sinergym* are the following :
+The main functionalities of *Sinergym* are the following:
 
--  **Compatibility with simulation engines**. Communication between
-   Python and [EnergyPlus](https://energyplus.net/) is established
-   using [Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html) as a middleware.
-   However, more of them (e.g.
-   [OpenModelica](https://openmodelica.org/)) could be included in
-   the backend while maintaining the Gymnasium API in the future.
-
--  **Benchmark environments**. Similarly to *Atari* or *Mujoco* environments
-   for RL community, we are designing a set of environments for
-   benchmarking and testing deep RL algorithms. These environments may
-   include different buildings, weathers, action/observation spaces, function rewards, etc.
-
--  **Customizable environments**. We aim to provide a
-   package which allows modifying experimental settings in an easy
-   manner. The user can create his own environments, combining his own
-   building model, weather, reward, observation/action space, variables, actuators, environment name, etc.
-   The user can also use these pre-configured environments available in *Sinergym* 
-   and change some aspect of it (for example, the weather) in such 
-   a way that he does not  have to make an entire definition of the 
-   environment and can start from one pre-designed by us.
-   Some parameters directly associated with the simulator can be set as **extra configuration** 
-   as well, such as people occupant, time-steps per simulation hour, run-period, etc.
-
--  **Customizable components**. *Sinergym* is easily scalable by third parties.
-   Following the structure of the implemented classes, new custom components 
-   can be created for new environments such as function rewards, wrappers,
-   controllers, etc.
-
--  **Automatic Building Model adaptation to user changes**. Many of the updates to the environment definition require changes 
-   to the building model (*epJSON* file) to adapt it to these new features before the simulation starts, which *Sinergym* will 
-   perform automatically. For example, using another weather file requires building location and design days update, using new 
-   observation variables requires to update the `Output:Variable` and `Output:Meter` fields, the same occurs with extra 
-   configuration context concerned with simulation directly, if weather variability is set, then a weather with noise 
-   will be used. These new building and weather file versions, is saved in the *Sinergym* output folder, leaving the original 
-   intact. In short, *Sinergym* automates the whole process of model adaptation so that the user 
-   only has to define what he wants for his environment.
-
--  **Automatic actuators control**. Related to the above, it will only be necessary to specify the name of the actuators to be controlled 
-   through the actions of the Gymnasium interface, and *Sinergym* will take care of everything.
-
--  **Extensive environment information**. It is important that users can get some information about *Sinergym* background components from environment interface easily.
-   From environment instance, it is possible to consult available schedulers, variables which compose an observation and action, whether simulator is running,
-   the building run period, episode length, timesteps per episode, available building zones... And much more.
-
--  **Stable Baseline 3 Integration**. Some functionalities like callbacks
-   have been customized by our team in order to test easily these environments
-   with deep reinforcement learning algorithms and logger specific information about 
-   *Sinergym* environments. 
-   However, *Sinergym* is completely agnostic to any DRL algorithm and can be used with any DRL 
-   library that works with gymnasium interface.
-
--  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
-   use your infrastructure with *Sinergym*, we tell you some details about how to do it.
-
--  **Weights & Biases tracking and visualization compatibility**. One of *Sinergym*'s objectives is to automate
-   and facilitate the training, reproducibility and comparison of agents in simulation-based 
-   building control problems, managing and monitoring model lifecycle from training to deployment. [WandB](https://wandb.ai/site)
-   is an open-source platform for the machine learning lifecycle helping us with this issue. 
-   It lets us register experiments hyperparameters, visualize data recorded in real-time, 
-   and store artifacts with experiment outputs and best obtained models. 
-
--  **Notebooks examples**. *Sinergym* develops code in notebook format with the purpose of offering use cases to 
-   the users in order to help them become familiar with the tool. They are constantly updated, along with the updates 
-   and improvements of the tool itself.
+- **Simulation Engine Compatibility**: Uses [EnergyPlus Python API](https://energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus communication. Future plans include more engines like [OpenModelica](https://openmodelica.org/).
 
--  This project is accompanied by extensive **documentation**, **unit tests** and **github actions workflows** to make 
-   *Sinergym* an efficient ecosystem for both understanding and development.
+- **Benchmark Environments**: Designs environments for benchmarking and testing deep RL algorithms or other external strategies, similar to *Atari* or *Mujoco*.
 
--  Many more!
+- **Customizable Environments**: Allows easy modification of experimental settings. Users can create their own environments or modify pre-configured ones in *Sinergym*.
+
+- **Customizable Components**: Enables creation of new custom components for new environments, making *Sinergym* scalable, such as function rewards, wrappers, controllers, etc.
+
+- **Automatic Building Model Adaptation**: *Sinergym* automates the process of adapting the building model to user changes in the environment definition.
+
+- **Automatic Actuators Control**: Controls actuators through the Gymnasium interface based on user specification, only actuators names are required and *Sinergym* will do the rest.
+
+- **Extensive Environment Information**: Provides comprehensive information about *Sinergym* background components from the environment interface.
+
+- **Stable Baseline 3 Integration**: Customizes functionalities for easy testing of environments with SB3 algorithms, such as callbacks and customizable training real-time logging. However, *Sinergym* is agnostic to any DRL algorithm.
+
+- **Google Cloud Integration**: Offers guidance on using *Sinergym* with Google Cloud infrastructure.
+
+- **Weights & Biases Compatibility**: Automates and facilitates training, reproducibility, and comparison of agents in simulation-based building control problems. [WandB](https://wandb.ai/site) assists in managing and monitoring model lifecycle.
+
+- **Notebook Examples**: Provides code in notebook format for user familiarity with the tool.
+
+- **Extensive Documentation, Unit Tests, and GitHub Actions Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and development.
+
+- And much more!
 
 _This is a project in active development. Stay tuned for upcoming releases._
 
 <div align="center">
   <img src="images/operation_diagram.png"><br><br>
 </div>
 
-## Project structure
+## Project Structure
 
-This repository is organized in the next directories:
+This repository is organized into the following directories:
 
-- `sinergym/`: Here you will find all the source code that forms *Sinergym*: environment, modeling, simulator, and tools such as wrappers, reward functions, etc.
-- `docs/`: Online documentation, generated with Sphinx and using Restructured Text (RST).
-- `examples/`: Here there are a set of notebooks written in Jupyter format. Use cases are illustrated with Sinergym.
-- `tests/`: All the unit tests of Sinergym. Fixtures and checks are defined here in order to check that the tool is in a stable state.
-- `scripts/`: This folder contains scripts in which Sinergym is used. We can find useful things for the users, such as agent training, agent loading, performance checks, etc. In addition, these scripts allow a high margin of configuration using the JSON format.
+- `sinergym/`: Contains the source code for *Sinergym*, including the environment, modeling, simulator, and tools such as wrappers and reward functions.
+- `docs/`: Online documentation generated with Sphinx and using Restructured Text (RST).
+- `examples/`: Jupyter notebooks illustrating use cases with Sinergym.
+- `tests/`: Unit tests for Sinergym to ensure stability.
+- `scripts/`: Scripts for various tasks such as agent training and performance checks, allowing configuration using JSON format.
 
-## List of available environments
+## Available Environments
 
-If you would like to see a complete and updated list of our available environments, please visit [our list](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the official *Sinergym* documentation.
+For a complete and up-to-date list of available environments, please refer to [our documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#).
 
 ## Installation
 
-Please, visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more information about Sinergym installation.
+Please visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation instructions.
 
 ## Usage example
 
+
 If you used our Dockerfile during installation, you should have the *try_env.py* file in your workspace as soon as you enter in. In case you have installed everything on your local machine directly, place it inside our cloned repository. In any case, we start from the point that you have at your disposal a terminal with the appropriate python version and *Sinergym* running correctly.
 
-*Sinergym* uses the standard Gymnasium API. So basic loop should be something like:
+*Sinergym* uses the standard Gymnasium API. So a basic loop should look like:
 
 ```python
 
 import gymnasium as gym
 import sinergym
 # Create the environment
 env = gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1')
@@ -171,17 +130,18 @@
     a = env.action_space.sample() # random action selection
     obs, reward, terminated, truncated, info = env.step(a) # get new observation and reward
     R += reward
 print('Total reward for the episode: %.4f' % R)
 env.close()
 ```
 
-Notice that a folder will be created in the working directory after creating the environment. It will contain the EnergyPlus outputs produced during the simulation.
+A folder will be created in the working directory after creating the environment. It will contain the Sinergym outputs produced during the simulation.
+
+For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
-:pencil: For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
 ## Google Cloud Platform support
 
 For more information about this functionality, please, visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud).
 
 ## Projects using Sinergym
```

#### html2text {}

```diff
@@ -7,127 +7,84 @@
                                    _v_e_r_s_i_o_n_]
 
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_S_u_p_p_o_r_t_e_d_%_2_0_b_y_-_V_S_C_o_d_e_%_2_0_P_o_w_e_r_%_2_0_U_s_e_r_%_2_0_%_E_2_%_8_6_%_9_2_-
            _g_r_a_y_._s_v_g_?_c_o_l_o_r_A_=_6_5_5_B_E_1_&_c_o_l_o_r_B_=_4_F_4_4_D_6_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 **Welcome to Sinergym!**
                         [images/general_blueprint.png]
 
-The goal of this project is to create an environment following [Gymnasium
-interface](https://gymnasium.farama.org/), for wrapping simulation engines for
-building control using **deep reinforcement learning**. For more information
-about Sinergym, we recommend to visit our [documentation here](https://ugr-
-sail.github.io/sinergym/compilation/main/index.html). Please, help us to
-improve by **reporting your questions and issues** [here](https://github.com/
-ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates
-(questions, bugs, improvements, etc.). More detailed info on how to report
-issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/
-creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://
-github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking
-about contributing to Sinergym. The main functionalities of *Sinergym* are the
-following : - **Compatibility with simulation engines**. Communication between
-Python and [EnergyPlus](https://energyplus.net/) is established using
-[Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html)
-as a middleware. However, more of them (e.g. [OpenModelica](https://
-openmodelica.org/)) could be included in the backend while maintaining the
-Gymnasium API in the future. - **Benchmark environments**. Similarly to *Atari*
-or *Mujoco* environments for RL community, we are designing a set of
-environments for benchmarking and testing deep RL algorithms. These
-environments may include different buildings, weathers, action/observation
-spaces, function rewards, etc. - **Customizable environments**. We aim to
-provide a package which allows modifying experimental settings in an easy
-manner. The user can create his own environments, combining his own building
-model, weather, reward, observation/action space, variables, actuators,
-environment name, etc. The user can also use these pre-configured environments
-available in *Sinergym* and change some aspect of it (for example, the weather)
-in such a way that he does not have to make an entire definition of the
-environment and can start from one pre-designed by us. Some parameters directly
-associated with the simulator can be set as **extra configuration** as well,
-such as people occupant, time-steps per simulation hour, run-period, etc. -
-**Customizable components**. *Sinergym* is easily scalable by third parties.
-Following the structure of the implemented classes, new custom components can
-be created for new environments such as function rewards, wrappers,
-controllers, etc. - **Automatic Building Model adaptation to user changes**.
-Many of the updates to the environment definition require changes to the
-building model (*epJSON* file) to adapt it to these new features before the
-simulation starts, which *Sinergym* will perform automatically. For example,
-using another weather file requires building location and design days update,
-using new observation variables requires to update the `Output:Variable` and
-`Output:Meter` fields, the same occurs with extra configuration context
-concerned with simulation directly, if weather variability is set, then a
-weather with noise will be used. These new building and weather file versions,
-is saved in the *Sinergym* output folder, leaving the original intact. In
-short, *Sinergym* automates the whole process of model adaptation so that the
-user only has to define what he wants for his environment. - **Automatic
-actuators control**. Related to the above, it will only be necessary to specify
-the name of the actuators to be controlled through the actions of the Gymnasium
-interface, and *Sinergym* will take care of everything. - **Extensive
-environment information**. It is important that users can get some information
-about *Sinergym* background components from environment interface easily. From
-environment instance, it is possible to consult available schedulers, variables
-which compose an observation and action, whether simulator is running, the
-building run period, episode length, timesteps per episode, available building
-zones... And much more. - **Stable Baseline 3 Integration**. Some
-functionalities like callbacks have been customized by our team in order to
-test easily these environments with deep reinforcement learning algorithms and
-logger specific information about *Sinergym* environments. However, *Sinergym*
-is completely agnostic to any DRL algorithm and can be used with any DRL
-library that works with gymnasium interface. - **Google Cloud Integration**.
-Whether you have a Google Cloud account and you want to use your infrastructure
-with *Sinergym*, we tell you some details about how to do it. - **Weights &
-Biases tracking and visualization compatibility**. One of *Sinergym*'s
-objectives is to automate and facilitate the training, reproducibility and
-comparison of agents in simulation-based building control problems, managing
-and monitoring model lifecycle from training to deployment. [WandB](https://
-wandb.ai/site) is an open-source platform for the machine learning lifecycle
-helping us with this issue. It lets us register experiments hyperparameters,
-visualize data recorded in real-time, and store artifacts with experiment
-outputs and best obtained models. - **Notebooks examples**. *Sinergym* develops
-code in notebook format with the purpose of offering use cases to the users in
-order to help them become familiar with the tool. They are constantly updated,
-along with the updates and improvements of the tool itself. - This project is
-accompanied by extensive **documentation**, **unit tests** and **github actions
-workflows** to make *Sinergym* an efficient ecosystem for both understanding
-and development. - Many more! _This is a project in active development. Stay
+The goal of this project is to create an environment following *Gymnasium*
+interface for wrapping simulation engines (*EnergyPlus*) for building control
+using **deep reinforcement learning** or any external control. For more
+information about Sinergym, please visit our [documentation](https://ugr-
+sail.github.io/sinergym/compilation/main/index.html). To report questions and
+issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/
+issues). We appreciate your feedback and contributions. Check out our
+[CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/
+CONTRIBUTING.md) for more details on how to contribute. The main
+functionalities of *Sinergym* are the following: - **Simulation Engine
+Compatibility**: Uses [EnergyPlus Python API](https://
+energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus
+communication. Future plans include more engines like [OpenModelica](https://
+openmodelica.org/). - **Benchmark Environments**: Designs environments for
+benchmarking and testing deep RL algorithms or other external strategies,
+similar to *Atari* or *Mujoco*. - **Customizable Environments**: Allows easy
+modification of experimental settings. Users can create their own environments
+or modify pre-configured ones in *Sinergym*. - **Customizable Components**:
+Enables creation of new custom components for new environments, making
+*Sinergym* scalable, such as function rewards, wrappers, controllers, etc. -
+**Automatic Building Model Adaptation**: *Sinergym* automates the process of
+adapting the building model to user changes in the environment definition. -
+**Automatic Actuators Control**: Controls actuators through the Gymnasium
+interface based on user specification, only actuators names are required and
+*Sinergym* will do the rest. - **Extensive Environment Information**: Provides
+comprehensive information about *Sinergym* background components from the
+environment interface. - **Stable Baseline 3 Integration**: Customizes
+functionalities for easy testing of environments with SB3 algorithms, such as
+callbacks and customizable training real-time logging. However, *Sinergym* is
+agnostic to any DRL algorithm. - **Google Cloud Integration**: Offers guidance
+on using *Sinergym* with Google Cloud infrastructure. - **Weights & Biases
+Compatibility**: Automates and facilitates training, reproducibility, and
+comparison of agents in simulation-based building control problems. [WandB]
+(https://wandb.ai/site) assists in managing and monitoring model lifecycle. -
+**Notebook Examples**: Provides code in notebook format for user familiarity
+with the tool. - **Extensive Documentation, Unit Tests, and GitHub Actions
+Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and
+development. - And much more! _This is a project in active development. Stay
 tuned for upcoming releases._
                         [images/operation_diagram.png]
 
-## Project structure This repository is organized in the next directories: -
-`sinergym/`: Here you will find all the source code that forms *Sinergym*:
-environment, modeling, simulator, and tools such as wrappers, reward functions,
-etc. - `docs/`: Online documentation, generated with Sphinx and using
-Restructured Text (RST). - `examples/`: Here there are a set of notebooks
-written in Jupyter format. Use cases are illustrated with Sinergym. - `tests/`:
-All the unit tests of Sinergym. Fixtures and checks are defined here in order
-to check that the tool is in a stable state. - `scripts/`: This folder contains
-scripts in which Sinergym is used. We can find useful things for the users,
-such as agent training, agent loading, performance checks, etc. In addition,
-these scripts allow a high margin of configuration using the JSON format. ##
-List of available environments If you would like to see a complete and updated
-list of our available environments, please visit [our list](https://ugr-
-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the
-official *Sinergym* documentation. ## Installation Please, visit [INSTALL.md]
-(https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more
-information about Sinergym installation. ## Usage example If you used our
-Dockerfile during installation, you should have the *try_env.py* file in your
-workspace as soon as you enter in. In case you have installed everything on
-your local machine directly, place it inside our cloned repository. In any
-case, we start from the point that you have at your disposal a terminal with
-the appropriate python version and *Sinergym* running correctly. *Sinergym*
-uses the standard Gymnasium API. So basic loop should be something like:
-```python import gymnasium as gym import sinergym # Create the environment env
-= gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the
-episode obs, info = env.reset() truncated = terminated = False R = 0.0 while
-not (terminated or truncated): a = env.action_space.sample() # random action
-selection obs, reward, terminated, truncated, info = env.step(a) # get new
-observation and reward R += reward print('Total reward for the episode: %.4f' %
-R) env.close() ``` Notice that a folder will be created in the working
-directory after creating the environment. It will contain the EnergyPlus
-outputs produced during the simulation. :pencil: For more examples and details,
-please visit our [usage examples](https://ugr-sail.github.io/sinergym/
-compilation/main/pages/notebooks/basic_example.html#Basic-example)
+## Project Structure This repository is organized into the following
+directories: - `sinergym/`: Contains the source code for *Sinergym*, including
+the environment, modeling, simulator, and tools such as wrappers and reward
+functions. - `docs/`: Online documentation generated with Sphinx and using
+Restructured Text (RST). - `examples/`: Jupyter notebooks illustrating use
+cases with Sinergym. - `tests/`: Unit tests for Sinergym to ensure stability. -
+`scripts/`: Scripts for various tasks such as agent training and performance
+checks, allowing configuration using JSON format. ## Available Environments For
+a complete and up-to-date list of available environments, please refer to [our
+documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/
+environments.html#). ## Installation Please visit [INSTALL.md](https://
+github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation
+instructions. ## Usage example If you used our Dockerfile during installation,
+you should have the *try_env.py* file in your workspace as soon as you enter
+in. In case you have installed everything on your local machine directly, place
+it inside our cloned repository. In any case, we start from the point that you
+have at your disposal a terminal with the appropriate python version and
+*Sinergym* running correctly. *Sinergym* uses the standard Gymnasium API. So a
+basic loop should look like: ```python import gymnasium as gym import sinergym
+# Create the environment env = gym.make('Eplus-datacenter-mixed-continuous-
+stochastic-v1') # Initialize the episode obs, info = env.reset() truncated =
+terminated = False R = 0.0 while not (terminated or truncated): a =
+env.action_space.sample() # random action selection obs, reward, terminated,
+truncated, info = env.step(a) # get new observation and reward R += reward
+print('Total reward for the episode: %.4f' % R) env.close() ``` A folder will
+be created in the working directory after creating the environment. It will
+contain the Sinergym outputs produced during the simulation. For more examples
+and details, please visit our [usage examples](https://ugr-sail.github.io/
+sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example)
 documentation section. ## Google Cloud Platform support For more information
 about this functionality, please, visit our documentation [here](https://ugr-
 sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-
 google-cloud). ## Projects using Sinergym The following are some of the
 projects benefiting from the advantages of Sinergym: - [Demosthen/ActiveRL]
 (https://github.com/Demosthen/ActiveRL) - [VectorInstitute/HV-Ai-C](https://
 github.com/VectorInstitute/HV-Ai-C) - [rdnfn/beobench](https://github.com/
```

### Comparing `sinergym-3.2.7/setup.py` & `sinergym-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/__init__.py` & `sinergym-3.3.0/sinergym/__init__.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/config/modeling.py` & `sinergym-3.3.0/sinergym/config/modeling.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/1ZoneDataCenterCRAC_wApproachTemp.epJSON`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9979508196721312%*

 * *Differences: {"'Output:VariableDictionary'": "{'Output:VariableDictionary 1': {'key_field': 'regular'}}"}*

```diff
@@ -1107,15 +1107,15 @@
             "key_value": "*",
             "reporting_frequency": "Hourly",
             "variable_name": "Performance Curve Output Value"
         }
     },
     "Output:VariableDictionary": {
         "Output:VariableDictionary 1": {
-            "key_field": "IDF"
+            "key_field": "regular"
         }
     },
     "OutputControl:Table:Style": {
         "OutputControl:Table:Style 1": {
             "column_separator": "HTML"
         }
     },
```

### Comparing `sinergym-3.2.7/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/2ZoneDataCenterHVAC_wEconomizer.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/5ZoneAutoDXVAV.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/ASHRAE901_OfficeMedium_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/ASHRAE901_Warehouse_STD2019_Denver.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/LrgOff_GridStorageScheduled.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/ShopWithPVandBattery.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/ShopWithPVandBattery.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/buildings/radiant_residential_building.epJSON` & `sinergym-3.3.0/sinergym/data/buildings/radiant_residential_building.epJSON`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json` & `sinergym-3.3.0/sinergym/data/default_configuration/1ZoneDataCenterCRAC_wApproachTemp.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json` & `sinergym-3.3.0/sinergym/data/default_configuration/2ZoneDataCenterHVAC_wEconomizer.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990079365079365%*

 * *Differences: {"'reward_kwargs'": "{'temperature_variables': {delete: [1]}}"}*

```diff
@@ -39,16 +39,15 @@
             30
         ],
         "summer_start": [
             6,
             1
         ],
         "temperature_variables": [
-            "west_zone_air_temperature",
-            "east_zone_air_temperature"
+            "west_zone_air_temperature"
         ]
     },
     "time_variables": [
         "month",
         "day_of_month",
         "hour"
     ],
```

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/5ZoneAutoDXVAV.json` & `sinergym-3.3.0/sinergym/data/default_configuration/5ZoneAutoDXVAV.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json` & `sinergym-3.3.0/sinergym/data/default_configuration/ASHRAE901_OfficeMedium_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json` & `sinergym-3.3.0/sinergym/data/default_configuration/ASHRAE901_Warehouse_STD2019_Denver.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json` & `sinergym-3.3.0/sinergym/data/default_configuration/LrgOff_GridStorageScheduled.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/ShopWithPVandBattery.json` & `sinergym-3.3.0/sinergym/data/default_configuration/ShopWithPVandBattery.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/default_configuration/radiant_residential_building.json` & `sinergym-3.3.0/sinergym/data/default_configuration/radiant_residential_building.json`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/AUS_NSW.Sydney.947670_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/COL_Bogota.802220_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/COL_Bogota.802220_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/ESP_Granada.084190_SWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/ESP_Granada.084190_SWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/FIN_Helsinki.029740_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/JPN_Tokyo.Hyakuri.477150_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/MDG_Antananarivo.670830_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy` & `sinergym-3.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw` & `sinergym-3.3.0/sinergym/data/weather/PRT_Lisboa.085360_INETI.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy` & `sinergym-3.3.0/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw` & `sinergym-3.3.0/sinergym/data/weather/SWE_Stockholm.Arlanda.024600_IWEC.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_AZ_Davis-Monthan.AFB.722745_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_CO_Aurora-Buckley.Field.ANGB.724695_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_IL_Chicago-OHare.Intl.AP.725300_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_NY_New.York-J.F.Kennedy.Intl.AP.744860_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_PA_Pittsburgh-Allegheny.County.AP.725205_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy` & `sinergym-3.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.ddy`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw` & `sinergym-3.3.0/sinergym/data/weather/USA_WA_Port.Angeles-William.R.Fairchild.Intl.AP.727885_TMY3.epw`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/envs/eplus_env.py` & `sinergym-3.3.0/sinergym/envs/eplus_env.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/simulators/eplus.py` & `sinergym-3.3.0/sinergym/simulators/eplus.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/callbacks.py` & `sinergym-3.3.0/sinergym/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/common.py` & `sinergym-3.3.0/sinergym/utils/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,24 +289,24 @@
                     prename = prename + '_'
                     output[prename +
                            specification['variable_names']] = (variable, key)
 
             else:
                 raise RuntimeError
 
-        elif isinstance(specification['variables_names'], list):
+        elif isinstance(specification['variable_names'], list):
 
             if isinstance(specification['keys'], str):
                 raise RuntimeError
 
             elif isinstance(specification['keys'], list):
-                assert len( specification['variables_names']) == len(
+                assert len( specification['variable_names']) == len(
                     specification['keys']), 'variable names and keys must have the same len in {}'.format(variable)
                 for variable_name, key_name in list(
-                        zip(specification['variables_names'], specification['keys'])):
+                        zip(specification['variable_names'], specification['keys'])):
                     output[variable_name] = (variable, key_name)
 
             else:
                 raise RuntimeError
 
         else:
```

### Comparing `sinergym-3.2.7/sinergym/utils/constants.py` & `sinergym-3.3.0/sinergym/utils/constants.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/controllers.py` & `sinergym-3.3.0/sinergym/utils/controllers.py`

 * *Files 19% similar despite different names*

```diff
@@ -76,14 +76,41 @@
 
 
 class RBCDatacenter(object):
 
     def __init__(self, env: EplusEnv) -> None:
         """Agent based on static rules for controlling 2ZoneDataCenterHVAC setpoints.
         Follows the ASHRAE recommended temperature ranges for data centers described in ASHRAE TC9.9 (2016).
+
+        Args:
+            env (EplusEnv): Simulation environment
+        """
+
+        self.env = env
+        self.observation_variables = env.get_wrapper_attr(
+            'observation_variables')
+        self.action_variables = env.get_wrapper_attr('action_variables')
+
+        # ASHRAE recommended temperature range = [18, 27] Celsius
+        self.range_datacenter = (18, 27)
+
+    def act(self) -> Sequence[Any]:
+        """Select same action always, corresponding with comfort range.
+
+        Returns:
+            Sequence[Any]: Action chosen.
+        """
+        return self.range_datacenter
+
+
+class RBCIncrementalDatacenter(object):
+
+    def __init__(self, env: EplusEnv) -> None:
+        """Agent based on rules for controlling 2ZoneDataCenterHVAC setpoints in a incremental way.
+        Follows the ASHRAE recommended temperature ranges for data centers described in ASHRAE TC9.9 (2016).
         Args:
             env (EplusEnv): Simulation environment
         """
 
         self.env = env
         self.observation_variables = env.get_wrapper_attr(
             'observation_variables')
```

### Comparing `sinergym-3.2.7/sinergym/utils/env_checker.py` & `sinergym-3.3.0/sinergym/utils/env_checker.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/evaluation.py` & `sinergym-3.3.0/sinergym/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/gcloud.py` & `sinergym-3.3.0/sinergym/utils/gcloud.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/logger.py` & `sinergym-3.3.0/sinergym/utils/logger.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/rewards.py` & `sinergym-3.3.0/sinergym/utils/rewards.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym/utils/wrappers.py` & `sinergym-3.3.0/sinergym/utils/wrappers.py`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym.egg-info/PKG-INFO` & `sinergym-3.3.0/sinergym.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sinergym
-Version: 3.2.7
+Version: 3.3.0
 Summary: The goal of sinergym is to create an environment following OpenAI Gym interface for wrapping simulation engines for building control using deep reinforcement learning.
 Home-page: https://github.com/ugr-sail/sinergym
 Author: J. Jiménez, J. Gómez, M. Molina, A. Manjavacas, A. Campoy
 Author-email: alejandroac79@gmail.com
 License: MIT
 Keywords: control reinforcement-learning buildings reinforcement-learning-environments
 Platform: UNKNOWN
@@ -68,121 +68,80 @@
 
 **Welcome to Sinergym!**
 
 <div align="center">
   <img src="images/general_blueprint.png" width=80%><br><br>
 </div>
 
-The goal of this project is to create an environment following [Gymnasium interface](https://gymnasium.farama.org/), for wrapping simulation engines for building control using **deep reinforcement learning**.
+The goal of this project is to create an environment following *Gymnasium* interface for wrapping 
+simulation engines (*EnergyPlus*) for building control using **deep reinforcement learning** 
+or any external control.
 
-For more information about Sinergym, we recommend to visit our [documentation here](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
+For more information about Sinergym, please visit our [documentation](https://ugr-sail.github.io/sinergym/compilation/main/index.html).
 
-Please, help us to improve by **reporting your questions and issues** [here](https://github.com/ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates (questions, bugs, improvements, etc.). More detailed info on how to report issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking about contributing to Sinergym.
+To report questions and issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/issues). We appreciate your feedback and contributions. Check out our [CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) for more details on how to contribute.
 
-The main functionalities of *Sinergym* are the following :
+The main functionalities of *Sinergym* are the following:
 
--  **Compatibility with simulation engines**. Communication between
-   Python and [EnergyPlus](https://energyplus.net/) is established
-   using [Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html) as a middleware.
-   However, more of them (e.g.
-   [OpenModelica](https://openmodelica.org/)) could be included in
-   the backend while maintaining the Gymnasium API in the future.
-
--  **Benchmark environments**. Similarly to *Atari* or *Mujoco* environments
-   for RL community, we are designing a set of environments for
-   benchmarking and testing deep RL algorithms. These environments may
-   include different buildings, weathers, action/observation spaces, function rewards, etc.
-
--  **Customizable environments**. We aim to provide a
-   package which allows modifying experimental settings in an easy
-   manner. The user can create his own environments, combining his own
-   building model, weather, reward, observation/action space, variables, actuators, environment name, etc.
-   The user can also use these pre-configured environments available in *Sinergym* 
-   and change some aspect of it (for example, the weather) in such 
-   a way that he does not  have to make an entire definition of the 
-   environment and can start from one pre-designed by us.
-   Some parameters directly associated with the simulator can be set as **extra configuration** 
-   as well, such as people occupant, time-steps per simulation hour, run-period, etc.
-
--  **Customizable components**. *Sinergym* is easily scalable by third parties.
-   Following the structure of the implemented classes, new custom components 
-   can be created for new environments such as function rewards, wrappers,
-   controllers, etc.
-
--  **Automatic Building Model adaptation to user changes**. Many of the updates to the environment definition require changes 
-   to the building model (*epJSON* file) to adapt it to these new features before the simulation starts, which *Sinergym* will 
-   perform automatically. For example, using another weather file requires building location and design days update, using new 
-   observation variables requires to update the `Output:Variable` and `Output:Meter` fields, the same occurs with extra 
-   configuration context concerned with simulation directly, if weather variability is set, then a weather with noise 
-   will be used. These new building and weather file versions, is saved in the *Sinergym* output folder, leaving the original 
-   intact. In short, *Sinergym* automates the whole process of model adaptation so that the user 
-   only has to define what he wants for his environment.
-
--  **Automatic actuators control**. Related to the above, it will only be necessary to specify the name of the actuators to be controlled 
-   through the actions of the Gymnasium interface, and *Sinergym* will take care of everything.
-
--  **Extensive environment information**. It is important that users can get some information about *Sinergym* background components from environment interface easily.
-   From environment instance, it is possible to consult available schedulers, variables which compose an observation and action, whether simulator is running,
-   the building run period, episode length, timesteps per episode, available building zones... And much more.
-
--  **Stable Baseline 3 Integration**. Some functionalities like callbacks
-   have been customized by our team in order to test easily these environments
-   with deep reinforcement learning algorithms and logger specific information about 
-   *Sinergym* environments. 
-   However, *Sinergym* is completely agnostic to any DRL algorithm and can be used with any DRL 
-   library that works with gymnasium interface.
-
--  **Google Cloud Integration**. Whether you have a Google Cloud account and you want to
-   use your infrastructure with *Sinergym*, we tell you some details about how to do it.
-
--  **Weights & Biases tracking and visualization compatibility**. One of *Sinergym*'s objectives is to automate
-   and facilitate the training, reproducibility and comparison of agents in simulation-based 
-   building control problems, managing and monitoring model lifecycle from training to deployment. [WandB](https://wandb.ai/site)
-   is an open-source platform for the machine learning lifecycle helping us with this issue. 
-   It lets us register experiments hyperparameters, visualize data recorded in real-time, 
-   and store artifacts with experiment outputs and best obtained models. 
-
--  **Notebooks examples**. *Sinergym* develops code in notebook format with the purpose of offering use cases to 
-   the users in order to help them become familiar with the tool. They are constantly updated, along with the updates 
-   and improvements of the tool itself.
+- **Simulation Engine Compatibility**: Uses [EnergyPlus Python API](https://energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus communication. Future plans include more engines like [OpenModelica](https://openmodelica.org/).
 
--  This project is accompanied by extensive **documentation**, **unit tests** and **github actions workflows** to make 
-   *Sinergym* an efficient ecosystem for both understanding and development.
+- **Benchmark Environments**: Designs environments for benchmarking and testing deep RL algorithms or other external strategies, similar to *Atari* or *Mujoco*.
 
--  Many more!
+- **Customizable Environments**: Allows easy modification of experimental settings. Users can create their own environments or modify pre-configured ones in *Sinergym*.
+
+- **Customizable Components**: Enables creation of new custom components for new environments, making *Sinergym* scalable, such as function rewards, wrappers, controllers, etc.
+
+- **Automatic Building Model Adaptation**: *Sinergym* automates the process of adapting the building model to user changes in the environment definition.
+
+- **Automatic Actuators Control**: Controls actuators through the Gymnasium interface based on user specification, only actuators names are required and *Sinergym* will do the rest.
+
+- **Extensive Environment Information**: Provides comprehensive information about *Sinergym* background components from the environment interface.
+
+- **Stable Baseline 3 Integration**: Customizes functionalities for easy testing of environments with SB3 algorithms, such as callbacks and customizable training real-time logging. However, *Sinergym* is agnostic to any DRL algorithm.
+
+- **Google Cloud Integration**: Offers guidance on using *Sinergym* with Google Cloud infrastructure.
+
+- **Weights & Biases Compatibility**: Automates and facilitates training, reproducibility, and comparison of agents in simulation-based building control problems. [WandB](https://wandb.ai/site) assists in managing and monitoring model lifecycle.
+
+- **Notebook Examples**: Provides code in notebook format for user familiarity with the tool.
+
+- **Extensive Documentation, Unit Tests, and GitHub Actions Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and development.
+
+- And much more!
 
 _This is a project in active development. Stay tuned for upcoming releases._
 
 <div align="center">
   <img src="images/operation_diagram.png"><br><br>
 </div>
 
-## Project structure
+## Project Structure
 
-This repository is organized in the next directories:
+This repository is organized into the following directories:
 
-- `sinergym/`: Here you will find all the source code that forms *Sinergym*: environment, modeling, simulator, and tools such as wrappers, reward functions, etc.
-- `docs/`: Online documentation, generated with Sphinx and using Restructured Text (RST).
-- `examples/`: Here there are a set of notebooks written in Jupyter format. Use cases are illustrated with Sinergym.
-- `tests/`: All the unit tests of Sinergym. Fixtures and checks are defined here in order to check that the tool is in a stable state.
-- `scripts/`: This folder contains scripts in which Sinergym is used. We can find useful things for the users, such as agent training, agent loading, performance checks, etc. In addition, these scripts allow a high margin of configuration using the JSON format.
+- `sinergym/`: Contains the source code for *Sinergym*, including the environment, modeling, simulator, and tools such as wrappers and reward functions.
+- `docs/`: Online documentation generated with Sphinx and using Restructured Text (RST).
+- `examples/`: Jupyter notebooks illustrating use cases with Sinergym.
+- `tests/`: Unit tests for Sinergym to ensure stability.
+- `scripts/`: Scripts for various tasks such as agent training and performance checks, allowing configuration using JSON format.
 
-## List of available environments
+## Available Environments
 
-If you would like to see a complete and updated list of our available environments, please visit [our list](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the official *Sinergym* documentation.
+For a complete and up-to-date list of available environments, please refer to [our documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/environments.html#).
 
 ## Installation
 
-Please, visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more information about Sinergym installation.
+Please visit [INSTALL.md](https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation instructions.
 
 ## Usage example
 
+
 If you used our Dockerfile during installation, you should have the *try_env.py* file in your workspace as soon as you enter in. In case you have installed everything on your local machine directly, place it inside our cloned repository. In any case, we start from the point that you have at your disposal a terminal with the appropriate python version and *Sinergym* running correctly.
 
-*Sinergym* uses the standard Gymnasium API. So basic loop should be something like:
+*Sinergym* uses the standard Gymnasium API. So a basic loop should look like:
 
 ```python
 
 import gymnasium as gym
 import sinergym
 # Create the environment
 env = gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1')
@@ -194,17 +153,18 @@
     a = env.action_space.sample() # random action selection
     obs, reward, terminated, truncated, info = env.step(a) # get new observation and reward
     R += reward
 print('Total reward for the episode: %.4f' % R)
 env.close()
 ```
 
-Notice that a folder will be created in the working directory after creating the environment. It will contain the EnergyPlus outputs produced during the simulation.
+A folder will be created in the working directory after creating the environment. It will contain the Sinergym outputs produced during the simulation.
+
+For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
-:pencil: For more examples and details, please visit our [usage examples](https://ugr-sail.github.io/sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example) documentation section.
 
 ## Google Cloud Platform support
 
 For more information about this functionality, please, visit our documentation [here](https://ugr-sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-google-cloud).
 
 ## Projects using Sinergym
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sinergym Version: 3.2.7 Summary: The goal of
+Metadata-Version: 2.1 Name: sinergym Version: 3.3.0 Summary: The goal of
 sinergym is to create an environment following OpenAI Gym interface for
 wrapping simulation engines for building control using deep reinforcement
 learning. Home-page: https://github.com/ugr-sail/sinergym Author: J. JimÃ©nez,
 J. GÃ³mez, M. Molina, A. Manjavacas, A. Campoy Author-email:
 alejandroac79@gmail.com License: MIT Keywords: control reinforcement-learning
 buildings reinforcement-learning-environments Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: Programming Language ::
@@ -19,127 +19,84 @@
                                    _v_e_r_s_i_o_n_]
 
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_S_u_p_p_o_r_t_e_d_%_2_0_b_y_-_V_S_C_o_d_e_%_2_0_P_o_w_e_r_%_2_0_U_s_e_r_%_2_0_%_E_2_%_8_6_%_9_2_-
            _g_r_a_y_._s_v_g_?_c_o_l_o_r_A_=_6_5_5_B_E_1_&_c_o_l_o_r_B_=_4_F_4_4_D_6_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 **Welcome to Sinergym!**
                         [images/general_blueprint.png]
 
-The goal of this project is to create an environment following [Gymnasium
-interface](https://gymnasium.farama.org/), for wrapping simulation engines for
-building control using **deep reinforcement learning**. For more information
-about Sinergym, we recommend to visit our [documentation here](https://ugr-
-sail.github.io/sinergym/compilation/main/index.html). Please, help us to
-improve by **reporting your questions and issues** [here](https://github.com/
-ugr-sail/sinergym/issues). It is easy, just 2 clicks using our issue templates
-(questions, bugs, improvements, etc.). More detailed info on how to report
-issues [here](https://docs.github.com/en/issues/tracking-your-work-with-issues/
-creating-an-issue). Don't forget to take a look at [CONTRIBUTING.md](https://
-github.com/ugr-sail/sinergym/blob/main/CONTRIBUTING.md) if you're thinking
-about contributing to Sinergym. The main functionalities of *Sinergym* are the
-following : - **Compatibility with simulation engines**. Communication between
-Python and [EnergyPlus](https://energyplus.net/) is established using
-[Energyplus Python API](https://energyplus.readthedocs.io/en/latest/api.html)
-as a middleware. However, more of them (e.g. [OpenModelica](https://
-openmodelica.org/)) could be included in the backend while maintaining the
-Gymnasium API in the future. - **Benchmark environments**. Similarly to *Atari*
-or *Mujoco* environments for RL community, we are designing a set of
-environments for benchmarking and testing deep RL algorithms. These
-environments may include different buildings, weathers, action/observation
-spaces, function rewards, etc. - **Customizable environments**. We aim to
-provide a package which allows modifying experimental settings in an easy
-manner. The user can create his own environments, combining his own building
-model, weather, reward, observation/action space, variables, actuators,
-environment name, etc. The user can also use these pre-configured environments
-available in *Sinergym* and change some aspect of it (for example, the weather)
-in such a way that he does not have to make an entire definition of the
-environment and can start from one pre-designed by us. Some parameters directly
-associated with the simulator can be set as **extra configuration** as well,
-such as people occupant, time-steps per simulation hour, run-period, etc. -
-**Customizable components**. *Sinergym* is easily scalable by third parties.
-Following the structure of the implemented classes, new custom components can
-be created for new environments such as function rewards, wrappers,
-controllers, etc. - **Automatic Building Model adaptation to user changes**.
-Many of the updates to the environment definition require changes to the
-building model (*epJSON* file) to adapt it to these new features before the
-simulation starts, which *Sinergym* will perform automatically. For example,
-using another weather file requires building location and design days update,
-using new observation variables requires to update the `Output:Variable` and
-`Output:Meter` fields, the same occurs with extra configuration context
-concerned with simulation directly, if weather variability is set, then a
-weather with noise will be used. These new building and weather file versions,
-is saved in the *Sinergym* output folder, leaving the original intact. In
-short, *Sinergym* automates the whole process of model adaptation so that the
-user only has to define what he wants for his environment. - **Automatic
-actuators control**. Related to the above, it will only be necessary to specify
-the name of the actuators to be controlled through the actions of the Gymnasium
-interface, and *Sinergym* will take care of everything. - **Extensive
-environment information**. It is important that users can get some information
-about *Sinergym* background components from environment interface easily. From
-environment instance, it is possible to consult available schedulers, variables
-which compose an observation and action, whether simulator is running, the
-building run period, episode length, timesteps per episode, available building
-zones... And much more. - **Stable Baseline 3 Integration**. Some
-functionalities like callbacks have been customized by our team in order to
-test easily these environments with deep reinforcement learning algorithms and
-logger specific information about *Sinergym* environments. However, *Sinergym*
-is completely agnostic to any DRL algorithm and can be used with any DRL
-library that works with gymnasium interface. - **Google Cloud Integration**.
-Whether you have a Google Cloud account and you want to use your infrastructure
-with *Sinergym*, we tell you some details about how to do it. - **Weights &
-Biases tracking and visualization compatibility**. One of *Sinergym*'s
-objectives is to automate and facilitate the training, reproducibility and
-comparison of agents in simulation-based building control problems, managing
-and monitoring model lifecycle from training to deployment. [WandB](https://
-wandb.ai/site) is an open-source platform for the machine learning lifecycle
-helping us with this issue. It lets us register experiments hyperparameters,
-visualize data recorded in real-time, and store artifacts with experiment
-outputs and best obtained models. - **Notebooks examples**. *Sinergym* develops
-code in notebook format with the purpose of offering use cases to the users in
-order to help them become familiar with the tool. They are constantly updated,
-along with the updates and improvements of the tool itself. - This project is
-accompanied by extensive **documentation**, **unit tests** and **github actions
-workflows** to make *Sinergym* an efficient ecosystem for both understanding
-and development. - Many more! _This is a project in active development. Stay
+The goal of this project is to create an environment following *Gymnasium*
+interface for wrapping simulation engines (*EnergyPlus*) for building control
+using **deep reinforcement learning** or any external control. For more
+information about Sinergym, please visit our [documentation](https://ugr-
+sail.github.io/sinergym/compilation/main/index.html). To report questions and
+issues, please use our [issue tracker](https://github.com/ugr-sail/sinergym/
+issues). We appreciate your feedback and contributions. Check out our
+[CONTRIBUTING.md](https://github.com/ugr-sail/sinergym/blob/main/
+CONTRIBUTING.md) for more details on how to contribute. The main
+functionalities of *Sinergym* are the following: - **Simulation Engine
+Compatibility**: Uses [EnergyPlus Python API](https://
+energyplus.readthedocs.io/en/latest/api.html) for Python-EnergyPlus
+communication. Future plans include more engines like [OpenModelica](https://
+openmodelica.org/). - **Benchmark Environments**: Designs environments for
+benchmarking and testing deep RL algorithms or other external strategies,
+similar to *Atari* or *Mujoco*. - **Customizable Environments**: Allows easy
+modification of experimental settings. Users can create their own environments
+or modify pre-configured ones in *Sinergym*. - **Customizable Components**:
+Enables creation of new custom components for new environments, making
+*Sinergym* scalable, such as function rewards, wrappers, controllers, etc. -
+**Automatic Building Model Adaptation**: *Sinergym* automates the process of
+adapting the building model to user changes in the environment definition. -
+**Automatic Actuators Control**: Controls actuators through the Gymnasium
+interface based on user specification, only actuators names are required and
+*Sinergym* will do the rest. - **Extensive Environment Information**: Provides
+comprehensive information about *Sinergym* background components from the
+environment interface. - **Stable Baseline 3 Integration**: Customizes
+functionalities for easy testing of environments with SB3 algorithms, such as
+callbacks and customizable training real-time logging. However, *Sinergym* is
+agnostic to any DRL algorithm. - **Google Cloud Integration**: Offers guidance
+on using *Sinergym* with Google Cloud infrastructure. - **Weights & Biases
+Compatibility**: Automates and facilitates training, reproducibility, and
+comparison of agents in simulation-based building control problems. [WandB]
+(https://wandb.ai/site) assists in managing and monitoring model lifecycle. -
+**Notebook Examples**: Provides code in notebook format for user familiarity
+with the tool. - **Extensive Documentation, Unit Tests, and GitHub Actions
+Workflows**: Ensures *Sinergym* is an efficient ecosystem for understanding and
+development. - And much more! _This is a project in active development. Stay
 tuned for upcoming releases._
                         [images/operation_diagram.png]
 
-## Project structure This repository is organized in the next directories: -
-`sinergym/`: Here you will find all the source code that forms *Sinergym*:
-environment, modeling, simulator, and tools such as wrappers, reward functions,
-etc. - `docs/`: Online documentation, generated with Sphinx and using
-Restructured Text (RST). - `examples/`: Here there are a set of notebooks
-written in Jupyter format. Use cases are illustrated with Sinergym. - `tests/`:
-All the unit tests of Sinergym. Fixtures and checks are defined here in order
-to check that the tool is in a stable state. - `scripts/`: This folder contains
-scripts in which Sinergym is used. We can find useful things for the users,
-such as agent training, agent loading, performance checks, etc. In addition,
-these scripts allow a high margin of configuration using the JSON format. ##
-List of available environments If you would like to see a complete and updated
-list of our available environments, please visit [our list](https://ugr-
-sail.github.io/sinergym/compilation/main/pages/environments.html#) in the
-official *Sinergym* documentation. ## Installation Please, visit [INSTALL.md]
-(https://github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for more
-information about Sinergym installation. ## Usage example If you used our
-Dockerfile during installation, you should have the *try_env.py* file in your
-workspace as soon as you enter in. In case you have installed everything on
-your local machine directly, place it inside our cloned repository. In any
-case, we start from the point that you have at your disposal a terminal with
-the appropriate python version and *Sinergym* running correctly. *Sinergym*
-uses the standard Gymnasium API. So basic loop should be something like:
-```python import gymnasium as gym import sinergym # Create the environment env
-= gym.make('Eplus-datacenter-mixed-continuous-stochastic-v1') # Initialize the
-episode obs, info = env.reset() truncated = terminated = False R = 0.0 while
-not (terminated or truncated): a = env.action_space.sample() # random action
-selection obs, reward, terminated, truncated, info = env.step(a) # get new
-observation and reward R += reward print('Total reward for the episode: %.4f' %
-R) env.close() ``` Notice that a folder will be created in the working
-directory after creating the environment. It will contain the EnergyPlus
-outputs produced during the simulation. :pencil: For more examples and details,
-please visit our [usage examples](https://ugr-sail.github.io/sinergym/
-compilation/main/pages/notebooks/basic_example.html#Basic-example)
+## Project Structure This repository is organized into the following
+directories: - `sinergym/`: Contains the source code for *Sinergym*, including
+the environment, modeling, simulator, and tools such as wrappers and reward
+functions. - `docs/`: Online documentation generated with Sphinx and using
+Restructured Text (RST). - `examples/`: Jupyter notebooks illustrating use
+cases with Sinergym. - `tests/`: Unit tests for Sinergym to ensure stability. -
+`scripts/`: Scripts for various tasks such as agent training and performance
+checks, allowing configuration using JSON format. ## Available Environments For
+a complete and up-to-date list of available environments, please refer to [our
+documentation](https://ugr-sail.github.io/sinergym/compilation/main/pages/
+environments.html#). ## Installation Please visit [INSTALL.md](https://
+github.com/ugr-sail/sinergym/blob/main/INSTALL.md) for detailed installation
+instructions. ## Usage example If you used our Dockerfile during installation,
+you should have the *try_env.py* file in your workspace as soon as you enter
+in. In case you have installed everything on your local machine directly, place
+it inside our cloned repository. In any case, we start from the point that you
+have at your disposal a terminal with the appropriate python version and
+*Sinergym* running correctly. *Sinergym* uses the standard Gymnasium API. So a
+basic loop should look like: ```python import gymnasium as gym import sinergym
+# Create the environment env = gym.make('Eplus-datacenter-mixed-continuous-
+stochastic-v1') # Initialize the episode obs, info = env.reset() truncated =
+terminated = False R = 0.0 while not (terminated or truncated): a =
+env.action_space.sample() # random action selection obs, reward, terminated,
+truncated, info = env.step(a) # get new observation and reward R += reward
+print('Total reward for the episode: %.4f' % R) env.close() ``` A folder will
+be created in the working directory after creating the environment. It will
+contain the Sinergym outputs produced during the simulation. For more examples
+and details, please visit our [usage examples](https://ugr-sail.github.io/
+sinergym/compilation/main/pages/notebooks/basic_example.html#Basic-example)
 documentation section. ## Google Cloud Platform support For more information
 about this functionality, please, visit our documentation [here](https://ugr-
 sail.github.io/sinergym/compilation/main/pages/gcloudAPI.html#sinergym-with-
 google-cloud). ## Projects using Sinergym The following are some of the
 projects benefiting from the advantages of Sinergym: - [Demosthen/ActiveRL]
 (https://github.com/Demosthen/ActiveRL) - [VectorInstitute/HV-Ai-C](https://
 github.com/VectorInstitute/HV-Ai-C) - [rdnfn/beobench](https://github.com/
```

### Comparing `sinergym-3.2.7/sinergym.egg-info/SOURCES.txt` & `sinergym-3.3.0/sinergym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sinergym-3.2.7/sinergym.egg-info/requires.txt` & `sinergym-3.3.0/sinergym.egg-info/requires.txt`

 * *Files identical despite different names*

