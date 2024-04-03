# Comparing `tmp/nautobot_golden_config-2.0.3.tar.gz` & `tmp/nautobot_golden_config-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_golden_config-2.0.3.tar", max compression
+gzip compressed data, was "nautobot_golden_config-2.0.4.tar", max compression
```

## Comparing `nautobot_golden_config-2.0.3.tar` & `nautobot_golden_config-2.0.4.tar`

### file list

```diff
@@ -1,291 +1,295 @@
--rw-r--r--   0        0        0      591 2024-03-14 22:43:21.907631 nautobot_golden_config-2.0.3/LICENSE
--rw-r--r--   0        0        0     7047 2024-03-14 22:43:21.907631 nautobot_golden_config-2.0.3/README.md
--rw-r--r--   0        0        0     3415 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/__init__.py
--rw-r--r--   0        0        0       54 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/api/__init__.py
--rw-r--r--   0        0        0     4023 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/api/serializers.py
--rw-r--r--   0        0        0     1071 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/api/urls.py
--rw-r--r--   0        0        0     6468 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/api/views.py
--rw-r--r--   0        0        0        5 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/app-config-schema.json
--rw-r--r--   0        0        0      950 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/choices.py
--rw-r--r--   0        0        0     9452 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/datasources.py
--rw-r--r--   0        0        0      402 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/exceptions.py
--rw-r--r--   0        0        0    14555 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/filters.py
--rw-r--r--   0        0        0    22228 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/forms.py
--rw-r--r--   0        0        0    22856 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/jobs.py
--rw-r--r--   0        0        0     4417 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/metrics.py
--rw-r--r--   0        0        0    12457 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0001_initial.py
--rw-r--r--   0        0        0      500 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0002_custom_data.py
--rw-r--r--   0        0        0     1814 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
--rw-r--r--   0        0        0     1824 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
--rw-r--r--   0        0        0     1538 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0005_json_compliance_rule.py
--rw-r--r--   0        0        0     1794 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
--rw-r--r--   0        0        0     2555 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
--rw-r--r--   0        0        0      665 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
--rw-r--r--   0        0        0     2558 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
--rw-r--r--   0        0        0      929 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
--rw-r--r--   0        0        0     1486 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
--rw-r--r--   0        0        0      909 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
--rw-r--r--   0        0        0      463 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
--rw-r--r--   0        0        0      429 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
--rw-r--r--   0        0        0      697 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
--rw-r--r--   0        0        0      742 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
--rw-r--r--   0        0        0     1594 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
--rw-r--r--   0        0        0      327 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
--rw-r--r--   0        0        0      678 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
--rw-r--r--   0        0        0     1113 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
--rw-r--r--   0        0        0      663 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
--rw-r--r--   0        0        0      389 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
--rw-r--r--   0        0        0      433 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0023_alter_custom_compliance.py
--rw-r--r--   0        0        0      936 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py
--rw-r--r--   0        0        0     2427 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0025_remediation_settings.py
--rw-r--r--   0        0        0     2925 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0026_configplan.py
--rw-r--r--   0        0        0     1243 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0027_auto_20230915_1657.py
--rw-r--r--   0        0        0     1332 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py
--rw-r--r--   0        0        0     7687 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py
--rw-r--r--   0        0        0      469 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0029_alter_configplan_unique_together.py
--rw-r--r--   0        0        0      581 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py
--rw-r--r--   0        0        0        0 2024-03-14 22:43:21.943631 nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/__init__.py
--rw-r--r--   0        0        0    28162 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/models.py
--rw-r--r--   0        0        0     4837 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/navigation.py
--rw-r--r--   0        0        0       51 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/__init__.py
--rw-r--r--   0        0        0     5628 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_backup.py
--rw-r--r--   0        0        0     8259 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_compliance.py
--rw-r--r--   0        0        0     5468 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_deployment.py
--rw-r--r--   0        0        0     5538 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_intended.py
--rw-r--r--   0        0        0     2964 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/processor.py
--rwxr-xr-x   0        0        0     3430 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/signals.py
--rw-r--r--   0        0        0     5157 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css
--rw-r--r--   0        0        0    67022 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js
--rw-r--r--   0        0        0    51068 2024-03-14 22:43:56.480188 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/404.html
--rw-r--r--   0        0        0    53070 2024-03-14 22:43:56.508188 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html
--rw-r--r--   0        0        0    72938 2024-03-14 22:43:56.520189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html
--rw-r--r--   0        0        0    75234 2024-03-14 22:43:56.528189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html
--rw-r--r--   0        0        0    51442 2024-03-14 22:43:56.540189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html
--rw-r--r--   0        0        0    53317 2024-03-14 22:43:56.544189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html
--rw-r--r--   0        0        0    67535 2024-03-14 22:43:56.548189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html
--rw-r--r--   0        0        0    61279 2024-03-14 22:43:56.556189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html
--rw-r--r--   0        0        0    58323 2024-03-14 22:43:56.560189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html
--rw-r--r--   0        0        0    66552 2024-03-14 22:43:56.564189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html
--rw-r--r--   0        0        0    55655 2024-03-14 22:43:56.568189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html
--rw-r--r--   0        0        0    60872 2024-03-14 22:43:56.576189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html
--rw-r--r--   0        0        0    55522 2024-03-14 22:43:56.580190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html
--rw-r--r--   0        0        0    60059 2024-03-14 22:43:56.584190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html
--rw-r--r--   0        0        0    67061 2024-03-14 22:43:56.592190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html
--rw-r--r--   0        0        0    53504 2024-03-14 22:43:56.600190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.600190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.604190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.608190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.612190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.616190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.620190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.624190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.628190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.632190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.636191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.640190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.644191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.644191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.648191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.652191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.656191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.660191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.664191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.668191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.672191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.676191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.680191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.684191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html
--rw-r--r--   0        0        0    53466 2024-03-14 22:43:56.688191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html
--rw-r--r--   0        0        0    53512 2024-03-14 22:43:56.688191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html
--rw-r--r--   0        0        0    52256 2024-03-14 22:43:56.596190 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html
--rw-r--r--   0        0        0    54288 2024-03-14 22:43:56.532189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html
--rw-r--r--   0        0        0    53811 2024-03-14 22:43:56.536189 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html
--rw-r--r--   0        0        0     1000 2024-03-14 22:43:56.332186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     5135 2024-03-14 22:43:56.332186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css
--rw-r--r--   0        0        0    15086 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico
--rw-r--r--   0        0        0     1870 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    97321 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js
--rw-r--r--   0        0        0   891518 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map
--rw-r--r--   0        0        0    17074 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     6882 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js
--rw-r--r--   0        0        0     3383 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2024-03-14 22:43:56.348186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    39431 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js
--rw-r--r--   0        0        0   214982 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map
--rw-r--r--   0        0        0     9204 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png
--rw-r--r--   0        0        0    13318 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg
--rw-r--r--   0        0        0     7562 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png
--rw-r--r--   0        0        0      846 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html
--rw-r--r--   0        0        0   122377 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css
--rw-r--r--   0        0        0    42299 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map
--rw-r--r--   0        0        0    12245 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css
--rw-r--r--   0        0        0     3639 2024-03-14 22:43:56.352186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map
--rw-r--r--   0        0        0    75597 2024-03-14 22:43:56.700191 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html
--rw-r--r--   0        0        0   193115 2024-03-14 22:43:56.804193 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html
--rw-r--r--   0        0        0    51809 2024-03-14 22:43:56.732192 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html
--rw-r--r--   0        0        0   312303 2024-03-14 22:43:56.944195 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html
--rw-r--r--   0        0        0    77149 2024-03-14 22:43:56.964196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html
--rw-r--r--   0        0        0    60245 2024-03-14 22:43:56.704192 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html
--rw-r--r--   0        0        0   114762 2024-03-14 22:43:56.724192 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html
--rw-r--r--   0        0        0    51997 2024-03-14 22:43:56.728192 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html
--rw-r--r--   0        0        0    75903 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png
--rw-r--r--   0        0        0   165191 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png
--rw-r--r--   0        0        0   276244 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png
--rw-r--r--   0        0        0    82969 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png
--rw-r--r--   0        0        0    67457 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png
--rw-r--r--   0        0        0    59437 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png
--rw-r--r--   0        0        0   157371 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png
--rw-r--r--   0        0        0   108592 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png
--rw-r--r--   0        0        0   116460 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png
--rw-r--r--   0        0        0   155101 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png
--rw-r--r--   0        0        0    59126 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png
--rw-r--r--   0        0        0    69205 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png
--rw-r--r--   0        0        0   204762 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png
--rw-r--r--   0        0        0    44937 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png
--rw-r--r--   0        0        0    89739 2024-03-14 22:43:56.336186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png
--rw-r--r--   0        0        0   175928 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png
--rw-r--r--   0        0        0   128918 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png
--rw-r--r--   0        0        0    34712 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png
--rw-r--r--   0        0        0   155103 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png
--rw-r--r--   0        0        0    67662 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png
--rw-r--r--   0        0        0    34084 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png
--rw-r--r--   0        0        0    64803 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png
--rw-r--r--   0        0        0    50317 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png
--rw-r--r--   0        0        0    78058 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png
--rw-r--r--   0        0        0    35263 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png
--rw-r--r--   0        0        0     5689 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png
--rw-r--r--   0        0        0   174561 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png
--rw-r--r--   0        0        0   259361 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png
--rw-r--r--   0        0        0   496898 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png
--rw-r--r--   0        0        0    56418 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png
--rw-r--r--   0        0        0   256279 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png
--rw-r--r--   0        0        0    50350 2024-03-14 22:43:56.340186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png
--rw-r--r--   0        0        0   119945 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png
--rw-r--r--   0        0        0    81496 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png
--rw-r--r--   0        0        0   114519 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png
--rw-r--r--   0        0        0   383810 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png
--rw-r--r--   0        0        0   340453 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png
--rw-r--r--   0        0        0   448190 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png
--rw-r--r--   0        0        0    83466 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png
--rw-r--r--   0        0        0   122430 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png
--rw-r--r--   0        0        0   244962 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png
--rw-r--r--   0        0        0   105992 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png
--rw-r--r--   0        0        0   156622 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png
--rw-r--r--   0        0        0   172988 2024-03-14 22:43:56.344186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png
--rw-r--r--   0        0        0    62138 2024-03-14 22:43:56.504188 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/index.html
--rw-r--r--   0        0        0      858 2024-03-14 22:43:56.332186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv
--rw-r--r--   0        0        0      119 2024-03-14 22:43:56.332186 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/requirements.txt
--rw-r--r--   0        0        0   311197 2024-03-14 22:43:57.084198 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json
--rw-r--r--   0        0        0    14890 2024-03-14 22:43:56.484188 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml
--rw-r--r--   0        0        0      689 2024-03-14 22:43:56.484188 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    63597 2024-03-14 22:43:56.968196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html
--rw-r--r--   0        0        0    64154 2024-03-14 22:43:56.976196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html
--rw-r--r--   0        0        0    58507 2024-03-14 22:43:56.980196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html
--rw-r--r--   0        0        0    75487 2024-03-14 22:43:56.988196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html
--rw-r--r--   0        0        0    55453 2024-03-14 22:43:56.992196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html
--rw-r--r--   0        0        0    59499 2024-03-14 22:43:57.000196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html
--rw-r--r--   0        0        0    65717 2024-03-14 22:43:57.004196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html
--rw-r--r--   0        0        0    69780 2024-03-14 22:43:57.012196 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html
--rw-r--r--   0        0        0    60732 2024-03-14 22:43:57.016197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html
--rw-r--r--   0        0        0    68945 2024-03-14 22:43:57.024197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html
--rw-r--r--   0        0        0    87551 2024-03-14 22:43:57.040197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html
--rw-r--r--   0        0        0    57419 2024-03-14 22:43:57.044197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html
--rw-r--r--   0        0        0    79335 2024-03-14 22:43:57.056197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html
--rw-r--r--   0        0        0    54161 2024-03-14 22:43:57.060197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html
--rw-r--r--   0        0        0    79432 2024-03-14 22:43:57.068197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html
--rw-r--r--   0        0        0    61399 2024-03-14 22:43:57.076197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html
--rw-r--r--   0        0        0    56432 2024-03-14 22:43:57.080197 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html
--rw-r--r--   0        0        0    60266 2024-03-14 22:43:57.084198 nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html
--rw-r--r--   0        0        0     9375 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/static/run_job.js
--rw-r--r--   0        0        0     3426 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/static/toggle_fields.js
--rw-r--r--   0        0        0    19310 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tables.py
--rw-r--r--   0        0        0     5390 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/template_content.py
--rw-r--r--   0        0        0     1123 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
--rw-r--r--   0        0        0     1429 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
--rw-r--r--   0        0        0     8122 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html
--rw-r--r--   0        0        0      607 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html
--rw-r--r--   0        0        0     3931 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html
--rw-r--r--   0        0        0     3607 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html
--rw-r--r--   0        0        0     4268 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html
--rw-r--r--   0        0        0     1861 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html
--rw-r--r--   0        0        0     3251 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html
--rw-r--r--   0        0        0      442 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_update.html
--rw-r--r--   0        0        0      964 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
--rw-r--r--   0        0        0      965 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
--rw-r--r--   0        0        0     4560 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
--rw-r--r--   0        0        0      150 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_details.html
--rw-r--r--   0        0        0     2597 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html
--rw-r--r--   0        0        0     3081 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
--rw-r--r--   0        0        0     2382 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html
--rw-r--r--   0        0        0     3681 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
--rw-r--r--   0        0        0     1393 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
--rw-r--r--   0        0        0      254 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/include/span_button.html
--rw-r--r--   0        0        0     1553 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html
--rw-r--r--   0        0        0      773 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html
--rw-r--r--   0        0        0       35 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templatetags/__init__.py
--rw-r--r--   0        0        0      451 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/templatetags/json_helpers.py
--rw-r--r--   0        0        0       49 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/__init__.py
--rw-r--r--   0        0        0    20312 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/conftest.py
--rw-r--r--   0        0        0       51 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/forms/__init__.py
--rw-r--r--   0        0        0     3216 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/forms/test_golden_config_settings.py
--rw-r--r--   0        0        0       83 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/jinja_filters.py
--rw-r--r--   0        0        0    16589 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_api.py
--rw-r--r--   0        0        0     1041 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_basic.py
--rw-r--r--   0        0        0     3624 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_datasources.py
--rw-r--r--   0        0        0    24891 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_filters.py
--rw-r--r--   0        0        0    12988 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_graphql.py
--rw-r--r--   0        0        0     5519 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_helpers.py
--rwxr-xr-x   0        0        0    33953 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_jobs.py
--rw-r--r--   0        0        0    18996 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_models.py
--rw-r--r--   0        0        0       58 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_nornir_plays/__init__.py
--rw-r--r--   0        0        0     2582 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
--rw-r--r--   0        0        0       55 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/__init__.py
--rw-r--r--   0        0        0     2588 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_config_plan.py
--rw-r--r--   0        0        0     3392 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_git.py
--rw-r--r--   0        0        0     1211 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_graphql.py
--rw-r--r--   0        0        0    15315 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_helpers.py
--rw-r--r--   0        0        0    15351 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_views.py
--rw-r--r--   0        0        0     1134 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/urls.py
--rw-r--r--   0        0        0       17 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/__init__.py
--rw-r--r--   0        0        0     1770 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/config_plan.py
--rw-r--r--   0        0        0     8845 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/config_postprocessing.py
--rw-r--r--   0        0        0     1106 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/constant.py
--rw-r--r--   0        0        0      607 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/db_management.py
--rw-r--r--   0        0        0     1271 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/git.py
--rw-r--r--   0        0        0     1773 2024-03-14 22:43:21.947631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/graphql.py
--rw-r--r--   0        0        0     9375 2024-03-14 22:43:21.951631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/helper.py
--rw-r--r--   0        0        0     1811 2024-03-14 22:43:21.951631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/logger.py
--rw-r--r--   0        0        0     4981 2024-03-14 22:43:21.951631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/mat_plot.py
--rw-r--r--   0        0        0     2081 2024-03-14 22:43:21.951631 nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/utils.py
--rw-r--r--   0        0        0    25070 2024-03-14 22:43:21.951631 nautobot_golden_config-2.0.3/nautobot_golden_config/views.py
--rw-r--r--   0        0        0     6159 2024-03-14 22:43:31.675788 nautobot_golden_config-2.0.3/pyproject.toml
--rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 nautobot_golden_config-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-04-03 00:39:45.454810 nautobot_golden_config-2.0.4/LICENSE
+-rw-r--r--   0        0        0     7047 2024-04-03 00:39:45.454810 nautobot_golden_config-2.0.4/README.md
+-rw-r--r--   0        0        0     3415 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/__init__.py
+-rw-r--r--   0        0        0     4023 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/serializers.py
+-rw-r--r--   0        0        0     1071 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/urls.py
+-rw-r--r--   0        0        0     6468 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/views.py
+-rw-r--r--   0        0        0        5 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/app-config-schema.json
+-rw-r--r--   0        0        0      950 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/choices.py
+-rw-r--r--   0        0        0     9452 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/datasources.py
+-rw-r--r--   0        0        0      745 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/exceptions.py
+-rw-r--r--   0        0        0    14555 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/filters.py
+-rw-r--r--   0        0        0    22228 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/forms.py
+-rw-r--r--   0        0        0    25131 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/jobs.py
+-rw-r--r--   0        0        0     4417 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/metrics.py
+-rw-r--r--   0        0        0    12457 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0001_initial.py
+-rw-r--r--   0        0        0      500 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0002_custom_data.py
+-rw-r--r--   0        0        0     1814 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
+-rw-r--r--   0        0        0     1824 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
+-rw-r--r--   0        0        0     1538 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0005_json_compliance_rule.py
+-rw-r--r--   0        0        0     1794 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
+-rw-r--r--   0        0        0     2555 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
+-rw-r--r--   0        0        0      665 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
+-rw-r--r--   0        0        0     2558 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
+-rw-r--r--   0        0        0      929 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
+-rw-r--r--   0        0        0     1486 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
+-rw-r--r--   0        0        0      909 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
+-rw-r--r--   0        0        0      463 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
+-rw-r--r--   0        0        0      429 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
+-rw-r--r--   0        0        0      697 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
+-rw-r--r--   0        0        0      742 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
+-rw-r--r--   0        0        0     1594 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
+-rw-r--r--   0        0        0      327 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
+-rw-r--r--   0        0        0      678 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
+-rw-r--r--   0        0        0     1113 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
+-rw-r--r--   0        0        0      663 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
+-rw-r--r--   0        0        0      389 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
+-rw-r--r--   0        0        0      433 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0023_alter_custom_compliance.py
+-rw-r--r--   0        0        0      936 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py
+-rw-r--r--   0        0        0     2427 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0025_remediation_settings.py
+-rw-r--r--   0        0        0     2925 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0026_configplan.py
+-rw-r--r--   0        0        0     1243 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0027_auto_20230915_1657.py
+-rw-r--r--   0        0        0     1332 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py
+-rw-r--r--   0        0        0     7687 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py
+-rw-r--r--   0        0        0      469 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0029_alter_configplan_unique_together.py
+-rw-r--r--   0        0        0      581 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py
+-rw-r--r--   0        0        0        0 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/__init__.py
+-rw-r--r--   0        0        0    28162 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/models.py
+-rw-r--r--   0        0        0     4837 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/navigation.py
+-rw-r--r--   0        0        0       51 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/__init__.py
+-rw-r--r--   0        0        0     6574 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_backup.py
+-rw-r--r--   0        0        0     9174 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_compliance.py
+-rw-r--r--   0        0        0     5626 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_deployment.py
+-rw-r--r--   0        0        0     6132 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_intended.py
+-rw-r--r--   0        0        0     2373 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/processor.py
+-rwxr-xr-x   0        0        0     3430 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/signals.py
+-rw-r--r--   0        0        0     5157 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css
+-rw-r--r--   0        0        0    67022 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js
+-rw-r--r--   0        0        0    51068 2024-04-03 00:40:54.330903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/404.html
+-rw-r--r--   0        0        0    53070 2024-04-03 00:40:54.358903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    72938 2024-04-03 00:40:54.370903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html
+-rw-r--r--   0        0        0    75234 2024-04-03 00:40:54.382903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html
+-rw-r--r--   0        0        0    51442 2024-04-03 00:40:54.394903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    53317 2024-04-03 00:40:54.398903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html
+-rw-r--r--   0        0        0    67535 2024-04-03 00:40:54.406903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html
+-rw-r--r--   0        0        0    61279 2024-04-03 00:40:54.410903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    58323 2024-04-03 00:40:54.414903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html
+-rw-r--r--   0        0        0    66552 2024-04-03 00:40:54.422903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html
+-rw-r--r--   0        0        0    55655 2024-04-03 00:40:54.426903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html
+-rw-r--r--   0        0        0    60872 2024-04-03 00:40:54.430903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html
+-rw-r--r--   0        0        0    55522 2024-04-03 00:40:54.434903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html
+-rw-r--r--   0        0        0    60059 2024-04-03 00:40:54.438903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html
+-rw-r--r--   0        0        0    68745 2024-04-03 00:40:54.446903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    53504 2024-04-03 00:40:54.454903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.458903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.462903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.466903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.470903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.474903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.478903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.478903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.482903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.486903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.490903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.494903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.498903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.502903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.506903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.510903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.514903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.518903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.522903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.526903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.530903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.534903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.538903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.542903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html
+-rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.546903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html
+-rw-r--r--   0        0        0    53512 2024-04-03 00:40:54.550903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html
+-rw-r--r--   0        0        0    50870 2024-04-03 00:40:54.554903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3027.html
+-rw-r--r--   0        0        0    50878 2024-04-03 00:40:54.554903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3028.html
+-rw-r--r--   0        0        0    50875 2024-04-03 00:40:54.558903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3029.html
+-rw-r--r--   0        0        0    50870 2024-04-03 00:40:54.562903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3030.html
+-rw-r--r--   0        0        0    52256 2024-04-03 00:40:54.450903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html
+-rw-r--r--   0        0        0    54288 2024-04-03 00:40:54.386903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    53811 2024-04-03 00:40:54.390903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    97321 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js
+-rw-r--r--   0        0        0   891518 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map
+-rw-r--r--   0        0        0    17074 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     6882 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js
+-rw-r--r--   0        0        0     3383 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    39431 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js
+-rw-r--r--   0        0        0   214982 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map
+-rw-r--r--   0        0        0     9204 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   122377 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css
+-rw-r--r--   0        0        0    42299 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map
+-rw-r--r--   0        0        0    12245 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css
+-rw-r--r--   0        0        0     3639 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map
+-rw-r--r--   0        0        0    75597 2024-04-03 00:40:54.574903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html
+-rw-r--r--   0        0        0   193115 2024-04-03 00:40:54.678903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    51809 2024-04-03 00:40:54.606903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0   312303 2024-04-03 00:40:54.818903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html
+-rw-r--r--   0        0        0    77149 2024-04-03 00:40:54.834903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    59370 2024-04-03 00:40:54.578903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html
+-rw-r--r--   0        0        0   114762 2024-04-03 00:40:54.598903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    51997 2024-04-03 00:40:54.602903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html
+-rw-r--r--   0        0        0    75903 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png
+-rw-r--r--   0        0        0   165191 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png
+-rw-r--r--   0        0        0   276244 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png
+-rw-r--r--   0        0        0    82969 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png
+-rw-r--r--   0        0        0    67457 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png
+-rw-r--r--   0        0        0    59437 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png
+-rw-r--r--   0        0        0   157371 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png
+-rw-r--r--   0        0        0   108592 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png
+-rw-r--r--   0        0        0   116460 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png
+-rw-r--r--   0        0        0   155101 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png
+-rw-r--r--   0        0        0    59126 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png
+-rw-r--r--   0        0        0    69205 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png
+-rw-r--r--   0        0        0   204762 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png
+-rw-r--r--   0        0        0    44937 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png
+-rw-r--r--   0        0        0    89739 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png
+-rw-r--r--   0        0        0   175928 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png
+-rw-r--r--   0        0        0   128918 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png
+-rw-r--r--   0        0        0    34712 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png
+-rw-r--r--   0        0        0   155103 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png
+-rw-r--r--   0        0        0    67662 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png
+-rw-r--r--   0        0        0    34084 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png
+-rw-r--r--   0        0        0    64803 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png
+-rw-r--r--   0        0        0    50317 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png
+-rw-r--r--   0        0        0    78058 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png
+-rw-r--r--   0        0        0    35263 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png
+-rw-r--r--   0        0        0     5689 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png
+-rw-r--r--   0        0        0   174561 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png
+-rw-r--r--   0        0        0   259361 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png
+-rw-r--r--   0        0        0   496898 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png
+-rw-r--r--   0        0        0    56418 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png
+-rw-r--r--   0        0        0   256279 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png
+-rw-r--r--   0        0        0    50350 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png
+-rw-r--r--   0        0        0   119945 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png
+-rw-r--r--   0        0        0    81496 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png
+-rw-r--r--   0        0        0   114519 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png
+-rw-r--r--   0        0        0   383810 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png
+-rw-r--r--   0        0        0   340453 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png
+-rw-r--r--   0        0        0   448190 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png
+-rw-r--r--   0        0        0    83466 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png
+-rw-r--r--   0        0        0   122430 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png
+-rw-r--r--   0        0        0   244962 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png
+-rw-r--r--   0        0        0   105992 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png
+-rw-r--r--   0        0        0   156622 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png
+-rw-r--r--   0        0        0   172988 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png
+-rw-r--r--   0        0        0    62138 2024-04-03 00:40:54.354903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/index.html
+-rw-r--r--   0        0        0      858 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv
+-rw-r--r--   0        0        0      119 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/requirements.txt
+-rw-r--r--   0        0        0   314253 2024-04-03 00:40:54.962904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json
+-rw-r--r--   0        0        0    15738 2024-04-03 00:40:54.334903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml
+-rw-r--r--   0        0        0      701 2024-04-03 00:40:54.334903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    63597 2024-04-03 00:40:54.842903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html
+-rw-r--r--   0        0        0    64154 2024-04-03 00:40:54.846903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html
+-rw-r--r--   0        0        0    58507 2024-04-03 00:40:54.850903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html
+-rw-r--r--   0        0        0    75487 2024-04-03 00:40:54.862903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html
+-rw-r--r--   0        0        0    55453 2024-04-03 00:40:54.866903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html
+-rw-r--r--   0        0        0    59499 2024-04-03 00:40:54.874903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html
+-rw-r--r--   0        0        0    65717 2024-04-03 00:40:54.878903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html
+-rw-r--r--   0        0        0    69780 2024-04-03 00:40:54.886903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html
+-rw-r--r--   0        0        0    60732 2024-04-03 00:40:54.890903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html
+-rw-r--r--   0        0        0    68945 2024-04-03 00:40:54.898903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html
+-rw-r--r--   0        0        0    87551 2024-04-03 00:40:54.914903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    57419 2024-04-03 00:40:54.922903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html
+-rw-r--r--   0        0        0    79335 2024-04-03 00:40:54.930904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    54161 2024-04-03 00:40:54.934903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html
+-rw-r--r--   0        0        0    79432 2024-04-03 00:40:54.942903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html
+-rw-r--r--   0        0        0    61399 2024-04-03 00:40:54.950904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html
+-rw-r--r--   0        0        0    56432 2024-04-03 00:40:54.954903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html
+-rw-r--r--   0        0        0    60266 2024-04-03 00:40:54.962904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html
+-rw-r--r--   0        0        0     9375 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/run_job.js
+-rw-r--r--   0        0        0     3426 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/toggle_fields.js
+-rw-r--r--   0        0        0    19310 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/tables.py
+-rw-r--r--   0        0        0     5390 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/template_content.py
+-rw-r--r--   0        0        0     1123 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
+-rw-r--r--   0        0        0     1429 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
+-rw-r--r--   0        0        0     8122 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html
+-rw-r--r--   0        0        0      607 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html
+-rw-r--r--   0        0        0     3931 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html
+-rw-r--r--   0        0        0     3607 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html
+-rw-r--r--   0        0        0     4268 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html
+-rw-r--r--   0        0        0     1861 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html
+-rw-r--r--   0        0        0     3251 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html
+-rw-r--r--   0        0        0      442 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_update.html
+-rw-r--r--   0        0        0      964 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
+-rw-r--r--   0        0        0      965 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
+-rw-r--r--   0        0        0     4560 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
+-rw-r--r--   0        0        0      150 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_details.html
+-rw-r--r--   0        0        0     2597 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html
+-rw-r--r--   0        0        0     3081 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
+-rw-r--r--   0        0        0     2382 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html
+-rw-r--r--   0        0        0     3681 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
+-rw-r--r--   0        0        0     1393 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
+-rw-r--r--   0        0        0      254 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/include/span_button.html
+-rw-r--r--   0        0        0     1553 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html
+-rw-r--r--   0        0        0      773 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html
+-rw-r--r--   0        0        0       35 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templatetags/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templatetags/json_helpers.py
+-rw-r--r--   0        0        0       49 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/__init__.py
+-rw-r--r--   0        0        0    20312 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/conftest.py
+-rw-r--r--   0        0        0       51 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/__init__.py
+-rw-r--r--   0        0        0     3216 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/test_golden_config_settings.py
+-rw-r--r--   0        0        0       83 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/jinja_filters.py
+-rw-r--r--   0        0        0    16589 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_api.py
+-rw-r--r--   0        0        0     1041 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_basic.py
+-rw-r--r--   0        0        0     3624 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_datasources.py
+-rw-r--r--   0        0        0    24891 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_filters.py
+-rw-r--r--   0        0        0    12988 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_graphql.py
+-rw-r--r--   0        0        0     5519 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_helpers.py
+-rwxr-xr-x   0        0        0    33953 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_jobs.py
+-rw-r--r--   0        0        0    18996 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_models.py
+-rw-r--r--   0        0        0       58 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/__init__.py
+-rw-r--r--   0        0        0     2582 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
+-rw-r--r--   0        0        0       55 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/__init__.py
+-rw-r--r--   0        0        0     2588 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_config_plan.py
+-rw-r--r--   0        0        0     3392 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_git.py
+-rw-r--r--   0        0        0     1211 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_graphql.py
+-rw-r--r--   0        0        0    15315 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_helpers.py
+-rw-r--r--   0        0        0    15351 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_views.py
+-rw-r--r--   0        0        0     1134 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/urls.py
+-rw-r--r--   0        0        0       17 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/__init__.py
+-rw-r--r--   0        0        0     1770 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_plan.py
+-rw-r--r--   0        0        0     8845 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_postprocessing.py
+-rw-r--r--   0        0        0     1106 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/constant.py
+-rw-r--r--   0        0        0      607 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/db_management.py
+-rw-r--r--   0        0        0     1271 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/git.py
+-rw-r--r--   0        0        0     1773 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/graphql.py
+-rw-r--r--   0        0        0     9375 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/helper.py
+-rw-r--r--   0        0        0     1811 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/logger.py
+-rw-r--r--   0        0        0     4981 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/mat_plot.py
+-rw-r--r--   0        0        0     2081 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/utils.py
+-rw-r--r--   0        0        0    25070 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/views.py
+-rw-r--r--   0        0        0     6159 2024-04-03 00:39:54.750823 nautobot_golden_config-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 nautobot_golden_config-2.0.4/PKG-INFO
```

### Comparing `nautobot_golden_config-2.0.3/LICENSE` & `nautobot_golden_config-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/README.md` & `nautobot_golden_config-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/__init__.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/api/serializers.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/api/urls.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/api/views.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/choices.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/datasources.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/filters.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/forms.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/jobs.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/jobs.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 )
 from nautobot.extras.models import DynamicGroup, Role, Status, Tag
 from nautobot.tenancy.models import Tenant, TenantGroup
 from nautobot_plugin_nornir.plugins.inventory.nautobot_orm import NautobotORMInventory
 from nornir.core.plugins.inventory import InventoryPluginRegister
 from nornir_nautobot.exceptions import NornirNautobotException
 from nautobot_golden_config.choices import ConfigPlanTypeChoice
