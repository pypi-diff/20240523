# Comparing `tmp/nautobot_golden_config-2.0.4.tar.gz` & `tmp/nautobot_golden_config-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautobot_golden_config-2.0.4.tar", max compression
+gzip compressed data, was "nautobot_golden_config-2.0.5.tar", max compression
```

## Comparing `nautobot_golden_config-2.0.4.tar` & `nautobot_golden_config-2.0.5.tar`

### file list

```diff
@@ -1,295 +1,295 @@
--rw-r--r--   0        0        0      591 2024-04-03 00:39:45.454810 nautobot_golden_config-2.0.4/LICENSE
--rw-r--r--   0        0        0     7047 2024-04-03 00:39:45.454810 nautobot_golden_config-2.0.4/README.md
--rw-r--r--   0        0        0     3415 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/__init__.py
--rw-r--r--   0        0        0       54 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/__init__.py
--rw-r--r--   0        0        0     4023 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/serializers.py
--rw-r--r--   0        0        0     1071 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/urls.py
--rw-r--r--   0        0        0     6468 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/api/views.py
--rw-r--r--   0        0        0        5 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/app-config-schema.json
--rw-r--r--   0        0        0      950 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/choices.py
--rw-r--r--   0        0        0     9452 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/datasources.py
--rw-r--r--   0        0        0      745 2024-04-03 00:39:45.490810 nautobot_golden_config-2.0.4/nautobot_golden_config/exceptions.py
--rw-r--r--   0        0        0    14555 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/filters.py
--rw-r--r--   0        0        0    22228 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/forms.py
--rw-r--r--   0        0        0    25131 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/jobs.py
--rw-r--r--   0        0        0     4417 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/metrics.py
--rw-r--r--   0        0        0    12457 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0001_initial.py
--rw-r--r--   0        0        0      500 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0002_custom_data.py
--rw-r--r--   0        0        0     1814 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
--rw-r--r--   0        0        0     1824 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
--rw-r--r--   0        0        0     1538 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0005_json_compliance_rule.py
--rw-r--r--   0        0        0     1794 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
--rw-r--r--   0        0        0     2555 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
--rw-r--r--   0        0        0      665 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
--rw-r--r--   0        0        0     2558 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
--rw-r--r--   0        0        0      929 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
--rw-r--r--   0        0        0     1486 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
--rw-r--r--   0        0        0      909 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
--rw-r--r--   0        0        0      463 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
--rw-r--r--   0        0        0      429 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
--rw-r--r--   0        0        0      697 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
--rw-r--r--   0        0        0      742 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
--rw-r--r--   0        0        0     1594 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
--rw-r--r--   0        0        0      327 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
--rw-r--r--   0        0        0      678 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
--rw-r--r--   0        0        0     1113 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
--rw-r--r--   0        0        0      663 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
--rw-r--r--   0        0        0      389 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
--rw-r--r--   0        0        0      433 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0023_alter_custom_compliance.py
--rw-r--r--   0        0        0      936 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py
--rw-r--r--   0        0        0     2427 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0025_remediation_settings.py
--rw-r--r--   0        0        0     2925 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0026_configplan.py
--rw-r--r--   0        0        0     1243 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0027_auto_20230915_1657.py
--rw-r--r--   0        0        0     1332 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py
--rw-r--r--   0        0        0     7687 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py
--rw-r--r--   0        0        0      469 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0029_alter_configplan_unique_together.py
--rw-r--r--   0        0        0      581 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py
--rw-r--r--   0        0        0        0 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/__init__.py
--rw-r--r--   0        0        0    28162 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/models.py
--rw-r--r--   0        0        0     4837 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/navigation.py
--rw-r--r--   0        0        0       51 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/__init__.py
--rw-r--r--   0        0        0     6574 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_backup.py
--rw-r--r--   0        0        0     9174 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_compliance.py
--rw-r--r--   0        0        0     5626 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_deployment.py
--rw-r--r--   0        0        0     6132 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_intended.py
--rw-r--r--   0        0        0     2373 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/processor.py
--rwxr-xr-x   0        0        0     3430 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/signals.py
--rw-r--r--   0        0        0     5157 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css
--rw-r--r--   0        0        0    67022 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js
--rw-r--r--   0        0        0    51068 2024-04-03 00:40:54.330903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/404.html
--rw-r--r--   0        0        0    53070 2024-04-03 00:40:54.358903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html
--rw-r--r--   0        0        0    72938 2024-04-03 00:40:54.370903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html
--rw-r--r--   0        0        0    75234 2024-04-03 00:40:54.382903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html
--rw-r--r--   0        0        0    51442 2024-04-03 00:40:54.394903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html
--rw-r--r--   0        0        0    53317 2024-04-03 00:40:54.398903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html
--rw-r--r--   0        0        0    67535 2024-04-03 00:40:54.406903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html
--rw-r--r--   0        0        0    61279 2024-04-03 00:40:54.410903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html
--rw-r--r--   0        0        0    58323 2024-04-03 00:40:54.414903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html
--rw-r--r--   0        0        0    66552 2024-04-03 00:40:54.422903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html
--rw-r--r--   0        0        0    55655 2024-04-03 00:40:54.426903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html
--rw-r--r--   0        0        0    60872 2024-04-03 00:40:54.430903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html
--rw-r--r--   0        0        0    55522 2024-04-03 00:40:54.434903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html
--rw-r--r--   0        0        0    60059 2024-04-03 00:40:54.438903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html
--rw-r--r--   0        0        0    68745 2024-04-03 00:40:54.446903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html
--rw-r--r--   0        0        0    53504 2024-04-03 00:40:54.454903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.458903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.462903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.466903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.470903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.474903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.478903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.478903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.482903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.486903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.490903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.494903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.498903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.502903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.506903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.510903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.514903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.518903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.522903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.526903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.530903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.534903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.538903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.542903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html
--rw-r--r--   0        0        0    53466 2024-04-03 00:40:54.546903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html
--rw-r--r--   0        0        0    53512 2024-04-03 00:40:54.550903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html
--rw-r--r--   0        0        0    50870 2024-04-03 00:40:54.554903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3027.html
--rw-r--r--   0        0        0    50878 2024-04-03 00:40:54.554903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3028.html
--rw-r--r--   0        0        0    50875 2024-04-03 00:40:54.558903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3029.html
--rw-r--r--   0        0        0    50870 2024-04-03 00:40:54.562903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3030.html
--rw-r--r--   0        0        0    52256 2024-04-03 00:40:54.450903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html
--rw-r--r--   0        0        0    54288 2024-04-03 00:40:54.386903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html
--rw-r--r--   0        0        0    53811 2024-04-03 00:40:54.390903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html
--rw-r--r--   0        0        0     1000 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css
--rw-r--r--   0        0        0     5135 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css
--rw-r--r--   0        0        0    15086 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico
--rw-r--r--   0        0        0     1870 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png
--rw-r--r--   0        0        0    97321 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js
--rw-r--r--   0        0        0   891518 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map
--rw-r--r--   0        0        0    17074 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-r--r--   0        0        0     4654 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js
--rw-r--r--   0        0        0     6119 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js
--rw-r--r--   0        0        0     6208 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js
--rw-r--r--   0        0        0    11499 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js
--rw-r--r--   0        0        0     9342 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-r--r--   0        0        0    10669 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-r--r--   0        0        0     6882 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js
--rw-r--r--   0        0        0     3383 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js
--rw-r--r--   0        0        0     9437 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-r--r--   0        0        0     1264 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js
--rw-r--r--   0        0        0    11232 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js
--rw-r--r--   0        0        0     2313 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-r--r--   0        0        0       36 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-r--r--   0        0        0     3494 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js
--rw-r--r--   0        0        0     7972 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js
--rw-r--r--   0        0        0      817 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-r--r--   0        0        0     6026 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-r--r--   0        0        0     4754 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js
--rw-r--r--   0        0        0    10171 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-r--r--   0        0        0    10958 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-r--r--   0        0        0    10331 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-r--r--   0        0        0     4901 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js
--rw-r--r--   0        0        0     3647 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-r--r--   0        0        0     4523 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-r--r--   0        0        0     2406 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js
--rw-r--r--   0        0        0     2330 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js
--rw-r--r--   0        0        0     1031 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js
--rw-r--r--   0        0        0    15009 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-r--r--   0        0        0      784 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-r--r--   0        0        0     2158 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js
--rw-r--r--   0        0        0    22878 2024-04-03 00:40:54.194903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js
--rw-r--r--   0        0        0   677463 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js
--rw-r--r--   0        0        0    39431 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js
--rw-r--r--   0        0        0   214982 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map
--rw-r--r--   0        0        0     9204 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png
--rw-r--r--   0        0        0    13318 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg
--rw-r--r--   0        0        0     7562 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png
--rw-r--r--   0        0        0      846 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html
--rw-r--r--   0        0        0   122377 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css
--rw-r--r--   0        0        0    42299 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map
--rw-r--r--   0        0        0    12245 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css
--rw-r--r--   0        0        0     3639 2024-04-03 00:40:54.198902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map
--rw-r--r--   0        0        0    75597 2024-04-03 00:40:54.574903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html
--rw-r--r--   0        0        0   193115 2024-04-03 00:40:54.678903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html
--rw-r--r--   0        0        0    51809 2024-04-03 00:40:54.606903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html
--rw-r--r--   0        0        0   312303 2024-04-03 00:40:54.818903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html
--rw-r--r--   0        0        0    77149 2024-04-03 00:40:54.834903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html
--rw-r--r--   0        0        0    59370 2024-04-03 00:40:54.578903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html
--rw-r--r--   0        0        0   114762 2024-04-03 00:40:54.598903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html
--rw-r--r--   0        0        0    51997 2024-04-03 00:40:54.602903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html
--rw-r--r--   0        0        0    75903 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png
--rw-r--r--   0        0        0   165191 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png
--rw-r--r--   0        0        0   276244 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png
--rw-r--r--   0        0        0    82969 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png
--rw-r--r--   0        0        0    67457 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png
--rw-r--r--   0        0        0    59437 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png
--rw-r--r--   0        0        0   157371 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png
--rw-r--r--   0        0        0   108592 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png
--rw-r--r--   0        0        0   116460 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png
--rw-r--r--   0        0        0   155101 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png
--rw-r--r--   0        0        0    59126 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png
--rw-r--r--   0        0        0    69205 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png
--rw-r--r--   0        0        0   204762 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png
--rw-r--r--   0        0        0    44937 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png
--rw-r--r--   0        0        0    89739 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png
--rw-r--r--   0        0        0   175928 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png
--rw-r--r--   0        0        0   128918 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png
--rw-r--r--   0        0        0    34712 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png
--rw-r--r--   0        0        0   155103 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png
--rw-r--r--   0        0        0    67662 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png
--rw-r--r--   0        0        0    34084 2024-04-03 00:40:54.182902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png
--rw-r--r--   0        0        0    64803 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png
--rw-r--r--   0        0        0    50317 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png
--rw-r--r--   0        0        0    78058 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png
--rw-r--r--   0        0        0    35263 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png
--rw-r--r--   0        0        0     5689 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png
--rw-r--r--   0        0        0   174561 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png
--rw-r--r--   0        0        0   259361 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png
--rw-r--r--   0        0        0   496898 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png
--rw-r--r--   0        0        0    56418 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png
--rw-r--r--   0        0        0   256279 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png
--rw-r--r--   0        0        0    50350 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png
--rw-r--r--   0        0        0   119945 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png
--rw-r--r--   0        0        0    81496 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png
--rw-r--r--   0        0        0   114519 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png
--rw-r--r--   0        0        0   383810 2024-04-03 00:40:54.186902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png
--rw-r--r--   0        0        0   340453 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png
--rw-r--r--   0        0        0   448190 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png
--rw-r--r--   0        0        0    83466 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png
--rw-r--r--   0        0        0   122430 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png
--rw-r--r--   0        0        0   244962 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png
--rw-r--r--   0        0        0   105992 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png
--rw-r--r--   0        0        0   156622 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png
--rw-r--r--   0        0        0   172988 2024-04-03 00:40:54.190902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png
--rw-r--r--   0        0        0    62138 2024-04-03 00:40:54.354903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/index.html
--rw-r--r--   0        0        0      858 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv
--rw-r--r--   0        0        0      119 2024-04-03 00:40:54.178902 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/requirements.txt
--rw-r--r--   0        0        0   314253 2024-04-03 00:40:54.962904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json
--rw-r--r--   0        0        0    15738 2024-04-03 00:40:54.334903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml
--rw-r--r--   0        0        0      701 2024-04-03 00:40:54.334903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml.gz
--rw-r--r--   0        0        0    63597 2024-04-03 00:40:54.842903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html
--rw-r--r--   0        0        0    64154 2024-04-03 00:40:54.846903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html
--rw-r--r--   0        0        0    58507 2024-04-03 00:40:54.850903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html
--rw-r--r--   0        0        0    75487 2024-04-03 00:40:54.862903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html
--rw-r--r--   0        0        0    55453 2024-04-03 00:40:54.866903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html
--rw-r--r--   0        0        0    59499 2024-04-03 00:40:54.874903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html
--rw-r--r--   0        0        0    65717 2024-04-03 00:40:54.878903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html
--rw-r--r--   0        0        0    69780 2024-04-03 00:40:54.886903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html
--rw-r--r--   0        0        0    60732 2024-04-03 00:40:54.890903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html
--rw-r--r--   0        0        0    68945 2024-04-03 00:40:54.898903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html
--rw-r--r--   0        0        0    87551 2024-04-03 00:40:54.914903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html
--rw-r--r--   0        0        0    57419 2024-04-03 00:40:54.922903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html
--rw-r--r--   0        0        0    79335 2024-04-03 00:40:54.930904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html
--rw-r--r--   0        0        0    54161 2024-04-03 00:40:54.934903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html
--rw-r--r--   0        0        0    79432 2024-04-03 00:40:54.942903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html
--rw-r--r--   0        0        0    61399 2024-04-03 00:40:54.950904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html
--rw-r--r--   0        0        0    56432 2024-04-03 00:40:54.954903 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html
--rw-r--r--   0        0        0    60266 2024-04-03 00:40:54.962904 nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html
--rw-r--r--   0        0        0     9375 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/run_job.js
--rw-r--r--   0        0        0     3426 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/static/toggle_fields.js
--rw-r--r--   0        0        0    19310 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/tables.py
--rw-r--r--   0        0        0     5390 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/template_content.py
--rw-r--r--   0        0        0     1123 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
--rw-r--r--   0        0        0     1429 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
--rw-r--r--   0        0        0     8122 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html
--rw-r--r--   0        0        0      607 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html
--rw-r--r--   0        0        0     3931 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html
--rw-r--r--   0        0        0     3607 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html
--rw-r--r--   0        0        0     4268 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html
--rw-r--r--   0        0        0     1861 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html
--rw-r--r--   0        0        0     3251 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html
--rw-r--r--   0        0        0      442 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_update.html
--rw-r--r--   0        0        0      964 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
--rw-r--r--   0        0        0      965 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
--rw-r--r--   0        0        0     4560 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
--rw-r--r--   0        0        0      150 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_details.html
--rw-r--r--   0        0        0     2597 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html
--rw-r--r--   0        0        0     3081 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
--rw-r--r--   0        0        0     2382 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html
--rw-r--r--   0        0        0     3681 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
--rw-r--r--   0        0        0     1393 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
--rw-r--r--   0        0        0      254 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/include/span_button.html
--rw-r--r--   0        0        0     1553 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html
--rw-r--r--   0        0        0      773 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html
--rw-r--r--   0        0        0       35 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templatetags/__init__.py
--rw-r--r--   0        0        0      451 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/templatetags/json_helpers.py
--rw-r--r--   0        0        0       49 2024-04-03 00:39:45.494810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/__init__.py
--rw-r--r--   0        0        0    20312 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/conftest.py
--rw-r--r--   0        0        0       51 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/__init__.py
--rw-r--r--   0        0        0     3216 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/test_golden_config_settings.py
--rw-r--r--   0        0        0       83 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/jinja_filters.py
--rw-r--r--   0        0        0    16589 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_api.py
--rw-r--r--   0        0        0     1041 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_basic.py
--rw-r--r--   0        0        0     3624 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_datasources.py
--rw-r--r--   0        0        0    24891 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_filters.py
--rw-r--r--   0        0        0    12988 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_graphql.py
--rw-r--r--   0        0        0     5519 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_helpers.py
--rwxr-xr-x   0        0        0    33953 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_jobs.py
--rw-r--r--   0        0        0    18996 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_models.py
--rw-r--r--   0        0        0       58 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/__init__.py
--rw-r--r--   0        0        0     2582 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
--rw-r--r--   0        0        0       55 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/__init__.py
--rw-r--r--   0        0        0     2588 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_config_plan.py
--rw-r--r--   0        0        0     3392 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_git.py
--rw-r--r--   0        0        0     1211 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_graphql.py
--rw-r--r--   0        0        0    15315 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_helpers.py
--rw-r--r--   0        0        0    15351 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_views.py
--rw-r--r--   0        0        0     1134 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/urls.py
--rw-r--r--   0        0        0       17 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_plan.py
--rw-r--r--   0        0        0     8845 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_postprocessing.py
--rw-r--r--   0        0        0     1106 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/constant.py
--rw-r--r--   0        0        0      607 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/db_management.py
--rw-r--r--   0        0        0     1271 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/git.py
--rw-r--r--   0        0        0     1773 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/graphql.py
--rw-r--r--   0        0        0     9375 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/helper.py
--rw-r--r--   0        0        0     1811 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/logger.py
--rw-r--r--   0        0        0     4981 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/mat_plot.py
--rw-r--r--   0        0        0     2081 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/utils.py
--rw-r--r--   0        0        0    25070 2024-04-03 00:39:45.498810 nautobot_golden_config-2.0.4/nautobot_golden_config/views.py
--rw-r--r--   0        0        0     6159 2024-04-03 00:39:54.750823 nautobot_golden_config-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 nautobot_golden_config-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      591 2024-05-23 18:10:43.391990 nautobot_golden_config-2.0.5/LICENSE
+-rw-r--r--   0        0        0     7047 2024-05-23 18:10:43.391990 nautobot_golden_config-2.0.5/README.md
+-rw-r--r--   0        0        0     3415 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/api/__init__.py
+-rw-r--r--   0        0        0     4023 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/api/serializers.py
+-rw-r--r--   0        0        0     1071 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/api/urls.py
+-rw-r--r--   0        0        0     6468 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/api/views.py
+-rw-r--r--   0        0        0        5 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/app-config-schema.json
+-rw-r--r--   0        0        0      950 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/choices.py
+-rw-r--r--   0        0        0     9452 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/datasources.py
+-rw-r--r--   0        0        0      745 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/exceptions.py
+-rw-r--r--   0        0        0    14555 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/filters.py
+-rw-r--r--   0        0        0    22228 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/forms.py
+-rw-r--r--   0        0        0    25137 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/jobs.py
+-rw-r--r--   0        0        0     4417 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/metrics.py
+-rw-r--r--   0        0        0    12457 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0001_initial.py
+-rw-r--r--   0        0        0      500 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0002_custom_data.py
+-rw-r--r--   0        0        0     1814 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0003_auto_20210510_2356.py
+-rw-r--r--   0        0        0     1824 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0004_auto_20210616_2234.py
+-rw-r--r--   0        0        0     1538 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0005_json_compliance_rule.py
+-rw-r--r--   0        0        0     1794 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py
+-rw-r--r--   0        0        0     2555 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py
+-rw-r--r--   0        0        0      665 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0008_multi_repo_support_final.py
+-rw-r--r--   0        0        0     2558 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py
+-rw-r--r--   0        0        0      929 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py
+-rw-r--r--   0        0        0     1486 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py
+-rw-r--r--   0        0        0      909 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py
+-rw-r--r--   0        0        0      463 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0013_multiple_gc_settings_part_5.py
+-rw-r--r--   0        0        0      429 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0014_convert_sotagg_queries_part1.py
+-rw-r--r--   0        0        0      697 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py
+-rw-r--r--   0        0        0      742 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py
+-rw-r--r--   0        0        0     1594 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py
+-rw-r--r--   0        0        0      327 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0018_convert_sotagg_queries_part5.py
+-rw-r--r--   0        0        0      678 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py
+-rw-r--r--   0        0        0     1113 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py
+-rw-r--r--   0        0        0      663 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py
+-rw-r--r--   0        0        0      389 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0022_alter_configcompliance_options.py
+-rw-r--r--   0        0        0      433 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0023_alter_custom_compliance.py
+-rw-r--r--   0        0        0      936 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py
+-rw-r--r--   0        0        0     2427 2024-05-23 18:10:43.427990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0025_remediation_settings.py
+-rw-r--r--   0        0        0     2925 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0026_configplan.py
+-rw-r--r--   0        0        0     1243 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0027_auto_20230915_1657.py
+-rw-r--r--   0        0        0     1332 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py
+-rw-r--r--   0        0        0     7687 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py
+-rw-r--r--   0        0        0      469 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0029_alter_configplan_unique_together.py
+-rw-r--r--   0        0        0      581 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py
+-rw-r--r--   0        0        0        0 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/__init__.py
+-rw-r--r--   0        0        0    28162 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/models.py
+-rw-r--r--   0        0        0     4837 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/navigation.py
+-rw-r--r--   0        0        0       51 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/__init__.py
+-rw-r--r--   0        0        0     6574 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_backup.py
+-rw-r--r--   0        0        0     9174 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_compliance.py
+-rw-r--r--   0        0        0     5626 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_deployment.py
+-rw-r--r--   0        0        0     6132 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_intended.py
+-rw-r--r--   0        0        0     2373 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/processor.py
+-rwxr-xr-x   0        0        0     3430 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/signals.py
+-rw-r--r--   0        0        0     5157 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css
+-rw-r--r--   0        0        0    67022 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js
+-rw-r--r--   0        0        0    51068 2024-05-23 18:11:24.587904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/404.html
+-rw-r--r--   0        0        0    53070 2024-05-23 18:11:24.615904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html
+-rw-r--r--   0        0        0    72938 2024-05-23 18:11:24.623904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html
+-rw-r--r--   0        0        0    75234 2024-05-23 18:11:24.635904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html
+-rw-r--r--   0        0        0    51442 2024-05-23 18:11:24.647904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html
+-rw-r--r--   0        0        0    53317 2024-05-23 18:11:24.651904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html
+-rw-r--r--   0        0        0    67535 2024-05-23 18:11:24.655904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html
+-rw-r--r--   0        0        0    61279 2024-05-23 18:11:24.663904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html
+-rw-r--r--   0        0        0    58323 2024-05-23 18:11:24.667904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html
+-rw-r--r--   0        0        0    66552 2024-05-23 18:11:24.671904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html
+-rw-r--r--   0        0        0    55655 2024-05-23 18:11:24.675904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html
+-rw-r--r--   0        0        0    60872 2024-05-23 18:11:24.683904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html
+-rw-r--r--   0        0        0    55522 2024-05-23 18:11:24.687904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html
+-rw-r--r--   0        0        0    60059 2024-05-23 18:11:24.691904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html
+-rw-r--r--   0        0        0    69872 2024-05-23 18:11:24.695904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html
+-rw-r--r--   0        0        0    53504 2024-05-23 18:11:24.703904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.707904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.711904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.715904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.719904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.723904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.727904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.731904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.735904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.739904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.743904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.747904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.751904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.755904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.759904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.763903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.767904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.771904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.771904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.775904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.779904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.783903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.787904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.791904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html
+-rw-r--r--   0        0        0    53466 2024-05-23 18:11:24.795904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html
+-rw-r--r--   0        0        0    53512 2024-05-23 18:11:24.799903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html
+-rw-r--r--   0        0        0    50870 2024-05-23 18:11:24.803903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3027.html
+-rw-r--r--   0        0        0    50878 2024-05-23 18:11:24.807903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3028.html
+-rw-r--r--   0        0        0    50875 2024-05-23 18:11:24.807903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3029.html
+-rw-r--r--   0        0        0    50870 2024-05-23 18:11:24.811904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3030.html
+-rw-r--r--   0        0        0    52256 2024-05-23 18:11:24.699904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html
+-rw-r--r--   0        0        0    54288 2024-05-23 18:11:24.639904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html
+-rw-r--r--   0        0        0    53811 2024-05-23 18:11:24.643904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html
+-rw-r--r--   0        0        0     1000 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     5135 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css
+-rw-r--r--   0        0        0    15086 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico
+-rw-r--r--   0        0        0     1870 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png
+-rw-r--r--   0        0        0    97321 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js
+-rw-r--r--   0        0        0   891518 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map
+-rw-r--r--   0        0        0    17074 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     6882 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js
+-rw-r--r--   0        0        0     3383 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    22878 2024-05-23 18:11:24.455904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    39431 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js
+-rw-r--r--   0        0        0   214982 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map
+-rw-r--r--   0        0        0     9204 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png
+-rw-r--r--   0        0        0    13318 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg
+-rw-r--r--   0        0        0     7562 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png
+-rw-r--r--   0        0        0      846 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html
+-rw-r--r--   0        0        0   122377 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css
+-rw-r--r--   0        0        0    42299 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map
+-rw-r--r--   0        0        0    12245 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css
+-rw-r--r--   0        0        0     3639 2024-05-23 18:11:24.459904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map
+-rw-r--r--   0        0        0    75597 2024-05-23 18:11:24.823903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html
+-rw-r--r--   0        0        0   193115 2024-05-23 18:11:24.927903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html
+-rw-r--r--   0        0        0    51809 2024-05-23 18:11:24.855903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html
+-rw-r--r--   0        0        0   312303 2024-05-23 18:11:25.063903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html
+-rw-r--r--   0        0        0    77149 2024-05-23 18:11:25.079903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html
+-rw-r--r--   0        0        0    59370 2024-05-23 18:11:24.827903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html
+-rw-r--r--   0        0        0   114762 2024-05-23 18:11:24.847903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html
+-rw-r--r--   0        0        0    51997 2024-05-23 18:11:24.851903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html
+-rw-r--r--   0        0        0    75903 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png
+-rw-r--r--   0        0        0   165191 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png
+-rw-r--r--   0        0        0   276244 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png
+-rw-r--r--   0        0        0    82969 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png
+-rw-r--r--   0        0        0    67457 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png
+-rw-r--r--   0        0        0    59437 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png
+-rw-r--r--   0        0        0   157371 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png
+-rw-r--r--   0        0        0   108592 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png
+-rw-r--r--   0        0        0   116460 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png
+-rw-r--r--   0        0        0   155101 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png
+-rw-r--r--   0        0        0    59126 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png
+-rw-r--r--   0        0        0    69205 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png
+-rw-r--r--   0        0        0   204762 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png
+-rw-r--r--   0        0        0    44937 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png
+-rw-r--r--   0        0        0    89739 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png
+-rw-r--r--   0        0        0   175928 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png
+-rw-r--r--   0        0        0   128918 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png
+-rw-r--r--   0        0        0    34712 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png
+-rw-r--r--   0        0        0   155103 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png
+-rw-r--r--   0        0        0    67662 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png
+-rw-r--r--   0        0        0    34084 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png
+-rw-r--r--   0        0        0    64803 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png
+-rw-r--r--   0        0        0    50317 2024-05-23 18:11:24.443904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png
+-rw-r--r--   0        0        0    78058 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png
+-rw-r--r--   0        0        0    35263 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png
+-rw-r--r--   0        0        0     5689 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png
+-rw-r--r--   0        0        0   174561 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png
+-rw-r--r--   0        0        0   259361 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png
+-rw-r--r--   0        0        0   496898 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png
+-rw-r--r--   0        0        0    56418 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png
+-rw-r--r--   0        0        0   256279 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png
+-rw-r--r--   0        0        0    50350 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png
+-rw-r--r--   0        0        0   119945 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png
+-rw-r--r--   0        0        0    81496 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png
+-rw-r--r--   0        0        0   114519 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png
+-rw-r--r--   0        0        0   383810 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png
+-rw-r--r--   0        0        0   340453 2024-05-23 18:11:24.447904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png
+-rw-r--r--   0        0        0   448190 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png
+-rw-r--r--   0        0        0    83466 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png
+-rw-r--r--   0        0        0   122430 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png
+-rw-r--r--   0        0        0   244962 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png
+-rw-r--r--   0        0        0   105992 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png
+-rw-r--r--   0        0        0   156622 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png
+-rw-r--r--   0        0        0   172988 2024-05-23 18:11:24.451904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png
+-rw-r--r--   0        0        0    62138 2024-05-23 18:11:24.611904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/index.html
+-rw-r--r--   0        0        0      858 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv
+-rw-r--r--   0        0        0      119 2024-05-23 18:11:24.439904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/requirements.txt
+-rw-r--r--   0        0        0   314552 2024-05-23 18:11:25.199903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json
+-rw-r--r--   0        0        0    15738 2024-05-23 18:11:24.463904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml
+-rw-r--r--   0        0        0      702 2024-05-23 18:11:24.463904 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml.gz
+-rw-r--r--   0        0        0    63597 2024-05-23 18:11:25.087903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html
+-rw-r--r--   0        0        0    64154 2024-05-23 18:11:25.091903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html
+-rw-r--r--   0        0        0    58507 2024-05-23 18:11:25.095903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html
+-rw-r--r--   0        0        0    75487 2024-05-23 18:11:25.107903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html
+-rw-r--r--   0        0        0    55453 2024-05-23 18:11:25.111903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html
+-rw-r--r--   0        0        0    59499 2024-05-23 18:11:25.115903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html
+-rw-r--r--   0        0        0    65717 2024-05-23 18:11:25.123903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html
+-rw-r--r--   0        0        0    69780 2024-05-23 18:11:25.127903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html
+-rw-r--r--   0        0        0    60732 2024-05-23 18:11:25.135903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html
+-rw-r--r--   0        0        0    68945 2024-05-23 18:11:25.139903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html
+-rw-r--r--   0        0        0    87551 2024-05-23 18:11:25.155903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html
+-rw-r--r--   0        0        0    57419 2024-05-23 18:11:25.159903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html
+-rw-r--r--   0        0        0    79335 2024-05-23 18:11:25.171903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html
+-rw-r--r--   0        0        0    54161 2024-05-23 18:11:25.171903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html
+-rw-r--r--   0        0        0    79432 2024-05-23 18:11:25.183903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html
+-rw-r--r--   0        0        0    61399 2024-05-23 18:11:25.187903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html
+-rw-r--r--   0        0        0    56432 2024-05-23 18:11:25.191903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html
+-rw-r--r--   0        0        0    60266 2024-05-23 18:11:25.199903 nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html
+-rw-r--r--   0        0        0     9375 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/static/run_job.js
+-rw-r--r--   0        0        0     3426 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/static/toggle_fields.js
+-rw-r--r--   0        0        0    19310 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tables.py
+-rw-r--r--   0        0        0     5390 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/template_content.py
+-rw-r--r--   0        0        0     1123 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html
+-rw-r--r--   0        0        0     1429 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html
+-rw-r--r--   0        0        0     8122 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html
+-rw-r--r--   0        0        0      607 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html
+-rw-r--r--   0        0        0     3931 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html
+-rw-r--r--   0        0        0     3607 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html
+-rw-r--r--   0        0        0     4268 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html
+-rw-r--r--   0        0        0     1861 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html
+-rw-r--r--   0        0        0     3251 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html
+-rw-r--r--   0        0        0      442 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_update.html
+-rw-r--r--   0        0        0      964 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html
+-rw-r--r--   0        0        0      965 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html
+-rw-r--r--   0        0        0     4560 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/content_template.html
+-rw-r--r--   0        0        0      150 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_details.html
+-rw-r--r--   0        0        0     2597 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html
+-rw-r--r--   0        0        0     3081 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html
+-rw-r--r--   0        0        0     2382 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html
+-rw-r--r--   0        0        0     3681 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html
+-rw-r--r--   0        0        0     1393 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html
+-rw-r--r--   0        0        0      254 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/include/span_button.html
+-rw-r--r--   0        0        0     1553 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html
+-rw-r--r--   0        0        0      773 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html
+-rw-r--r--   0        0        0       35 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templatetags/__init__.py
+-rw-r--r--   0        0        0      451 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/templatetags/json_helpers.py
+-rw-r--r--   0        0        0       49 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/__init__.py
+-rw-r--r--   0        0        0    20312 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/conftest.py
+-rw-r--r--   0        0        0       51 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/forms/__init__.py
+-rw-r--r--   0        0        0     3216 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/forms/test_golden_config_settings.py
+-rw-r--r--   0        0        0       83 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/jinja_filters.py
+-rw-r--r--   0        0        0    16589 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_api.py
+-rw-r--r--   0        0        0     1041 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_basic.py
+-rw-r--r--   0        0        0     3624 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_datasources.py
+-rw-r--r--   0        0        0    24891 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_filters.py
+-rw-r--r--   0        0        0    12988 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_graphql.py
+-rw-r--r--   0        0        0     5519 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_helpers.py
+-rwxr-xr-x   0        0        0    33953 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_jobs.py
+-rw-r--r--   0        0        0    18996 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_models.py
+-rw-r--r--   0        0        0       58 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_nornir_plays/__init__.py
+-rw-r--r--   0        0        0     2582 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py
+-rw-r--r--   0        0        0       55 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/__init__.py
+-rw-r--r--   0        0        0     2588 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_config_plan.py
+-rw-r--r--   0        0        0     3392 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_git.py
+-rw-r--r--   0        0        0     1211 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_graphql.py
+-rw-r--r--   0        0        0    15315 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_helpers.py
+-rw-r--r--   0        0        0    15351 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_views.py
+-rw-r--r--   0        0        0     1134 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/urls.py
+-rw-r--r--   0        0        0       17 2024-05-23 18:10:43.431990 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/config_plan.py
+-rw-r--r--   0        0        0     8845 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/config_postprocessing.py
+-rw-r--r--   0        0        0     1106 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/constant.py
+-rw-r--r--   0        0        0      607 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/db_management.py
+-rw-r--r--   0        0        0     1271 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/git.py
+-rw-r--r--   0        0        0     1773 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/graphql.py
+-rw-r--r--   0        0        0     9375 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/helper.py
+-rw-r--r--   0        0        0     1811 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/logger.py
+-rw-r--r--   0        0        0     4981 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/mat_plot.py
+-rw-r--r--   0        0        0     2081 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/utils.py
+-rw-r--r--   0        0        0    25070 2024-05-23 18:10:43.435989 nautobot_golden_config-2.0.5/nautobot_golden_config/views.py
+-rw-r--r--   0        0        0     6159 2024-05-23 18:10:56.523965 nautobot_golden_config-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8596 1970-01-01 00:00:00.000000 nautobot_golden_config-2.0.5/PKG-INFO
```

### Comparing `nautobot_golden_config-2.0.4/LICENSE` & `nautobot_golden_config-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/README.md` & `nautobot_golden_config-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/__init__.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/__init__.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/api/serializers.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/api/serializers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/api/urls.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/api/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/api/views.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/api/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/choices.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/choices.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/datasources.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/exceptions.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/exceptions.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/filters.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/forms.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/forms.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/jobs.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
         List[GitRepo]: List of GitRepos to be used with Job(s).
     """
     job.logger.debug("Compiling device data for GC job.", extra={"grouping": "Get Job Filter"})
     job.qs = get_job_filter(data)
     job.logger.debug(f"In scope device count for this job: {job.qs.count()}", extra={"grouping": "Get Job Filter"})
     job.logger.debug("Mapping device(s) to GC Settings.", extra={"grouping": "Device to Settings Map"})
     job.device_to_settings_map = get_device_to_settings_map(queryset=job.qs)
-    gitrepo_types = list(set(get_repo_types_for_job(job.name)))
+    gitrepo_types = list(set(get_repo_types_for_job(job.class_path)))
     job.logger.debug(
         f"Repository types to sync: {', '.join(sorted(gitrepo_types))}",
         extra={"grouping": "GC Repo Syncs"},
     )
     current_repos = get_refreshed_repos(job_obj=job, repo_types=gitrepo_types, data=job.qs)
     return current_repos
```

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/metrics.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/metrics.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0001_initial.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0003_auto_20210510_2356.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0003_auto_20210510_2356.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0004_auto_20210616_2234.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0004_auto_20210616_2234.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0005_json_compliance_rule.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0005_json_compliance_rule.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0006_multi_repo_support_temp_field.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0007_multi_repo_support_convert_many.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0008_multi_repo_support_final.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0008_multi_repo_support_final.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0009_multiple_gc_settings_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0010_multiple_gc_settings_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0011_multiple_gc_settings_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0012_multiple_gc_settings_part_4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0015_convert_sotagg_queries_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0016_convert_sotagg_queries_part3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0017_convert_sotagg_queries_part4.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0019_convert_dynamicgroup_part_1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0020_convert_dynamicgroup_part_2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0021_convert_dynamicgroup_part_3.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0024_convert_custom_compliance_rules.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0025_remediation_settings.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0025_remediation_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0026_configplan.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0026_configplan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0027_auto_20230915_1657.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0027_auto_20230915_1657.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0028_auto_20230916_1712_part1.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0028_auto_20230916_1712_part2.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/migrations/0030_alter_goldenconfig_device.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/models.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/navigation.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/navigation.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_backup.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_backup.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_compliance.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_deployment.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_deployment.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/config_intended.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/config_intended.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/nornir_plays/processor.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/nornir_plays/processor.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/signals.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/signals.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/diff2html-3.4.43/diff2html.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/404.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/404.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/compatibility_matrix.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/install.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/migrating_to_v2.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.10.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_0.9.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.0.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.1.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.2.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.3.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.4.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.5.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_1.6.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/release_notes/version_2.0.html`

 * *Files 1% similar despite different names*

```diff
@@ -1768,23 +1768,43 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
+  <a href="#v205-2024-05" class="md-nav__link">
+    v2.0.5 2024-05
+  </a>
+  
+    <nav class="md-nav" aria-label="v2.0.5 2024-05">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#fixed" class="md-nav__link">
+    Fixed
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
   <a href="#v204-2024-04" class="md-nav__link">
     v2.0.4 2024-04
   </a>
   
     <nav class="md-nav" aria-label="v2.0.4 2024-04">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed" class="md-nav__link">
+  <a href="#fixed_1" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#housekeeping" class="md-nav__link">
@@ -1810,15 +1830,15 @@
   <a href="#added" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_1" class="md-nav__link">
+  <a href="#fixed_2" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
       </ul>
     </nav>
@@ -1837,15 +1857,15 @@
   <a href="#added_1" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_2" class="md-nav__link">
+  <a href="#fixed_3" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed" class="md-nav__link">
@@ -1864,15 +1884,15 @@
     v2.0.1 - 2023-12
   </a>
   
     <nav class="md-nav" aria-label="v2.0.1 - 2023-12">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed_3" class="md-nav__link">
+  <a href="#fixed_4" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed_1" class="md-nav__link">
@@ -2423,23 +2443,43 @@
     <label class="md-nav__title" for="__toc">
       <span class="md-nav__icon md-icon"></span>
       Table of contents
     </label>
     <ul class="md-nav__list" data-md-component="toc" data-md-scrollfix>
       
         <li class="md-nav__item">
+  <a href="#v205-2024-05" class="md-nav__link">
+    v2.0.5 2024-05
+  </a>
+  
+    <nav class="md-nav" aria-label="v2.0.5 2024-05">
+      <ul class="md-nav__list">
+        
+          <li class="md-nav__item">
+  <a href="#fixed" class="md-nav__link">
+    Fixed
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
   <a href="#v204-2024-04" class="md-nav__link">
     v2.0.4 2024-04
   </a>
   
     <nav class="md-nav" aria-label="v2.0.4 2024-04">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed" class="md-nav__link">
+  <a href="#fixed_1" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#housekeeping" class="md-nav__link">
@@ -2465,15 +2505,15 @@
   <a href="#added" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_1" class="md-nav__link">
+  <a href="#fixed_2" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
       </ul>
     </nav>
@@ -2492,15 +2532,15 @@
   <a href="#added_1" class="md-nav__link">
     Added
   </a>
   
 </li>
         
           <li class="md-nav__item">
-  <a href="#fixed_2" class="md-nav__link">
+  <a href="#fixed_3" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed" class="md-nav__link">
@@ -2519,15 +2559,15 @@
     v2.0.1 - 2023-12
   </a>
   
     <nav class="md-nav" aria-label="v2.0.1 - 2023-12">
       <ul class="md-nav__list">
         
           <li class="md-nav__item">
-  <a href="#fixed_3" class="md-nav__link">
+  <a href="#fixed_4" class="md-nav__link">
     Fixed
   </a>
   
 </li>
         
           <li class="md-nav__item">
   <a href="#changed_1" class="md-nav__link">
@@ -2616,39 +2656,44 @@
 <li>Moved config compliance view to be a tab within device instead of a dedicated page.</li>
 <li>Removed management command in favor of Nautobot Core's.</li>
 </ul>
 <div class="admonition note">
 <p class="admonition-title">Note</p>
 <p>Please see <a href="../migrating_to_v2.html">migrating guide</a> for details on migration.</p>
 </div>
-<h2 id="v204-2024-04">v2.0.4 2024-04<a class="headerlink" href="#v204-2024-04" title="Permanent link">&para;</a></h2>
+<h2 id="v205-2024-05">v2.0.5 2024-05<a class="headerlink" href="#v205-2024-05" title="Permanent link">&para;</a></h2>
 <h3 id="fixed">Fixed<a class="headerlink" href="#fixed" title="Permanent link">&para;</a></h3>
 <ul>
+<li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/749">#759</a> - Fix issue with Git Repo not syncing by changing to explicitly use class_path property.</li>
+</ul>
+<h2 id="v204-2024-04">v2.0.4 2024-04<a class="headerlink" href="#v204-2024-04" title="Permanent link">&para;</a></h2>
+<h3 id="fixed_1">Fixed<a class="headerlink" href="#fixed_1" title="Permanent link">&para;</a></h3>
+<ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/749">#749</a> - Corrected issue where consecutive Golden Config Jobs in All Golden Configs Job wouldn't execute if prior Job had an Exception raised.</li>
 </ul>
 <h3 id="housekeeping">Housekeeping<a class="headerlink" href="#housekeeping" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/741">#741</a> - Re-baked from the latest template.</li>
 </ul>
 <h2 id="v203-2024-03">v2.0.3 2024-03<a class="headerlink" href="#v203-2024-03" title="Permanent link">&para;</a></h2>
 <h3 id="added">Added<a class="headerlink" href="#added" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/736">#736</a> - Add a boolean job parameter <code>fail_job_on_task_failure</code> which will determine whether a single task failure anywhere in the job-result should result in job-result status of failed vs successful.</li>
 </ul>
-<h3 id="fixed_1">Fixed<a class="headerlink" href="#fixed_1" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_2">Fixed<a class="headerlink" href="#fixed_2" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/issues/736">#736</a> - Fixes repo push and commit not executing if a exception was raised on any task inside a job.</li>
 </ul>
 <h2 id="v202-2024-03">v2.0.2 - 2024-03<a class="headerlink" href="#v202-2024-03" title="Permanent link">&para;</a></h2>
 <h3 id="added_1">Added<a class="headerlink" href="#added_1" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Added autoformat invoke command.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/730">#730</a> - Added app config schema generator and validator.</li>
 </ul>
-<h3 id="fixed_2">Fixed<a class="headerlink" href="#fixed_2" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_3">Fixed<a class="headerlink" href="#fixed_3" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/699">#699</a> - Fixed stale reference to platform_slug_map.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/719">#719</a> - Fixed generate config plans Status filter.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/715">#715</a> - Fixed close threaded db connections during config deployment.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/726">#726</a> - Fixed objectchange log excludes for object_data_v2 data as well.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/718">#718</a> - Fixed logic to handle jobs requiring approvals.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/724">#724</a> - Fixed performance issue on UNIX file diff view.</li>
@@ -2659,15 +2704,15 @@
 <h3 id="changed">Changed<a class="headerlink" href="#changed" title="Permanent link">&para;</a></h3>
 <ul>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/691">#691</a> - Changed repo name and references to nautobot-app-golden-config.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Changed from pydocstyle to ruff.</li>
 <li><a href="https://github.com/nautobot/nautobot-app-golden-config/pull/707">#707</a> - Changed release notes to towncrier based.</li>
 </ul>
 <h2 id="v201-2023-12">v2.0.1 - 2023-12<a class="headerlink" href="#v201-2023-12" title="Permanent link">&para;</a></h2>
-<h3 id="fixed_3">Fixed<a class="headerlink" href="#fixed_3" title="Permanent link">&para;</a></h3>
+<h3 id="fixed_4">Fixed<a class="headerlink" href="#fixed_4" title="Permanent link">&para;</a></h3>
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
@@ -70,14 +70,16 @@
                 # _E_3_0_2_5
                 # _E_3_0_2_6
           o _M_i_g_r_a_t_i_n_g_ _T_o_ _v_2
           o 
             _R_e_l_e_a_s_e_ _N_o_t_e_s
             Release Notes
                 # ??v2.0 _v_2_._0_ Table of contents
+                      # _v_2_._0_._5_ _2_0_2_4_-_0_5
+                            # _F_i_x_e_d
                       # _v_2_._0_._4_ _2_0_2_4_-_0_4
                             # _F_i_x_e_d
                             # _H_o_u_s_e_k_e_e_p_i_n_g
                       # _v_2_._0_._3_ _2_0_2_4_-_0_3
                             # _A_d_d_e_d
                             # _F_i_x_e_d
                       # _v_2_._0_._2_ _-_ _2_0_2_4_-_0_3
@@ -109,14 +111,16 @@
             _C_o_d_e_ _R_e_f_e_r_e_n_c_e
             Code Reference
                 # _M_o_d_e_l_s
                 # _P_a_c_k_a_g_e
                 # _A_P_I
     * _N_a_u_t_o_b_o_t_ _D_o_c_s_ _H_o_m_e_ _↗_︎
 Table of contents
+    * _v_2_._0_._5_ _2_0_2_4_-_0_5
+          o _F_i_x_e_d
     * _v_2_._0_._4_ _2_0_2_4_-_0_4
           o _F_i_x_e_d
           o _H_o_u_s_e_k_e_e_p_i_n_g
     * _v_2_._0_._3_ _2_0_2_4_-_0_3
           o _A_d_d_e_d
           o _F_i_x_e_d
     * _v_2_._0_._2_ _-_ _2_0_2_4_-_0_3
@@ -140,14 +144,18 @@
       MERGE_CONFIG_FRAMEWORK, and REPLACE_CONFIG_FRAMEWORK) and
       customer_dispatcher to remove dispatcher_mapping.
     * Moved config compliance view to be a tab within device instead of a
       dedicated page.
     * Removed management command in favor of Nautobot Core's.
 Note
 Please see _m_i_g_r_a_t_i_n_g_ _g_u_i_d_e for details on migration.
+********** vv22..00..55 22002244--0055_?¶ **********
+******** FFiixxeedd_?¶ ********
+    * _#_7_5_9 - Fix issue with Git Repo not syncing by changing to explicitly use
+      class_path property.
 ********** vv22..00..44 22002244--0044_?¶ **********
 ******** FFiixxeedd_?¶ ********
     * _#_7_4_9 - Corrected issue where consecutive Golden Config Jobs in All Golden
       Configs Job wouldn't execute if prior Job had an Exception raised.
 ******** HHoouusseekkeeeeppiinngg_?¶ ********
     * _#_7_4_1 - Re-baked from the latest template.
 ********** vv22..00..33 22002244--0033_?¶ **********
```

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3001.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3002.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3003.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3004.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3005.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3006.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3007.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3008.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3009.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3010.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3011.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3012.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3013.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3014.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3015.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3016.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3017.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3018.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3019.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3020.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3021.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3022.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3023.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3024.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3025.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3026.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3027.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3027.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3028.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3028.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3029.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3029.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3030.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/E3030.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/troubleshooting/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/uninstall.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/admin/upgrade.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/_mkdocstrings.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/extra.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/bundle.78eede0e.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.he.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.hy.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.kn.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ko.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sa.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.ta.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.te.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.th.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/min/lunr.zh.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/lunr/wordcut.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/javascripts/workers/search.dfff1995.min.js.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/nautobot_logo.svg`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/networktocode_bw.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/overrides/partials/copyright.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/main.0e669242.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/assets/stylesheets/palette.85d0ee34.min.css.map`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/arch_decision.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/api.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/models.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/code_reference/package.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/contributing.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/dev_environment.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/dev/extending.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-backup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/00-troubleshooting.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-backup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/01-troubleshooting.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/02-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/03-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/04-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/05-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/06-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/07-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/08-navigating-compliance-json.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/backup-git-step3.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-detail.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/compliance-rule-edit.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-edit.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-filters.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-manual.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-generate-missing.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_plan-view.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/config_postprocessing_1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/device-compliance.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/git-step1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/icon-NautobotGoldenConfig.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/intended-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/job-result.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/navigate-compliance-rules.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_custom_function_setup.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_enable_compliance_rule_feature.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_hier_edit_options.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_settings_per_platform.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/remediation_validate_feature.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step1.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/secret-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/setting-dynamic-group.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-device.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-report.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_compliance-rule.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/ss_golden-overview.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/images/templates-git-step2.png`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/index.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/index.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/objects.inv`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/search/search_index.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9988545246277205%*

 * *Differences: {"'docs'": "{133: {'location': 'admin/release_notes/version_2.0.html#fixed_1'}, 137: {'location': "*

 * *           "'admin/release_notes/version_2.0.html#fixed_2'}, 140: {'location': "*

 * *           "'admin/release_notes/version_2.0.html#fixed_3'}, 143: {'location': "*

 * *           "'admin/release_notes/version_2.0.html#fixed_4'}, insert: [(130, "*

 * *           "OrderedDict([('location', 'admin/release_notes/version_2.0.html#v205-2024-05'), "*

 * *           "('title', 'v2.0.5 2024-05'), ('text', '')])), (131, OrderedDict([( […]*

```diff
@@ -656,20 +656,30 @@
         },
         {
             "location": "admin/release_notes/version_2.0.html",
             "text": "<ul> <li>Updated <code>nautobot</code> to <code>2.0.0</code> and made associated changes.</li> <li>Integrated all relevant sections with <code>Platform.network_driver</code>.</li> <li>Added a standard way to provide error codes.</li> <li>Changed Config Compliance view to be based on model, not dynamic group and provide a <code>message</code> when they have drifted.</li> <li>Added constance settings (<code>DEFAULT_FRAMEWORK</code>, <code>GET_CONFIG_FRAMEWORK</code>, <code>MERGE_CONFIG_FRAMEWORK</code>, and <code>REPLACE_CONFIG_FRAMEWORK</code>) and customer_dispatcher to remove dispatcher_mapping.</li> <li>Moved config compliance view to be a tab within device instead of a dedicated page.</li> <li>Removed management command in favor of Nautobot Core's.</li> </ul> <p>Note</p> <p>Please see migrating guide for details on migration.</p>",
             "title": "v2.0 Release Notes"
         },
         {
+            "location": "admin/release_notes/version_2.0.html#v205-2024-05",
+            "text": "",
+            "title": "v2.0.5 2024-05"
+        },
+        {
+            "location": "admin/release_notes/version_2.0.html#fixed",
+            "text": "<ul> <li>#759 - Fix issue with Git Repo not syncing by changing to explicitly use class_path property.</li> </ul>",
+            "title": "Fixed"
+        },
+        {
             "location": "admin/release_notes/version_2.0.html#v204-2024-04",
             "text": "",
             "title": "v2.0.4 2024-04"
         },
         {
-            "location": "admin/release_notes/version_2.0.html#fixed",
+            "location": "admin/release_notes/version_2.0.html#fixed_1",
             "text": "<ul> <li>#749 - Corrected issue where consecutive Golden Config Jobs in All Golden Configs Job wouldn't execute if prior Job had an Exception raised.</li> </ul>",
             "title": "Fixed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#housekeeping",
             "text": "<ul> <li>#741 - Re-baked from the latest template.</li> </ul>",
             "title": "Housekeeping"
@@ -681,45 +691,45 @@
         },
         {
             "location": "admin/release_notes/version_2.0.html#added",
             "text": "<ul> <li>#736 - Add a boolean job parameter <code>fail_job_on_task_failure</code> which will determine whether a single task failure anywhere in the job-result should result in job-result status of failed vs successful.</li> </ul>",
             "title": "Added"
         },
         {
-            "location": "admin/release_notes/version_2.0.html#fixed_1",
+            "location": "admin/release_notes/version_2.0.html#fixed_2",
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
-            "location": "admin/release_notes/version_2.0.html#fixed_2",
+            "location": "admin/release_notes/version_2.0.html#fixed_3",
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
-            "location": "admin/release_notes/version_2.0.html#fixed_3",
+            "location": "admin/release_notes/version_2.0.html#fixed_4",
             "text": "<ul> <li>#676 - Fixes docs for running config plan job in 2.0.</li> <li>#680 - Resolve RTD build issue.</li> <li>#684 - Fix repo sync not executing on any task failure.</li> <li>#685 - Cherry-pick #669 - Removed unneeded lookup for GoldenConfigSetting.</li> <li>#686 - Fix incorrect permissions.</li> </ul>",
             "title": "Fixed"
         },
         {
             "location": "admin/release_notes/version_2.0.html#changed_1",
             "text": "<ul> <li>#658 - Cookie updated by NetworkToCode Cookie Drift Manager Tool.</li> <li>#671 - Finish Documentation Updates from Drift Manager.</li> </ul>",
             "title": "Changed"
```

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml`

 * *Files 6% similar despite different names*

#### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/sitemap.xml`

```diff
@@ -1,373 +1,373 @@
 <?xml version="1.0" encoding="utf-8"?>
 <urlset xmlns="http://www.sitemaps.org/schemas/sitemap/0.9">
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/index.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/compatibility_matrix.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/install.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/migrating_to_v2.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/uninstall.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/upgrade.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/index.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_0.10.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_0.9.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.0.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.1.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.2.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.3.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.4.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.5.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_1.6.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/release_notes/version_2.0.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/index.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3001.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3002.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3003.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3004.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3005.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3006.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3007.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3008.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3009.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3010.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3011.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3012.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3013.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3014.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3015.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3016.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3017.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3018.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3019.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3020.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3021.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3022.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3023.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3024.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3025.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3026.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3027.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3028.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3029.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/admin/troubleshooting/E3030.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/arch_decision.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/contributing.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/dev_environment.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/extending.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/index.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/api.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/models.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/dev/code_reference/package.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_backup.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliance.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancecli.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancecustom.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_compliancejson.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_config_plans.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_config_postprocessing.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_intended.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_remediation.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_feature_sotagg.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_getting_started.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_overview.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/app_use_cases.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/external_interactions.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/faq.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_credentials.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_dispatchers.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
   <url>
     <loc>https://docs.nautobot.com/projects/golden-config/en/latest/user/troubleshooting/troubleshoot_general.html</loc>
-    <lastmod>2024-04-03</lastmod>
+    <lastmod>2024-05-23</lastmod>
     <changefreq>daily</changefreq>
   </url>
 </urlset>
```

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_backup.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliance.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecli.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancecustom.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_compliancejson.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_plans.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_config_postprocessing.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_intended.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_remediation.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_feature_sotagg.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_getting_started.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/app_use_cases.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/external_interactions.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/faq.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_credentials.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_dispatchers.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/nautobot_golden_config/docs/user/troubleshooting/troubleshoot_general.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/run_job.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/run_job.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/static/toggle_fields.js` & `nautobot_golden_config-2.0.5/nautobot_golden_config/static/toggle_fields.js`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tables.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tables.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/template_content.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/template_content.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/compliancefeature_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/compliancerule_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_devicetab.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_overview.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configcompliance_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_create.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configplan_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configremove_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/configreplace_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/content_template.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/content_template.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_detailsmodal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_list.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfig_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/goldenconfigsetting_update.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/job_result_modal.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html` & `nautobot_golden_config-2.0.5/nautobot_golden_config/templates/nautobot_golden_config/remediationsetting_retrieve.html`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/conftest.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/forms/test_golden_config_settings.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/forms/test_golden_config_settings.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_api.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_basic.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_datasources.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_datasources.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_filters.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_graphql.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_helpers.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_jobs.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_models.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_nornir_plays/test_config_compliance.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_config_plan.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_config_plan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_git.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_graphql.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_utilities/test_helpers.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_utilities/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/tests/test_views.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/urls.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/urls.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_plan.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/config_plan.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/config_postprocessing.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/config_postprocessing.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/constant.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/constant.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/db_management.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/db_management.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/git.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/git.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/graphql.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/graphql.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/helper.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/helper.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/logger.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/mat_plot.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/mat_plot.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/utilities/utils.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/nautobot_golden_config/views.py` & `nautobot_golden_config-2.0.5/nautobot_golden_config/views.py`

 * *Files identical despite different names*

### Comparing `nautobot_golden_config-2.0.4/pyproject.toml` & `nautobot_golden_config-2.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nautobot-golden-config"
-version = "v2.0.4"
+version = "v2.0.5"
 description = "An app for configuration on nautobot"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/nautobot/nautobot-app-golden-config"
 repository = "https://github.com/nautobot/nautobot-app-golden-config"
 documentation = "https://docs.nautobot.com/projects/golden-config/en/latest/"
```

### Comparing `nautobot_golden_config-2.0.4/PKG-INFO` & `nautobot_golden_config-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautobot-golden-config
-Version: 2.0.4
+Version: 2.0.5
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
-Metadata-Version: 2.1 Name: nautobot-golden-config Version: 2.0.4 Summary: An
+Metadata-Version: 2.1 Name: nautobot-golden-config Version: 2.0.5 Summary: An
 app for configuration on nautobot Home-page: https://github.com/nautobot/
 nautobot-app-golden-config License: Apache-2.0 Keywords: nautobot,nautobot-
 app,nautobot-plugin Author: Network to Code, LLC Author-email:
 opensource@networktocode.com Requires-Python: >=3.8,<3.12 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