+from nautobot_golden_config.exceptions import BackupFailure, ComplianceFailure, IntendedGenerationFailure
 from nautobot_golden_config.models import ComplianceFeature, ConfigPlan, GoldenConfig
 from nautobot_golden_config.nornir_plays.config_backup import config_backup
 from nautobot_golden_config.nornir_plays.config_compliance import config_compliance
 from nautobot_golden_config.nornir_plays.config_deployment import config_deployment
 from nautobot_golden_config.nornir_plays.config_intended import config_intended
 from nautobot_golden_config.utilities import constant
 from nautobot_golden_config.utilities.config_plan import (
@@ -95,55 +96,77 @@
             and "nautobot_golden_config.backupconfigs" in git_repo.nautobot_repo_obj.provided_contents
         ):
             commit = True
         repositories[str(git_repo.nautobot_repo_obj.id)] = {"repo_obj": git_repo, "to_commit": commit}
     return repositories
 
 
+def gc_repo_prep(job, data):
+    """Prepare Golden Config git repos for work.
+
+    Args:
+        job (Job): Nautobot Job object with logger and other vars.
+        data (dict): Data being passed from Job.
+
+    Returns:
+        List[GitRepo]: List of GitRepos to be used with Job(s).
+    """
+    job.logger.debug("Compiling device data for GC job.", extra={"grouping": "Get Job Filter"})
+    job.qs = get_job_filter(data)
+    job.logger.debug(f"In scope device count for this job: {job.qs.count()}", extra={"grouping": "Get Job Filter"})
+    job.logger.debug("Mapping device(s) to GC Settings.", extra={"grouping": "Device to Settings Map"})
+    job.device_to_settings_map = get_device_to_settings_map(queryset=job.qs)
+    gitrepo_types = list(set(get_repo_types_for_job(job.name)))
+    job.logger.debug(
+        f"Repository types to sync: {', '.join(sorted(gitrepo_types))}",
+        extra={"grouping": "GC Repo Syncs"},
+    )
+    current_repos = get_refreshed_repos(job_obj=job, repo_types=gitrepo_types, data=job.qs)
+    return current_repos
+
+
+def gc_repo_push(job, current_repos):
+    """Push any work from worker to git repos in Job.
+
+    Args:
+        job (Job): Nautobot Job with logger and other attributes.
+        current_repos (List[GitRepo]): List of GitRepos to be used with Job(s).
+    """
+    now = make_aware(datetime.now())
+    job.logger.debug(
+        f"Finished the {job.Meta.name} job execution.",
+        extra={"grouping": "GC After Run"},
+    )
+    if current_repos:
+        for _, repo in current_repos.items():
+            if repo["to_commit"]:
+                job.logger.debug(
+                    f"Pushing {job.Meta.name} results to repo {repo['repo_obj'].base_url}.",
+                    extra={"grouping": "GC Repo Commit and Push"},
+                )
+                repo["repo_obj"].commit_with_added(f"{job.Meta.name.upper()} JOB {now}")
+                repo["repo_obj"].push()
+
+
 def gc_repos(func):
     """Decorator used for handle repo syncing, commiting, and pushing."""
 
     def gc_repo_wrapper(self, *args, **kwargs):
         """Decorator used for handle repo syncing, commiting, and pushing."""
-        self.logger.debug("Compiling device data for GC job.", extra={"grouping": "Get Job Filter"})
-        self.qs = get_job_filter(kwargs)
-        self.logger.debug(
-            f"In scope device count for this job: {self.qs.count()}", extra={"grouping": "Get Job Filter"}
-        )
-        self.logger.debug("Mapping device(s) to GC Settings.", extra={"grouping": "Device to Settings Map"})
-        self.device_to_settings_map = get_device_to_settings_map(queryset=self.qs)
-        gitrepo_types = list(set(get_repo_types_for_job(self.name)))
-        self.logger.debug(
-            f"Repository types to sync: {', '.join(sorted(gitrepo_types))}",
-            extra={"grouping": "GC Repo Syncs"},
-        )
-        current_repos = get_refreshed_repos(job_obj=self, repo_types=gitrepo_types, data=self.qs)
+        current_repos = gc_repo_prep(job=self, data=kwargs)
         # This is where the specific jobs run method runs via this decorator.
         try:
             func(self, *args, **kwargs)
         except Exception as error:  # pylint: disable=broad-exception-caught
             error_msg = f"`E3001:` General Exception handler, original error message ```{error}```"
             # Raise error only if the job kwarg (checkbox) is selected to do so on the job execution form.
-            if kwargs["fail_job_on_task_failure"]:
+            if kwargs.get("fail_job_on_task_failure"):
                 raise NornirNautobotException(error_msg) from error
         finally:
-            now = make_aware(datetime.now())
-            self.logger.debug(
-                f"Finished the {self.Meta.name} job execution.",
-                extra={"grouping": "GC After Run"},
-            )
-            if current_repos:
-                for _, repo in current_repos.items():
-                    if repo["to_commit"]:
-                        self.logger.debug(
-                            f"Pushing {self.Meta.name} results to repo {repo['repo_obj'].base_url}.",
-                            extra={"grouping": "GC Repo Commit and Push"},
-                        )
-                        repo["repo_obj"].commit_with_added(f"{self.Meta.name.upper()} JOB {now}")
-                        repo["repo_obj"].push()
+            gc_repo_push(job=self, current_repos=current_repos)
 
     return gc_repo_wrapper
 
 
 class FormEntry:  # pylint disable=too-few-public-method
     """Class definition to use as Mixin for form definitions."""
 
@@ -164,22 +187,21 @@
         model=Status,
         required=False,
         query_params={"content_types": Device._meta.label_lower},
         display_field="label",
         label="Device Status",
     )
     debug = BooleanVar(description="Enable for more verbose debug logging")
-    fail_job_on_task_failure = BooleanVar(
-        description="If any device in the tasks list fails, fail the entire job result."
-    )
 
 
 class GoldenConfigJobMixin(Job):  # pylint: disable=abstract-method
     """Reused mixin to be able to set defaults for instance attributes in all GC jobs."""
 
+    fail_job_on_task_failure = BooleanVar(description="If any tasks for any device fails, fail the entire job result.")
+
     def __init__(self, *args, **kwargs):
         """Initialize the job."""
         super().__init__(*args, **kwargs)
         self.qs = None
         self.device_to_settings_map = {}
 
 
@@ -196,20 +218,15 @@
     @gc_repos
     def run(self, *args, **data):  # pylint: disable=unused-argument
         """Run config compliance report script."""
         self.logger.warning("Starting config compliance nornir play.")
         if not constant.ENABLE_COMPLIANCE:
             self.logger.critical("Compliance is disabled in application settings.")
             raise ValueError("Compliance is disabled in application settings.")
-        config_compliance(
-            self.job_result,
-            self.logger.getEffectiveLevel(),
-            self.qs,  # pylint: disable=no-member
-            self.device_to_settings_map,  # pylint: disable=no-member
-        )
+        config_compliance(self)
 
 
 class IntendedJob(GoldenConfigJobMixin, FormEntry):
     """Job to to run generation of intended configurations."""
 
     class Meta:
         """Meta object boilerplate for intended."""
@@ -221,21 +238,15 @@
     @gc_repos
     def run(self, *args, **data):  # pylint: disable=unused-argument
         """Run config generation script."""
         self.logger.debug("Building device settings mapping and running intended config nornir play.")
         if not constant.ENABLE_INTENDED:
             self.logger.critical("Intended Generation is disabled in application settings.")
             raise ValueError("Intended Generation is disabled in application settings.")
-        config_intended(
-            self.job_result,
-            self.logger.getEffectiveLevel(),
-            self,
-            self.qs,  # pylint: disable=no-member
-            self.device_to_settings_map,  # pylint: disable=no-member
-        )
+        config_intended(self)
 
 
 class BackupJob(GoldenConfigJobMixin, FormEntry):
     """Job to to run the backup job."""
 
     class Meta:
         """Meta object boilerplate for backup configurations."""
@@ -247,20 +258,15 @@
     @gc_repos
     def run(self, *args, **data):  # pylint: disable=unused-argument
         """Run config backup process."""
         self.logger.debug("Starting config backup nornir play.")
         if not constant.ENABLE_BACKUP:
             self.logger.critical("Backups are disabled in application settings.")
             raise ValueError("Backups are disabled in application settings.")
-        config_backup(
-            self.job_result,
-            self.logger.getEffectiveLevel(),
-            self.qs,
-            self.device_to_settings_map,
-        )
+        config_backup(self)
 
 
 class AllGoldenConfig(GoldenConfigJobMixin):
     """Job to to run all three jobs against a single device."""
 
     device = ObjectVar(model=Device, required=True)
     debug = BooleanVar(description="Enable for more verbose debug logging")
@@ -268,76 +274,100 @@
     class Meta:
         """Meta object boilerplate for all jobs to run against a device."""
 
         name = "Execute All Golden Configuration Jobs - Single Device"
         description = "Process to run all Golden Configuration jobs configured."
         has_sensitive_variables = False
 
-    @gc_repos
-    def run(self, *args, **data):  # pylint: disable=unused-argument
+    def run(self, *args, **data):  # pylint: disable=unused-argument, too-many-branches
         """Run all jobs on a single device."""
-        if constant.ENABLE_INTENDED:
-            config_intended(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self,
-                self.qs,
-                self.device_to_settings_map,
-            )
-        if constant.ENABLE_BACKUP:
-            config_backup(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self.qs,
-                self.device_to_settings_map,
-            )
-        if constant.ENABLE_COMPLIANCE:
-            config_compliance(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self.qs,
-                self.device_to_settings_map,
-            )
+        current_repos = gc_repo_prep(job=self, data=data)
+        failed_jobs = []
+        error_msg, jobs_list = "", "All"
+        for enabled, play in [
+            (constant.ENABLE_INTENDED, config_intended),
+            (constant.ENABLE_BACKUP, config_backup),
+            (constant.ENABLE_COMPLIANCE, config_compliance),
+        ]:
+            try:
+                if enabled:
+                    play(self)
+            except BackupFailure:
+                self.logger.error("Backup failure occurred!")
+                failed_jobs.append("Backup")
+            except IntendedGenerationFailure:
+                self.logger.error("Intended failure occurred!")
+                failed_jobs.append("Intended")
+            except ComplianceFailure:
+                self.logger.error("Compliance failure occurred!")
+                failed_jobs.append("Compliance")
+            except Exception as error:  # pylint: disable=broad-exception-caught
+                error_msg = f"`E3001:` General Exception handler, original error message ```{error}```"
+        gc_repo_push(job=self, current_repos=current_repos)
+        if len(failed_jobs) > 1:
+            jobs_list = ", ".join(failed_jobs)
+        elif len(failed_jobs) == 1:
+            jobs_list = failed_jobs[0]
+        failure_msg = f"`E3030:` Failure during {jobs_list} Job(s)."
+        if len(failed_jobs) > 0:
+            self.logger.error(failure_msg)
+        if (len(failed_jobs) > 0 or error_msg) and data["fail_job_on_task_failure"]:
+            if not error_msg:
+                error_msg = failure_msg
+            # Raise error only if the job kwarg (checkbox) is selected to do so on the job execution form.
+            raise NornirNautobotException(error_msg)
 
 
 class AllDevicesGoldenConfig(GoldenConfigJobMixin, FormEntry):
     """Job to to run all three jobs against multiple devices."""
 
     class Meta:
         """Meta object boilerplate for all jobs to run against multiple devices."""
 
         name = "Execute All Golden Configuration Jobs - Multiple Device"
         description = "Process to run all Golden Configuration jobs configured against multiple devices."
         has_sensitive_variables = False
 
-    @gc_repos
-    def run(self, *args, **data):  # pylint: disable=unused-argument
+    def run(self, *args, **data):  # pylint: disable=unused-argument, too-many-branches
         """Run all jobs on multiple devices."""
-        if constant.ENABLE_INTENDED:
-            config_intended(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self,
-                self.qs,
-                self.device_to_settings_map,
-            )
-        if constant.ENABLE_BACKUP:
-            config_backup(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self.qs,
-                self.device_to_settings_map,
-            )
-        if constant.ENABLE_COMPLIANCE:
-            config_compliance(
-                self.job_result,
-                self.logger.getEffectiveLevel(),
-                self.qs,
-                self.device_to_settings_map,
-            )
+        current_repos = gc_repo_prep(job=self, data=data)
+        failed_jobs = []
+        error_msg, jobs_list = "", "All"
+        for enabled, play in [
+            (constant.ENABLE_INTENDED, config_intended),
+            (constant.ENABLE_BACKUP, config_backup),
+            (constant.ENABLE_COMPLIANCE, config_compliance),
+        ]:
+            try:
+                if enabled:
+                    play(self)
+            except BackupFailure:
+                self.logger.error("Backup failure occurred!")
+                failed_jobs.append("Backup")
+            except IntendedGenerationFailure:
+                self.logger.error("Intended failure occurred!")
+                failed_jobs.append("Intended")
+            except ComplianceFailure:
+                self.logger.error("Compliance failure occurred!")
+                failed_jobs.append("Compliance")
+            except Exception as error:  # pylint: disable=broad-exception-caught
+                error_msg = f"`E3001:` General Exception handler, original error message ```{error}```"
+        gc_repo_push(job=self, current_repos=current_repos)
+        if len(failed_jobs) > 1:
+            jobs_list = ", ".join(failed_jobs)
+        elif len(failed_jobs) == 1:
+            jobs_list = failed_jobs[0]
+        failure_msg = f"`E3030:` Failure during {jobs_list} Job(s)."
+        if len(failed_jobs) > 0:
+            self.logger.error(failure_msg)
+        if (len(failed_jobs) > 0 or error_msg) and data["fail_job_on_task_failure"]:
+            if not error_msg:
+                error_msg = failure_msg
+            # Raise error only if the job kwarg (checkbox) is selected to do so on the job execution form.
+            raise NornirNautobotException(error_msg)
 
 
 class GenerateConfigPlans(Job, FormEntry):
     """Job to generate config plans."""
 
     # Config Plan generation fields
     plan_type = ChoiceVar(choices=ConfigPlanTypeChoice.CHOICES)
@@ -475,34 +505,45 @@
     class Meta:
         """Meta object boilerplate for config plan deployment."""
 
         name = "Deploy Config Plans"
         description = "Deploy config plans to devices."
         has_sensitive_variables = False
 
+    def __init__(self, *args, **kwargs):
+        """Initialize the job."""
+        super().__init__(*args, **kwargs)
+        self.data = {}
+
     def run(self, **data):  # pylint: disable=arguments-differ
         """Run config plan deployment process."""
         self.logger.debug("Starting config plan deployment job.")
-        config_deployment(self.job_result, self.logger.getEffectiveLevel(), data)
+        self.data = data
+        config_deployment(self)
 
 
 class DeployConfigPlanJobButtonReceiver(JobButtonReceiver):
     """Job button to deploy a config plan."""
 
     class Meta:
         """Meta object boilerplate for config plan deployment job button."""
 
         name = "Deploy Config Plan (Job Button Receiver)"
         has_sensitive_variables = False
 
+    def __init__(self, *args, **kwargs):
+        """Initialize the job."""
+        super().__init__(*args, **kwargs)
+        self.data = {}
+
     def receive_job_button(self, obj):
         """Run config plan deployment process."""
         self.logger.debug("Starting config plan deployment job.")
-        data = {"debug": False, "config_plan": ConfigPlan.objects.filter(id=obj.id)}
-        config_deployment(self.job_result, self.logger.getEffectiveLevel(), data)
+        self.data = {"debug": False, "config_plan": ConfigPlan.objects.filter(id=obj.id)}
+        config_deployment(self)
 
 
 class SyncGoldenConfigWithDynamicGroups(Job):
     """Job to sync (add/remove) GoldenConfig table based on DynamicGroup members."""
 
     class Meta:
         """Meta object boilerplate for syncing GoldenConfig table."""
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/metrics.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0001_initial.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0003_auto_20210510_2356.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0003_auto_20210510_2356.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0004_auto_20210616_2234.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0004_auto_20210616_2234.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0005_json_compliance_rule.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0005_json_compliance_rule.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0008_multi_repo_support_final.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0008_multi_repo_support_final.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0025_remediation_settings.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0025_remediation_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0026_configplan.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0026_configplan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0027_auto_20230915_1657.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0027_auto_20230915_1657.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/models.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/navigation.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_backup.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_backup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Nornir job for backing up actual config."""
+
 # pylint: disable=relative-beyond-top-level
 import logging
 import os
 from datetime import datetime
 
 from django.utils.timezone import make_aware
 from nautobot_plugin_nornir.constants import NORNIR_SETTINGS
 from nautobot_plugin_nornir.plugins.inventory.nautobot_orm import NautobotORMInventory
 from nornir import InitNornir
 from nornir.core.plugins.inventory import InventoryPluginRegister
 from nornir.core.task import Result, Task
+from nornir_nautobot.exceptions import NornirNautobotException
 from nornir_nautobot.plugins.tasks.dispatcher import dispatcher
+from nautobot_golden_config.exceptions import BackupFailure
 from nautobot_golden_config.models import ConfigRemove, ConfigReplace, GoldenConfig
 from nautobot_golden_config.nornir_plays.processor import ProcessGoldenConfig
 from nautobot_golden_config.utilities.db_management import close_threaded_db_connections
 from nautobot_golden_config.utilities.helper import (
     dispatch_params,
     render_jinja_template,
     verify_settings,
@@ -77,20 +80,31 @@
     backup_obj.save()
 
     logger.info("Successfully extracted running configuration from device.", extra={"object": obj})
 
     return Result(host=task.host, result=running_config)
 
 
-def config_backup(job_result, log_level, qs, device_to_settings_map):
-    """Nornir play to backup configurations."""
+def config_backup(job):
+    """
+    Nornir play to backup configurations.
+
+    Args:
+        job (Job): The Nautobot Job instance being run.
+
+    Returns:
+        None: Backup configuration files are written to filesystem.
+
+    Raises:
+        BackupFailure: If failure found in Nornir tasks then Exception will be raised.
+    """
     now = make_aware(datetime.now())
-    logger = NornirLogger(job_result, log_level)
+    logger = NornirLogger(job.job_result, job.logger.getEffectiveLevel())
 
-    for settings in set(device_to_settings_map.values()):
+    for settings in set(job.device_to_settings_map.values()):
         verify_settings(logger, settings, ["backup_path_template"])
 
     # Build a dictionary, with keys of platform.network_driver, and the regex line in it for the netutils func.
     remove_regex_dict = {}
     for regex in ConfigRemove.objects.all():
         if not remove_regex_dict.get(regex.platform.network_driver):
             remove_regex_dict[regex.platform.network_driver] = []
@@ -98,33 +112,43 @@
 
     # Build a dictionary, with keys of platform.network_driver, and the regex and replace keys for the netutils func.
     replace_regex_dict = {}
     for regex in ConfigReplace.objects.all():
         if not replace_regex_dict.get(regex.platform.network_driver):
             replace_regex_dict[regex.platform.network_driver] = []
         replace_regex_dict[regex.platform.network_driver].append({"replace": regex.replace, "regex": regex.regex})
-    with InitNornir(
-        runner=NORNIR_SETTINGS.get("runner"),
-        logging={"enabled": False},
-        inventory={
-            "plugin": "nautobot-inventory",
-            "options": {
-                "credentials_class": NORNIR_SETTINGS.get("credentials"),
-                "params": NORNIR_SETTINGS.get("inventory_params"),
-                "queryset": qs,
-                "defaults": {"now": now},
+    try:
+        with InitNornir(
+            runner=NORNIR_SETTINGS.get("runner"),
+            logging={"enabled": False},
+            inventory={
+                "plugin": "nautobot-inventory",
+                "options": {
+                    "credentials_class": NORNIR_SETTINGS.get("credentials"),
+                    "params": NORNIR_SETTINGS.get("inventory_params"),
+                    "queryset": job.qs,
+                    "defaults": {"now": now},
+                },
             },
-        },
-    ) as nornir_obj:
-        nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
-
-        logger.debug("Run nornir backup tasks.")
-        nr_with_processors.run(
-            task=run_backup,
-            name="BACKUP CONFIG",
-            logger=logger,
-            device_to_settings_map=device_to_settings_map,
-            remove_regex_dict=remove_regex_dict,
-            replace_regex_dict=replace_regex_dict,
+        ) as nornir_obj:
+            nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
+
+            logger.debug("Run nornir backup tasks.")
+            results = nr_with_processors.run(
+                task=run_backup,
+                name="BACKUP CONFIG",
+                logger=logger,
+                device_to_settings_map=job.device_to_settings_map,
+                remove_regex_dict=remove_regex_dict,
+                replace_regex_dict=replace_regex_dict,
+            )
+            logger.debug("Completed configuration from devices.")
+    except NornirNautobotException as err:
+        logger.error(
+            f"`E3027:` NornirNautobotException raised during backup tasks. Original exception message: ```{err}```"
         )
-        logger.debug("Completed configuration from devices.")
+        # re-raise Exception if it's raised from nornir-nautobot or nautobot-app-nornir
+        if str(err).startswith("`E2") or str(err).startswith("`E1"):
+            raise NornirNautobotException(err) from err
     logger.debug("Completed configuration backup job for devices.")
+    if results.failed:
+        raise BackupFailure()
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_compliance.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_compliance.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from nautobot_plugin_nornir.plugins.inventory.nautobot_orm import NautobotORMInventory
 from netutils.config.compliance import _open_file_config, parser_map, section_config
 from nornir import InitNornir
 from nornir.core.plugins.inventory import InventoryPluginRegister
 from nornir.core.task import Result, Task
 from nornir_nautobot.exceptions import NornirNautobotException
 from nautobot_golden_config.choices import ComplianceRuleConfigTypeChoice
+from nautobot_golden_config.exceptions import ComplianceFailure
 from nautobot_golden_config.models import ComplianceRule, ConfigCompliance, GoldenConfig
 from nautobot_golden_config.nornir_plays.processor import ProcessGoldenConfig
 from nautobot_golden_config.utilities.db_management import close_threaded_db_connections
 from nautobot_golden_config.utilities.helper import get_json_config, render_jinja_template, verify_settings
 from nautobot_golden_config.utilities.logger import NornirLogger
 
 InventoryPluginRegister.register("nautobot-inventory", NautobotORMInventory)
@@ -164,40 +165,61 @@
     compliance_obj.compliance_config = "\n".join(diff_files(backup_file, intended_file))
     compliance_obj.save()
     logger.info("Successfully tested compliance job.", extra={"object": obj})
 
     return Result(host=task.host)
 
 
-def config_compliance(job_result, log_level, qs, device_to_settings_map):
-    """Nornir play to generate configurations."""
+def config_compliance(job):  # pylint: disable=unused-argument
+    """
+    Nornir play to generate configurations.
+
+    Args:
+        job (Job): The Nautobot Job instance being run.
+
+    Returns:
+        None: Compliance results are written to database.
+
+    Raises:
+        ComplianceFailure: If failure found in Nornir tasks then Exception will be raised.
+    """
     now = make_aware(datetime.now())
-    logger = NornirLogger(job_result, log_level)
+    logger = NornirLogger(job.job_result, job.logger.getEffectiveLevel())
 
     rules = get_rules()
 
-    for settings in set(device_to_settings_map.values()):
+    for settings in set(job.device_to_settings_map.values()):
         verify_settings(logger, settings, ["backup_path_template", "intended_path_template"])
-    with InitNornir(
-        runner=NORNIR_SETTINGS.get("runner"),
-        logging={"enabled": False},
-        inventory={
-            "plugin": "nautobot-inventory",
-            "options": {
-                "credentials_class": NORNIR_SETTINGS.get("credentials"),
-                "params": NORNIR_SETTINGS.get("inventory_params"),
-                "queryset": qs,
-                "defaults": {"now": now},
+    try:
+        with InitNornir(
+            runner=NORNIR_SETTINGS.get("runner"),
+            logging={"enabled": False},
+            inventory={
+                "plugin": "nautobot-inventory",
+                "options": {
+                    "credentials_class": NORNIR_SETTINGS.get("credentials"),
+                    "params": NORNIR_SETTINGS.get("inventory_params"),
+                    "queryset": job.qs,
+                    "defaults": {"now": now},
+                },
             },
-        },
-    ) as nornir_obj:
-        nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
-
-        logger.debug("Run nornir compliance tasks.")
-        nr_with_processors.run(
-            task=run_compliance,
-            name="RENDER COMPLIANCE TASK GROUP",
-            logger=logger,
-            device_to_settings_map=device_to_settings_map,
-            rules=rules,
+        ) as nornir_obj:
+            nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
+
+            logger.debug("Run nornir compliance tasks.")
+            results = nr_with_processors.run(
+                task=run_compliance,
+                name="RENDER COMPLIANCE TASK GROUP",
+                logger=logger,
+                device_to_settings_map=job.device_to_settings_map,
+                rules=rules,
+            )
+    except NornirNautobotException as err:
+        logger.error(
+            f"`E3028:` NornirNautobotException raised during compliance tasks. Original exception message: ```{err}```"
         )
+        # re-raise Exception if it's raised from nornir-nautobot or nautobot-app-nornir
+        if str(err).startswith("`E2") or str(err).startswith("`E1"):
+            raise NornirNautobotException(err) from err
     logger.debug("Completed compliance job for devices.")
+    if results.failed:
+        raise ComplianceFailure()
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_deployment.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_deployment.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,21 +70,29 @@
         error_msg = f"`E3024:` Failed deployment to the device with error: {error}"
         logger.error(error_msg, extra={"object": obj})
         raise NornirNautobotException(error_msg) from error
 
     return Result(host=task.host, result=task_result)
 
 
-def config_deployment(job_result, log_level, data):
-    """Nornir play to deploy configurations."""
+def config_deployment(job):
+    """
+    Nornir play to deploy configurations.
+
+    Args:
+        job (Job): The Nautobot Job instance being run.
+
+    Returns:
+        None: Deployment results are written to database.
+    """
     now = make_aware(datetime.now())
-    logger = NornirLogger(job_result, log_level)
+    logger = NornirLogger(job.job_result, job.logger.getEffectiveLevel())
 
     logger.debug("Starting config deployment")
-    config_plan_qs = data["config_plan"]
+    config_plan_qs = job.data["config_plan"]
     if config_plan_qs.filter(status__name=DEFAULT_DEPLOY_STATUS).exists():
         error_msg = "`E3025:` Cannot deploy configuration(s). One or more config plans are not approved."
         logger.error(error_msg)
         raise NornirNautobotException(error_msg)
     if config_plan_qs.filter(status__name="Completed").exists():
         error_msg = "`E3026:` Cannot deploy configuration(s). One or more config plans are already completed."
         logger.error(error_msg)
@@ -108,15 +116,15 @@
             nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
 
             nr_with_processors.run(
                 task=run_deployment,
                 name="DEPLOY CONFIG",
                 logger=logger,
                 config_plan_qs=config_plan_qs,
-                deploy_job_result=job_result,
+                deploy_job_result=job.job_result,
             )
     except Exception as error:
         error_msg = f"`E3001:` General Exception handler, original error message ```{error}```"
         logger.error(error_msg)
         raise NornirNautobotException(error_msg) from error
 
     logger.debug("Completed configuration deployment.")
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/config_intended.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_intended.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Nornir job for generating the intended config."""
+
 # pylint: disable=relative-beyond-top-level
 import logging
 import os
 from datetime import datetime
 
 from django.utils.timezone import make_aware
 from nornir import InitNornir
 from nornir.core.plugins.inventory import InventoryPluginRegister
 from nornir.core.task import Result, Task
 from nornir_nautobot.exceptions import NornirNautobotException
 from nornir_nautobot.plugins.tasks.dispatcher import dispatcher
 from nautobot_plugin_nornir.constants import NORNIR_SETTINGS
 from nautobot_plugin_nornir.plugins.inventory.nautobot_orm import NautobotORMInventory
+from nautobot_golden_config.exceptions import IntendedGenerationFailure
 from nautobot_golden_config.models import GoldenConfig
 from nautobot_golden_config.nornir_plays.processor import ProcessGoldenConfig
 from nautobot_golden_config.utilities.db_management import close_threaded_db_connections
 from nautobot_golden_config.utilities.graphql import graph_ql_query
 from nautobot_golden_config.utilities.helper import (
     dispatch_params,
     get_django_env,
@@ -86,52 +88,63 @@
     intended_obj.save()
 
     logger.info("Successfully generated the intended configuration.", extra={"object": obj})
 
     return Result(host=task.host, result=generated_config)
 
 
-def config_intended(job_result, log_level, job_class_instance, qs, device_to_settings_map):
+def config_intended(job):
     """
     Nornir play to generate configurations.
 
     Args:
-        logger (NornirLogger): The Nautobot Job instance being run.
-        job_class_instance (Job): The Nautobot Job instance being run.
-        data (dict): Form data from Nautobot Job.
+        job (Job): The Nautobot Job instance being run.
 
     Returns:
         None: Intended configuration files are written to filesystem.
+
+    Raises:
+        IntendedGenerationFailure: If failure found in Nornir tasks then Exception will be raised.
     """
     now = make_aware(datetime.now())
-    logger = NornirLogger(job_result, log_level)
+    logger = NornirLogger(job.job_result, job.logger.getEffectiveLevel())
 
-    for settings in set(device_to_settings_map.values()):
+    for settings in set(job.device_to_settings_map.values()):
         verify_settings(logger, settings, ["jinja_path_template", "intended_path_template", "sot_agg_query"])
 
     # Retrieve filters from the Django jinja template engine
     jinja_env = get_django_env()
-    with InitNornir(
-        runner=NORNIR_SETTINGS.get("runner"),
-        logging={"enabled": False},
-        inventory={
-            "plugin": "nautobot-inventory",
-            "options": {
-                "credentials_class": NORNIR_SETTINGS.get("credentials"),
-                "params": NORNIR_SETTINGS.get("inventory_params"),
-                "queryset": qs,
-                "defaults": {"now": now},
+    try:
+        with InitNornir(
+            runner=NORNIR_SETTINGS.get("runner"),
+            logging={"enabled": False},
+            inventory={
+                "plugin": "nautobot-inventory",
+                "options": {
+                    "credentials_class": NORNIR_SETTINGS.get("credentials"),
+                    "params": NORNIR_SETTINGS.get("inventory_params"),
+                    "queryset": job.qs,
+                    "defaults": {"now": now},
+                },
             },
-        },
-    ) as nornir_obj:
-        nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
-
-        logger.debug("Run nornir render config tasks.")
-        # Run the Nornir Tasks
-        nr_with_processors.run(
-            task=run_template,
-            name="RENDER CONFIG",
-            logger=logger,
-            device_to_settings_map=device_to_settings_map,
-            job_class_instance=job_class_instance,
-            jinja_env=jinja_env,
+        ) as nornir_obj:
+            nr_with_processors = nornir_obj.with_processors([ProcessGoldenConfig(logger)])
+
+            logger.debug("Run nornir render config tasks.")
+            # Run the Nornir Tasks
+            results = nr_with_processors.run(
+                task=run_template,
+                name="RENDER CONFIG",
+                logger=logger,
+                device_to_settings_map=job.device_to_settings_map,
+                job_class_instance=job,
+                jinja_env=jinja_env,
+            )
+    except NornirNautobotException as err:
+        logger.error(
+            f"`E3029:` NornirNautobotException raised during intended tasks. Original exception message: ```{err}```"
         )
+        # re-raise Exception if it's raised from nornir-nautobot or nautobot-app-nornir
+        if str(err).startswith("`E2") or str(err).startswith("`E1"):
+            raise NornirNautobotException(err) from err
+    if results.failed:
+        raise IntendedGenerationFailure()
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/nornir_plays/processor.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/processor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 """Processor used by Golden Config to catch unknown errors."""
 from nornir.core.inventory import Host
-from nornir.core.task import AggregatedResult, MultiResult, Result, Task
+from nornir.core.task import MultiResult, Result, Task
 from nornir_nautobot.exceptions import NornirNautobotException
 from nornir_nautobot.plugins.processors import BaseLoggingProcessor
 
 
 class ProcessGoldenConfig(BaseLoggingProcessor):
     """Processor class for golden configuration jobs."""
 
     def __init__(self, logger):
         """Set logging facility."""
         self.logger = logger
 
-    def task_completed(self, task: Task, result: AggregatedResult) -> None:
-        """Task outside of thread to determine what to do."""
-        if result.failed:
-            self.logger.error(f"{task.name} failed: {result}")
-            raise ValueError(result)
-
     def _find_result_exceptions(self, result):
         """Walk the results and return only valid Exceptions.
 
         NornirNautobotException is expected to be raised in some situations.
         """
         valid_exceptions = []
         if result.failed:
@@ -52,13 +46,7 @@
         host.close_connections()
         exceptions = self._find_result_exceptions(result)
 
         if result.failed and exceptions:
             exception_string = ", ".join([str(e[0]) for e in exceptions])
             # Log only exception summary to users
             self.logger.error(f"{task.name} failed: {exception_string}", extra={"object": task.host.data["obj"]})
-            for exception in exceptions:
-                # Log full exception and traceback to debug
-                self.logger.warning(
-                    f"""{task.host}, {task.name} failed: {exception[0]} {exception[1]}""",
-                    extra={"object": task.host.data["obj"]},
-                )
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/signals.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/404.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/404.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html`

 * *Files 2% similar despite different names*

```diff
@@ -1768,14 +1768,41 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
+  <a href="#v204-2024-04" class="md-nav__link">
+    v2.0.4 2024-04
+  </a>
+  
+    <nav class="md-nav" aria-label="v2.0.4 2024-04">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#fixed" class="md-nav__link">
+    Fixed
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#housekeeping" class="md-nav__link">
+    Housekeeping
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
   <a href="#v203-2024-03" class="md-nav__link">
     v2.0.3 2024-03
   </a>
   
     <nav class="md-nav" aria-label="v2.0.3 2024-03">
       <ul class="md-nav__list">
         
@@ -1783,15 +1810,15 @@
   <a href="#added" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed" class="md-nav__link">
+  <a href="#fixed_1" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
       </ul>
     </nav>
@@ -1810,15 +1837,15 @@
   <a href="#added_1" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_1" class="md-nav__link">
+  <a href="#fixed_2" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed" class="md-nav__link">
@@ -1837,15 +1864,15 @@
     v2.0.1 - 2023-12
   </a>
   
     <nav class="md-nav" aria-label="v2.0.1 - 2023-12">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed_2" class="md-nav__link">
+  <a href="#fixed_3" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed_1" class="md-nav__link">
@@ -2396,14 +2423,41 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
+  <a href="#v204-2024-04" class="md-nav__link">
+    v2.0.4 2024-04
+  </a>
+  
+    <nav class="md-nav" aria-label="v2.0.4 2024-04">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#fixed" class="md-nav__link">
+    Fixed
+  </a>
+  
+</li>
+        
+          <li class="md-nav__item">
+  <a href="#housekeeping" class="md-nav__link">
+    Housekeeping
+  </a>
+  
+</li>
+        
+      </ul>
+    </nav>
+  
+</li>
+      
+        <li class="md-nav__item">
   <a href="#v203-2024-03" class="md-nav__link">
     v2.0.3 2024-03
   </a>
   
     <nav class="md-nav" aria-label="v2.0.3 2024-03">
       <ul class="md-nav__list">
         
@@ -2411,15 +2465,15 @@
   <a href="#added" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed" class="md-nav__link">
+  <a href="#fixed_1" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
       </ul>
     </nav>
@@ -2438,15 +2492,15 @@
   <a href="#added_1" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_1" class="md-nav__link">
+  <a href="#fixed_2" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed" class="md-nav__link">
@@ -2465,15 +2519,15 @@
     v2.0.1 - 2023-12
   </a>
   
     <nav class="md-nav" aria-label="v2.0.1 - 2023-12">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed_2" class="md-nav__link">
+  <a href="#fixed_3" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed_1" class="md-nav__link">
@@ -2562,30 +2616,39 @@
 <li>Moved config compliance view to be a tab within device instead of a dedicated page.</li>
 <li>Removed management command in favor of Nautobot Core's.</li>
 </ul>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>Please see <a href="../migrating_to_v2.html">migrating guide</a> for details on migration.</p>
 </div>
+<h2 id="v204-2024-04">v2.0.4 2024-04<a class="headerlink" href="#v204-2024-04" title="Permanent link">&para;</a></h2>
+<h3 id="fixed">Fixed<a class="headerlink" href="#fixed" title="Permanent link">&para;</a></h3>
+<ul>
+<li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/749">#749</a> - Corrected issue where consecutive Golden Config Jobs in All Golden Configs Job wouldn't execute if prior Job had an Exception raised.</li>
+</ul>
+<h3 id="housekeeping">Housekeeping<a class="headerlink" href="#housekeeping" title="Permanent link">&para;</a></h3>
+<ul>
+<li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/741">#741</a> - Re-baked from the latest template.</li>
+</ul>
 <h2 id="v203-2024-03">v2.0.3 2024-03<a class="headerlink" href="#v203-2024-03" title="Permanent link">&para;</a></h2>
 <h3 id="added">Added<a class="headerlink" href="#added" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/736">#736</a> - Add a boolean job parameter <code>fail_job_on_task_failure</code> which will determine whether a single task failure anywhere in the job-result should result in job-result status of failed vs successful.</li>
 </ul>
-<h3 id="fixed">Fixed<a class="headerlink" href="#fixed" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_1">Fixed<a class="headerlink" href="#fixed_1" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/736">#736</a> - Fixes repo push and commit not executing if a exception was raised on any task inside a job.</li>
 </ul>
 <h2 id="v202-2024-03">v2.0.2 - 2024-03<a class="headerlink" href="#v202-2024-03" title="Permanent link">&para;</a></h2>
 <h3 id="added_1">Added<a class="headerlink" href="#added_1" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Added autoformat invoke command.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/730">#730</a> - Added app config schema generator and validator.</li>
 </ul>
-<h3 id="fixed_1">Fixed<a class="headerlink" href="#fixed_1" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_2">Fixed<a class="headerlink" href="#fixed_2" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/699">#699</a> - Fixed stale reference to platform_slug_map.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/719">#719</a> - Fixed generate config plans Status filter.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/715">#715</a> - Fixed close threaded db connections during config deployment.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/726">#726</a> - Fixed objectchange log excludes for object_data_v2 data as well.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/718">#718</a> - Fixed logic to handle jobs requiring approvals.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/724">#724</a> - Fixed performance issue on UNIX file diff view.</li>
@@ -2596,15 +2659,15 @@
 <h3 id="changed">Changed<a class="headerlink" href="#changed" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/691">#691</a> - Changed repo name and references to nautobot-app-golden-config.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Changed from pydocstyle to ruff.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Changed release notes to towncrier based.</li>
 </ul>
 <h2 id="v201-2023-12">v2.0.1 - 2023-12<a class="headerlink" href="#v201-2023-12" title="Permanent link">&para;</a></h2>
-<h3 id="fixed_2">Fixed<a class="headerlink" href="#fixed_2" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_3">Fixed<a class="headerlink" href="#fixed_3" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/676">#676</a> - Fixes docs for running config plan job in 2.0.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/680">#680</a> - Resolve RTD build issue.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/684">#684</a> - Fix repo sync not executing on any task failure.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/685">#685</a> - Cherry-pick #669 - Removed unneeded lookup for GoldenConfigSetting.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/686">#686</a> - Fix incorrect permissions.</li>
 </ul>
```

#### html2text {}

```diff
@@ -70,14 +70,17 @@
                 # _E_3_0_2_5
                 # _E_3_0_2_6
           o _M_i_g_r_a_t_i_n_g_ _T_o_ _v_2
           o 
             _R_e_l_e_a_s_e_ _N_o_t_e_s
             Release Notes
                 # ??v2.0 _v_2_._0_ Table of contents
+                      # _v_2_._0_._4_ _2_0_2_4_-_0_4
+                            # _F_i_x_e_d
+                            # _H_o_u_s_e_k_e_e_p_i_n_g
                       # _v_2_._0_._3_ _2_0_2_4_-_0_3
                             # _A_d_d_e_d
                             # _F_i_x_e_d
                       # _v_2_._0_._2_ _-_ _2_0_2_4_-_0_3
                             # _A_d_d_e_d
                             # _F_i_x_e_d
                             # _C_h_a_n_g_e_d
@@ -106,14 +109,17 @@
             _C_o_d_e_ _R_e_f_e_r_e_n_c_e
             Code Reference
                 # _M_o_d_e_l_s
                 # _P_a_c_k_a_g_e
                 # _A_P_I
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
 Table of contents
+    * _v_2_._0_._4_ _2_0_2_4_-_0_4
+          o _F_i_x_e_d
+          o _H_o_u_s_e_k_e_e_p_i_n_g
     * _v_2_._0_._3_ _2_0_2_4_-_0_3
           o _A_d_d_e_d
           o _F_i_x_e_d
     * _v_2_._0_._2_ _-_ _2_0_2_4_-_0_3
           o _A_d_d_e_d
           o _F_i_x_e_d
           o _C_h_a_n_g_e_d
@@ -134,14 +140,20 @@
       MERGE_CONFIG_FRAMEWORK, and REPLACE_CONFIG_FRAMEWORK) and
       customer_dispatcher to remove dispatcher_mapping.
     * Moved config compliance view to be a tab within device instead of a
       dedicated page.
     * Removed management command in favor of Nautobot Core's.
 Note
 Please see _m_i_g_r_a_t_i_n_g_ _g_u_i_d_e for details on migration.
+********** vv22..00..44 22002244--0044_?¶ **********
+******** FFiixxeedd_?¶ ********
+    * _#_7_4_9 - Corrected issue where consecutive Golden Config Jobs in All Golden
+      Configs Job wouldn't execute if prior Job had an Exception raised.
+******** HHoouusseekkeeeeppiinngg_?¶ ********
+    * _#_7_4_1 - Re-baked from the latest template.
 ********** vv22..00..33 22002244--0033_?¶ **********
 ******** AAddddeedd_?¶ ********
     * _#_7_3_6 - Add a boolean job parameter fail_job_on_task_failure which will
       determine whether a single task failure anywhere in the job-result should
       result in job-result status of failed vs successful.
 ******** FFiixxeedd_?¶ ********
     * _#_7_3_6 - Fixes repo push and commit not executing if a exception was raised
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html`

 * *Files 4% similar despite different names*

```diff
@@ -2380,44 +2380,36 @@
 <h2 id="branching-policy">Branching Policy<a class="headerlink" href="#branching-policy" title="Permanent link">&para;</a></h2>
 <p>The branching policy includes the following tenets:</p>
 <ul>
 <li>The <code>develop</code> branch is the branch of the next major and minor paired version planned.</li>
 <li>PRs intended to add new features should be sourced from the <code>develop</code> branch.</li>
 <li>PRs intended to fix issues in the Nautobot LTM compatible release should be sourced from the latest <code>ltm-&lt;major.minor&gt;</code> branch instead of <code>develop</code>.</li>
 </ul>
-<p>Golden Config will observe semantic versioning, as of 1.0. This may result in a quick turnaround in minor versions to keep pace with an ever growing feature set.</p>
+<p>Golden Config will observe semantic versioning, as of 1.0. This may result in a quick turnaround in minor versions to keep pace with an ever-growing feature set.</p>
 <h2 id="release-policy">Release Policy<a class="headerlink" href="#release-policy" title="Permanent link">&para;</a></h2>
 <p>Golden Config has currently no intended scheduled release schedule, and will release new features in minor versions.</p>
 <p>When a release is ready to be created from either <code>develop</code> or <code>ltm-x.x</code>, the following should happen.</p>
 <ul>
-<li>Create a release PR by:<ul>
-<li>Source from <code>develop</code> or <code>ltm-&lt;major&gt;.&lt;minor&gt;</code> branch and creatch new branch, generally <code>release/&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li>
-<li>Update the release notes in <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> file to reflect the changes.<ul>
-<li>You can run <code>invoke generate-release-notes</code> to generate these notes and delete the legacy towncrier fragments.</li>
-<li>Please consider adding changelog's from ltm releases in current release, as applicable.</li>
-</ul>
-</li>
-<li>Update the mkdocs.yml file to include the reference to <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> as applicable.</li>
+<li>A release PR is created from <code>develop</code> with:<ul>
+<li>Update the release notes in <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> file to reflect the changes.</li>
 <li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;-beta</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> in <code>pyproject.toml</code>.</li>
-<li>Set the PR to the <code>main</code> or <code>ltm-&lt;major&gt;.&lt;minor&gt;</code> branch respectively.</li>
+<li>Set the PR to the <code>main</code> branch.</li>
 </ul>
 </li>
 <li>Ensure the tests for the PR pass.</li>
 <li>Merge the PR.</li>
 <li>Create a new tag:<ul>
 <li>The tag should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li>
 <li>The title should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li>
 <li>The description should be the changes that were added to the <code>version_&lt;major&gt;.&lt;minor&gt;.md</code> document.</li>
-<li>Include full changelog in description <code>**Full Changelog**: https://github.com/nautobot/&lt;repo-name&gt;/compare/v&lt;prior-verion&gt;...v&lt;current-verion&gt;</code>.</li>
-<li><strong>Note</strong> Please ensure to uncheck <code>Set as the latest release</code> when updating an ltm release.</li>
 </ul>
 </li>
 <li>If merged into <code>main</code>, then push from <code>main</code> to <code>develop</code>, in order to retain the merge commit created when the PR was merged</li>
 <li>A post release PR is created with:<ul>
-<li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch + 1&gt;-beta</code> in <code>pyproject.toml</code>.</li>
+<li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch + 1&gt;-beta</code> in both <code>pyproject.toml</code> and <code>nautobot.__init__.__version__</code>.</li>
 <li>Set the PR to the proper branch, <code>develop</code>.</li>
 <li>Once tests pass, merge.</li>
 </ul>
 </li>
 </ul>
```

#### html2text {}

```diff
@@ -145,52 +145,40 @@
     * The develop branch is the branch of the next major and minor paired
       version planned.
     * PRs intended to add new features should be sourced from the develop
       branch.
     * PRs intended to fix issues in the Nautobot LTM compatible release should
       be sourced from the latest ltm-<major.minor> branch instead of develop.
 Golden Config will observe semantic versioning, as of 1.0. This may result in a
-quick turnaround in minor versions to keep pace with an ever growing feature
+quick turnaround in minor versions to keep pace with an ever-growing feature
 set.
 ********** RReelleeaassee PPoolliiccyy_?¶ **********
 Golden Config has currently no intended scheduled release schedule, and will
 release new features in minor versions.
 When a release is ready to be created from either develop or ltm-x.x, the
 following should happen.
-    * Create a release PR by:
-          o Source from develop or ltm-<major>.<minor> branch and creatch new
-            branch, generally release/<major>.<minor>.<patch>.
+    * A release PR is created from develop with:
           o Update the release notes in docs/admin/release_notes/
             version_<major>.<minor>.md file to reflect the changes.
-                # You can run invoke generate-release-notes to generate these
-                  notes and delete the legacy towncrier fragments.
-                # Please consider adding changelog's from ltm releases in
-                  current release, as applicable.
-          o Update the mkdocs.yml file to include the reference to docs/admin/
-            release_notes/version_<major>.<minor>.md as applicable.
           o Change the version from <major>.<minor>.<patch>-beta to
             <major>.<minor>.<patch> in pyproject.toml.
-          o Set the PR to the main or ltm-<major>.<minor> branch respectively.
+          o Set the PR to the main branch.
     * Ensure the tests for the PR pass.
     * Merge the PR.
     * Create a new tag:
           o The tag should be in the form of v<major>.<minor>.<patch>.
           o The title should be in the form of v<major>.<minor>.<patch>.
           o The description should be the changes that were added to the
             version_<major>.<minor>.md document.
-          o Include full changelog in description **Full Changelog**: https://
-            github.com/nautobot/<repo-name>/compare/v<prior-
-            verion>...v<current-verion>.
-          o NNoottee Please ensure to uncheck Set as the latest release when
-            updating an ltm release.
     * If merged into main, then push from main to develop, in order to retain
       the merge commit created when the PR was merged
     * A post release PR is created with:
           o Change the version from <major>.<minor>.<patch> to
-            <major>.<minor>.<patch + 1>-beta in pyproject.toml.
+            <major>.<minor>.<patch + 1>-beta in both pyproject.toml and
+            nautobot.__init__.__version__.
           o Set the PR to the proper branch, develop.
           o Once tests pass, merge.
 _P_r_e_v_i_o_u_s
 _E_x_t_e_n_d_i_n_g_ _t_h_e_ _A_p_p
 _N_e_x_t
 _D_e_v_e_l_o_p_m_e_n_t_ _E_n_v_i_r_o_n_m_e_n_t
 Copyright © The Authors
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/index.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9897270114942529%*

 * *Differences: {"'docs'": "{135: {'location': 'admin/release_notes/version_2.0.html#fixed_1'}, 138: {'location': "*

 * *           "'admin/release_notes/version_2.0.html#fixed_2'}, 141: {'location': "*

 * *           "'admin/release_notes/version_2.0.html#fixed_3'}, 318: {'text': '<p>The branching "*

 * *           'policy includes the following tenets:</p> <ul> <li>The <code>develop</code> branch is '*

 * *           'the branch of the next major and minor paired version planned.</li> <li>PRs intended '*

 * *           'to add new features shoul […]*

```diff
@@ -656,55 +656,70 @@
         },
         {
             "location": "admin/release_notes/version_2.0.html",
             "text": "<ul> <li>Updated <code>nautobot</code> to <code>2.0.0</code> and made associated changes.</li> <li>Integrated all relevant sections with <code>Platform.network_driver</code>.</li> <li>Added a standard way to provide error codes.</li> <li>Changed Config Compliance view to be based on model, not dynamic group and provide a <code>message</code> when they have drifted.</li> <li>Added constance settings (<code>DEFAULT_FRAMEWORK</code>, <code>GET_CONFIG_FRAMEWORK</code>, <code>MERGE_CONFIG_FRAMEWORK</code>, and <code>REPLACE_CONFIG_FRAMEWORK</code>) and customer_dispatcher to remove dispatcher_mapping.</li> <li>Moved config compliance view to be a tab within device instead of a dedicated page.</li> <li>Removed management command in favor of Nautobot Core's.</li> </ul> <p>Note</p> <p>Please see migrating guide for details on migration.</p>",
             "title": "v2.0 Release Notes"
         },
         {
+            "location": "admin/release_notes/version_2.0.html#v204-2024-04",
+            "text": "",
+            "title": "v2.0.4 2024-04"
+        },
+        {
+            "location": "admin/release_notes/version_2.0.html#fixed",
+            "text": "<ul> <li>#749 - Corrected issue where consecutive Golden Config Jobs in All Golden Configs Job wouldn't execute if prior Job had an Exception raised.</li> </ul>",
+            "title": "Fixed"
+        },
+        {
+            "location": "admin/release_notes/version_2.0.html#housekeeping",
+            "text": "<ul> <li>#741 - Re-baked from the latest template.</li> </ul>",
+            "title": "Housekeeping"
+        },
+        {
             "location": "admin/release_notes/version_2.0.html#v203-2024-03",
             "text": "",
             "title": "v2.0.3 2024-03"
         },
         {
             "location": "admin/release_notes/version_2.0.html#added",
             "text": "<ul> <li>#736 - Add a boolean job parameter <code>fail_job_on_task_failure</code> which will determine whether a single task failure anywhere in the job-result should result in job-result status of failed vs successful.</li> </ul>",
             "title": "Added"
         },
         {
-            "location": "admin/release_notes/version_2.0.html#fixed",
+            "location": "admin/release_notes/version_2.0.html#fixed_1",
             "text": "<ul> <li>#736 - Fixes repo push and commit not executing if a exception was raised on any task inside a job.</li> </ul>",
             "title": "Fixed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#v202-2024-03",
             "text": "",
             "title": "v2.0.2 - 2024-03"
         },
         {
             "location": "admin/release_notes/version_2.0.html#added_1",
             "text": "<ul> <li>#707 - Added autoformat invoke command.</li> <li>#730 - Added app config schema generator and validator.</li> </ul>",
             "title": "Added"
         },
         {
-            "location": "admin/release_notes/version_2.0.html#fixed_1",
+            "location": "admin/release_notes/version_2.0.html#fixed_2",
             "text": "<ul> <li>#699 - Fixed stale reference to platform_slug_map.</li> <li>#719 - Fixed generate config plans Status filter.</li> <li>#715 - Fixed close threaded db connections during config deployment.</li> <li>#726 - Fixed objectchange log excludes for object_data_v2 data as well.</li> <li>#718 - Fixed logic to handle jobs requiring approvals.</li> <li>#724 - Fixed performance issue on UNIX file diff view.</li> <li>#724 - Fixed non-working repos list creation and syncing.</li> <li>#731 - Fixed missing right panel with config types.</li> <li>#734 - Fixed incorrect netutils_parser lookup.</li> </ul>",
             "title": "Fixed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#changed",
             "text": "<ul> <li>#691 - Changed repo name and references to nautobot-app-golden-config.</li> <li>#707 - Changed from pydocstyle to ruff.</li> <li>#707 - Changed release notes to towncrier based.</li> </ul>",
             "title": "Changed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#v201-2023-12",
             "text": "",
             "title": "v2.0.1 - 2023-12"
         },
         {
-            "location": "admin/release_notes/version_2.0.html#fixed_2",
+            "location": "admin/release_notes/version_2.0.html#fixed_3",
             "text": "<ul> <li>#676 - Fixes docs for running config plan job in 2.0.</li> <li>#680 - Resolve RTD build issue.</li> <li>#684 - Fix repo sync not executing on any task failure.</li> <li>#685 - Cherry-pick #669 - Removed unneeded lookup for GoldenConfigSetting.</li> <li>#686 - Fix incorrect permissions.</li> </ul>",
             "title": "Fixed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#changed_1",
             "text": "<ul> <li>#658 - Cookie updated by NetworkToCode Cookie Drift Manager Tool.</li> <li>#671 - Finish Documentation Updates from Drift Manager.</li> </ul>",
             "title": "Changed"
@@ -1381,14 +1396,114 @@
         },
         {
             "location": "admin/troubleshooting/E3026.html#recommendation",
             "text": "<p>Recommendation that is coming soon.</p>",
             "title": "Recommendation:"
         },
         {
+            "location": "admin/troubleshooting/E3027.html",
+            "text": "",
+            "title": "E3027 Details"
+        },
+        {
+            "location": "admin/troubleshooting/E3027.html#message-emitted",
+            "text": "<p><code>E3027: NornirNautobotException raised during backup tasks. Original exception message</code></p>",
+            "title": "Message emitted:"
+        },
+        {
+            "location": "admin/troubleshooting/E3027.html#description",
+            "text": "<p>A NornirNautobotException is raised during a Backup Job.</p>",
+            "title": "Description:"
+        },
+        {
+            "location": "admin/troubleshooting/E3027.html#troubleshooting",
+            "text": "<p>Review the exception message and worker logs to determine the cause of the failure.</p>",
+            "title": "Troubleshooting:"
+        },
+        {
+            "location": "admin/troubleshooting/E3027.html#recommendation",
+            "text": "<p>This type of error is usually resource related or caused by a misconfiguration and should be logged as such.</p>",
+            "title": "Recommendation:"
+        },
+        {
+            "location": "admin/troubleshooting/E3028.html",
+            "text": "",
+            "title": "E3028 Details"
+        },
+        {
+            "location": "admin/troubleshooting/E3028.html#message-emitted",
+            "text": "<p><code>E3028: NornirNautobotException raised during compliance tasks. Original exception message</code></p>",
+            "title": "Message emitted:"
+        },
+        {
+            "location": "admin/troubleshooting/E3028.html#description",
+            "text": "<p>A NornirNautobotException is raised during a Compliance Job.</p>",
+            "title": "Description:"
+        },
+        {
+            "location": "admin/troubleshooting/E3028.html#troubleshooting",
+            "text": "<p>Review the exception message and worker logs to determine the cause of the failure.</p>",
+            "title": "Troubleshooting:"
+        },
+        {
+            "location": "admin/troubleshooting/E3028.html#recommendation",
+            "text": "<p>This type of error is usually resource related or caused by a misconfiguration and should be logged as such.</p>",
+            "title": "Recommendation:"
+        },
+        {
+            "location": "admin/troubleshooting/E3029.html",
+            "text": "",
+            "title": "E3029 Details"
+        },
+        {
+            "location": "admin/troubleshooting/E3029.html#message-emitted",
+            "text": "<p><code>E3029: NornirNautobotException raised during intended tasks. Original exception message</code></p>",
+            "title": "Message emitted:"
+        },
+        {
+            "location": "admin/troubleshooting/E3029.html#description",
+            "text": "<p>A NornirNautobotException is raised during an Intended Job.</p>",
+            "title": "Description:"
+        },
+        {
+            "location": "admin/troubleshooting/E3029.html#troubleshooting",
+            "text": "<p>Review the exception message and worker logs to determine the cause of the failure.</p>",
+            "title": "Troubleshooting:"
+        },
+        {
+            "location": "admin/troubleshooting/E3029.html#recommendation",
+            "text": "<p>This type of error is usually resource related or caused by a misconfiguration and should be logged as such.</p>",
+            "title": "Recommendation:"
+        },
+        {
+            "location": "admin/troubleshooting/E3030.html",
+            "text": "",
+            "title": "E3030 Details"
+        },
+        {
+            "location": "admin/troubleshooting/E3030.html#message-emitted",
+            "text": "<p><code>E3030: Failure during (Backup, Intended, Compliance) Job(s).</code></p>",
+            "title": "Message emitted:"
+        },
+        {
+            "location": "admin/troubleshooting/E3030.html#description",
+            "text": "<p>A NornirNautobotException is raised during a Backup, Intended, or Compliance Job.</p>",
+            "title": "Description:"
+        },
+        {
+            "location": "admin/troubleshooting/E3030.html#troubleshooting",
+            "text": "<p>Review the exception message and worker logs to determine the cause of the failure.</p>",
+            "title": "Troubleshooting:"
+        },
+        {
+            "location": "admin/troubleshooting/E3030.html#recommendation",
+            "text": "<p>This type of error is usually resource related or caused by a misconfiguration and should be logged as such.</p>",
+            "title": "Recommendation:"
+        },
+        {
             "location": "dev/arch_decision.html",
             "text": "<p>The intention is to document deviations from a standard Model View Controller (MVC) design.</p>",
             "title": "Architecture Decision Records"
         },
         {
             "location": "dev/arch_decision.html#pivoting-compliance-view",
             "text": "<p>The view that was preferred for compliance would be devices on y-axis but the features on the x-axis. However, the x-axis (features) cannot be known when building the Django model. The model ends up looking like:</p> Device feature Compliance nyc-rt01 aaa True nyc-rt01 ntp False nyc-rt01 dns False nyc-rt02 aaa True nyc-rt02 dns False <p>The expected view required expected is something like:</p> Device aaa dns ntp nyc-rt01 True False False nyc-rt02 True False <p>In order to accommodate this, <code>django-pivot</code> is used, which greatly simplifies building the query. However, <code>django-pivot</code> requires the ability to \"count\" versus a boolean. Because of that, there is a \"shadow\" field created that is set to 0 if False, and 1 if True. This is enforced on the <code>save</code> method of the <code>ConfigCompliance</code> model.</p>",
@@ -1482,20 +1597,20 @@
         {
             "location": "dev/contributing.html#creating-changelog-fragments",
             "text": "<p>All pull requests to <code>next</code> or <code>develop</code> must include a changelog fragment file in the <code>./changes</code> directory. To create a fragment, use your GitHub issue number and fragment type as the filename. For example, <code>2362.added</code>. Valid fragment types are <code>added</code>, <code>changed</code>, <code>deprecated</code>, <code>fixed</code>, <code>removed</code>, and <code>security</code>. The change summary is added to the file in plain text. Change summaries should be complete sentences, starting with a capital letter and ending with a period, and be in past tense. Each line of the change fragment will generate a single change entry in the release notes. Use multiple lines in the same file if your change needs to generate multiple release notes in the same category. If the change needs to create multiple entries in separate categories, create multiple files.</p> <p>Example</p> <p>Wrong changes/1234.fixed<pre><code>fix critical bug in documentation\n</code></pre></p> <p>Right changes/1234.fixed<pre><code>Fixed critical bug in documentation.\n</code></pre></p> <p>Multiple Entry Example</p> <p>This will generate 2 entries in the <code>fixed</code> category and one entry in the <code>changed</code> category.</p> changes/1234.fixed<pre><code>Fixed critical bug in documentation.\nFixed release notes generation.\n</code></pre> changes/1234.changed<pre><code>Changed release notes generation.\n</code></pre>",
             "title": "Creating Changelog Fragments"
         },
         {
             "location": "dev/contributing.html#branching-policy",
-            "text": "<p>The branching policy includes the following tenets:</p> <ul> <li>The <code>develop</code> branch is the branch of the next major and minor paired version planned.</li> <li>PRs intended to add new features should be sourced from the <code>develop</code> branch.</li> <li>PRs intended to fix issues in the Nautobot LTM compatible release should be sourced from the latest <code>ltm-&lt;major.minor&gt;</code> branch instead of <code>develop</code>.</li> </ul> <p>Golden Config will observe semantic versioning, as of 1.0. This may result in a quick turnaround in minor versions to keep pace with an ever growing feature set.</p>",
+            "text": "<p>The branching policy includes the following tenets:</p> <ul> <li>The <code>develop</code> branch is the branch of the next major and minor paired version planned.</li> <li>PRs intended to add new features should be sourced from the <code>develop</code> branch.</li> <li>PRs intended to fix issues in the Nautobot LTM compatible release should be sourced from the latest <code>ltm-&lt;major.minor&gt;</code> branch instead of <code>develop</code>.</li> </ul> <p>Golden Config will observe semantic versioning, as of 1.0. This may result in a quick turnaround in minor versions to keep pace with an ever-growing feature set.</p>",
             "title": "Branching Policy"
         },
         {
             "location": "dev/contributing.html#release-policy",
-            "text": "<p>Golden Config has currently no intended scheduled release schedule, and will release new features in minor versions.</p> <p>When a release is ready to be created from either <code>develop</code> or <code>ltm-x.x</code>, the following should happen.</p> <ul> <li>Create a release PR by:<ul> <li>Source from <code>develop</code> or <code>ltm-&lt;major&gt;.&lt;minor&gt;</code> branch and creatch new branch, generally <code>release/&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li> <li>Update the release notes in <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> file to reflect the changes.<ul> <li>You can run <code>invoke generate-release-notes</code> to generate these notes and delete the legacy towncrier fragments.</li> <li>Please consider adding changelog's from ltm releases in current release, as applicable.</li> </ul> </li> <li>Update the mkdocs.yml file to include the reference to <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> as applicable.</li> <li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;-beta</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> in <code>pyproject.toml</code>.</li> <li>Set the PR to the <code>main</code> or <code>ltm-&lt;major&gt;.&lt;minor&gt;</code> branch respectively.</li> </ul> </li> <li>Ensure the tests for the PR pass.</li> <li>Merge the PR.</li> <li>Create a new tag:<ul> <li>The tag should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li> <li>The title should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li> <li>The description should be the changes that were added to the <code>version_&lt;major&gt;.&lt;minor&gt;.md</code> document.</li> <li>Include full changelog in description <code>**Full Changelog**: https://github.com/nautobot/&lt;repo-name&gt;/compare/v&lt;prior-verion&gt;...v&lt;current-verion&gt;</code>.</li> <li>Note Please ensure to uncheck <code>Set as the latest release</code> when updating an ltm release.</li> </ul> </li> <li>If merged into <code>main</code>, then push from <code>main</code> to <code>develop</code>, in order to retain the merge commit created when the PR was merged</li> <li>A post release PR is created with:<ul> <li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch + 1&gt;-beta</code> in <code>pyproject.toml</code>.</li> <li>Set the PR to the proper branch, <code>develop</code>.</li> <li>Once tests pass, merge.</li> </ul> </li> </ul>",
+            "text": "<p>Golden Config has currently no intended scheduled release schedule, and will release new features in minor versions.</p> <p>When a release is ready to be created from either <code>develop</code> or <code>ltm-x.x</code>, the following should happen.</p> <ul> <li>A release PR is created from <code>develop</code> with:<ul> <li>Update the release notes in <code>docs/admin/release_notes/version_&lt;major&gt;.&lt;minor&gt;.md</code> file to reflect the changes.</li> <li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;-beta</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> in <code>pyproject.toml</code>.</li> <li>Set the PR to the <code>main</code> branch.</li> </ul> </li> <li>Ensure the tests for the PR pass.</li> <li>Merge the PR.</li> <li>Create a new tag:<ul> <li>The tag should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li> <li>The title should be in the form of <code>v&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code>.</li> <li>The description should be the changes that were added to the <code>version_&lt;major&gt;.&lt;minor&gt;.md</code> document.</li> </ul> </li> <li>If merged into <code>main</code>, then push from <code>main</code> to <code>develop</code>, in order to retain the merge commit created when the PR was merged</li> <li>A post release PR is created with:<ul> <li>Change the version from <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;</code> to <code>&lt;major&gt;.&lt;minor&gt;.&lt;patch + 1&gt;-beta</code> in both <code>pyproject.toml</code> and <code>nautobot.__init__.__version__</code>.</li> <li>Set the PR to the proper branch, <code>develop</code>.</li> <li>Once tests pass, merge.</li> </ul> </li> </ul>",
             "title": "Release Policy"
         },
         {
             "location": "dev/dev_environment.html",
             "text": "",
             "title": "Building Your Development Environment"
         },
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml`

 * *Files 5% similar despite different names*

#### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml`

```diff
@@ -1,353 +1,373 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/index.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/compatibility_matrix.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/install.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/migrating_to_v2.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/uninstall.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/upgrade.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/index.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_0.10.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_0.9.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.0.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.1.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.2.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.3.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.4.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.5.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.6.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_2.0.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/index.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3001.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3002.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3003.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3004.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3005.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3006.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3007.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3008.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3009.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3010.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3011.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3012.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3013.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3014.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3015.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3016.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3017.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3018.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3019.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3020.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3021.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3022.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3023.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3024.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3025.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3026.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
+    <changefreq>daily</changefreq>
+  </url>
+  <url>
+    <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3027.html</loc>
+    <lastmod>2024-04-03</lastmod>
+    <changefreq>daily</changefreq>
+  </url>
+  <url>
+    <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3028.html</loc>
+    <lastmod>2024-04-03</lastmod>
+    <changefreq>daily</changefreq>
+  </url>
+  <url>
+    <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3029.html</loc>
+    <lastmod>2024-04-03</lastmod>
+    <changefreq>daily</changefreq>
+  </url>
+  <url>
+    <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3030.html</loc>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/arch_decision.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/contributing.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_environment.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/extending.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/index.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/api.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/models.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/package.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_backup.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliance.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancecli.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancecustom.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancejson.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_config_plans.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_config_postprocessing.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_intended.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_remediation.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_sotagg.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_getting_started.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_overview.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_use_cases.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/external_interactions.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/faq.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_credentials.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_dispatchers.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_general.html</loc>
-    <lastmod>2024-03-14</lastmod>
+    <lastmod>2024-04-03</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/run_job.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/run_job.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/static/toggle_fields.js` & `nautobot_golden_config-2.0.4/nautobot_golden_config/static/toggle_fields.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tables.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/template_content.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/content_template.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/content_template.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html` & `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/conftest.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/forms/test_golden_config_settings.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/test_golden_config_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_api.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_basic.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_datasources.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_filters.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_graphql.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_helpers.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_jobs.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_models.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_config_plan.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_config_plan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_git.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_graphql.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_utilities/test_helpers.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/tests/test_views.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/urls.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/config_plan.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_plan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/config_postprocessing.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_postprocessing.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/constant.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/constant.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/db_management.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/db_management.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/git.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/graphql.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/helper.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/logger.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/mat_plot.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/mat_plot.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/utilities/utils.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/nautobot_golden_config/views.py` & `nautobot_golden_config-2.0.4/nautobot_golden_config/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.3/pyproject.toml` & `nautobot_golden_config-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-golden-config"
-version = "v2.0.3"
+version = "v2.0.4"
 description = "An app for configuration on nautobot"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-app-golden-config"
 repository = "https://github.com/nautobot/nautobot-app-golden-config"
 documentation = "https://docs.nautobot.com/projects/golden-config/en/latest/"
```

### Comparing `nautobot_golden_config-2.0.3/PKG-INFO` & `nautobot_golden_config-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-golden-config
-Version: 2.0.3
+Version: 2.0.4
 Summary: An app for configuration on nautobot
 Home-page: https://github.com/nautobot/nautobot-app-golden-config
 License: Apache-2.0
 Keywords: nautobot,nautobot-app,nautobot-plugin
 Author: Network to Code, LLC
 Author-email: opensource@networktocode.com
 Requires-Python: >=3.8,<3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nautobot-golden-config Version: 2.0.3 Summary: An
+Metadata-Version: 2.1 Name: nautobot-golden-config Version: 2.0.4 Summary: An
 app for configuration on nautobot Home-page: https://github.com/nautobot/
 nautobot-app-golden-config License: Apache-2.0 Keywords: nautobot,nautobot-
 app,nautobot-plugin Author: Network to Code, LLC Author-email:
 opensource@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

