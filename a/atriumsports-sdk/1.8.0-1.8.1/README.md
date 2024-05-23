# Comparing `tmp/atriumsports_sdk-1.8.0.tar.gz` & `tmp/atriumsports_sdk-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atriumsports_sdk-1.8.0.tar", last modified: Wed Apr 24 22:48:33 2024, max compression
+gzip compressed data, was "atriumsports_sdk-1.8.1.tar", last modified: Thu May 23 08:52:28 2024, max compression
```

## Comparing `atriumsports_sdk-1.8.0.tar` & `atriumsports_sdk-1.8.1.tar`

### file list

```diff
@@ -1,509 +1,509 @@
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:33.327720 atriumsports_sdk-1.8.0/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.8.0/LICENSE
--rw-r--r--   0 k.kieda    (502) staff       (20)     5634 2024-04-24 22:48:33.326909 atriumsports_sdk-1.8.0/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.8.0/README.md
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:31.910128 atriumsports_sdk-1.8.0/atriumsports/
--rw-r--r--   0 k.kieda    (502) staff       (20)     1097 2024-02-13 12:15:30.000000 atriumsports_sdk-1.8.0/atriumsports/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.8.0/atriumsports/atrium_response.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:31.912048 atriumsports_sdk-1.8.0/atriumsports/datacore/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7401 2024-04-24 22:16:59.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/datacore.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:31.927137 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/
--rw-r--r--   0 k.kieda    (502) staff       (20)    62423 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/__init__.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:32.338286 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/
--rw-r--r--   0 k.kieda    (502) staff       (20)     5660 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   120734 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/awards_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59687 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/career_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18893 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/change_log_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    74964 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competition_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    96831 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competition_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127048 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competitions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77982 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conduct_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    74756 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conference_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   137447 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    74208 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/division_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    66129 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/download_video_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    91813 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73565 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    20995 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   127248 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    75127 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_group_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    69993 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_groups_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59298 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    74008 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11179 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    59177 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   119124 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    86391 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76500 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    89126 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   447888 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixtures_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   271916 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/images_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70447 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73212 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/league_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    69832 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leagues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73625 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70029 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/merge_records_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    65837 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/organizations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    35882 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/partner_apis_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23514 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   134126 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    92819 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   107207 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/rankings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   157407 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/roles_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    94294 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entities_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    49499 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71417 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    44544 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_leaders_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    51478 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71412 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_person_placings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    77617 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_persons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    97550 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_roster_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    90055 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_series_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   177284 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_statistics_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   122831 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/seasons_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72966 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/site_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    68237 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/sites_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   229284 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   105183 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    71524 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standing_configurations_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   136931 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standings_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    70919 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/transfers_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73204 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/venue_external_ids_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)   102524 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/venues_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    73804 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    76083 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    72199 2024-04-24 22:13:09.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_streams_available_api.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    28607 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api_client.py
--rw-r--r--   0 k.kieda    (502) staff       (20)      787 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    14726 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5302 2024-04-24 22:12:59.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/exceptions.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:33.313498 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/
--rw-r--r--   0 k.kieda    (502) staff       (20)    42434 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6108 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/award_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5940 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/award_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10489 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2358 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3071 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/blank_model_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5055 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2558 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3776 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4462 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4419 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2549 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3763 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4838 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2918 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2676 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4316 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4415 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2549 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3763 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9610 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9381 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11979 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2404 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12235 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2464 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2524 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3727 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    24250 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2365 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2952 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    19418 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    19279 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5065 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2501 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3129 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2892 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3691 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5707 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5188 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7601 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2396 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3569 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3142 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/contact_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4985 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3083 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2856 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3667 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6123 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5690 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8560 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2380 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    19002 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3533 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2524 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5255 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4677 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5296 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4885 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2510 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2926 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2682 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3704 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4890 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11302 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4236 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3420 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11133 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13249 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2405 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4850 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16495 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4172 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3362 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16373 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1957 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/environmental_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2863 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/error_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2839 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/error_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6958 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13584 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2384 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2346 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10136 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3618 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2761 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4714 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2517 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5207 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2573 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3809 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2258 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3715 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4729 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2477 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2828 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2606 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2717 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6439 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_participant.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10079 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2453 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7669 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7078 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3619 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4500 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2390 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2674 2023-09-07 13:28:45.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3558 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7638 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2517 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6104 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2574 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3152 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3809 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4781 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3715 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10885 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7941 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23517 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3974 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2664 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2407 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3618 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3560 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3239 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5984 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2392 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3666 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23389 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7178 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2414 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4330 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3215 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    29959 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3691 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_competition_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    29919 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    29855 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2385 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2372 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_round.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2331 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_series.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2302 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3533 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4993 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3595 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7695 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3595 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1911 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_identification.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2063 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2513 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9721 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2357 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1771 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2475 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1904 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/included_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3214 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2443 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2099 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1851 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3824 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3649 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5881 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2470 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2458 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3630 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2742 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_summary_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_summary_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4686 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model_league.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6666 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6544 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8607 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6008 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organization_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5798 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organization_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7133 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organizations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3593 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organizations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5700 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_additional_details.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4673 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5847 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2570 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_list_default_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13384 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5748 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13329 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15357 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6117 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/pool_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/pool_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5578 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4632 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4472 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3570 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2214 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/response_links.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3451 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/response_meta_data.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11652 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/role_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11531 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/role_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15539 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2348 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3497 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7071 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/round_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6641 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/round_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8862 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2472 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9032 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5638 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6507 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3964 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3752 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4073 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3679 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5255 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4693 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6236 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2554 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2468 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2478 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3786 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7190 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4144 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3752 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4073 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_placings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3679 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_placings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5745 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6209 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3797 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5119 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2550 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3764 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6850 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2464 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7020 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4086 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     8515 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2390 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3570 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    19143 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    19295 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10471 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2406 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5995 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10010 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2398 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4480 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_competitor.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    16347 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2399 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5747 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stage_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5262 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stage_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7551 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2405 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5302 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2570 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5304 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11016 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2456 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3557 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3368 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3557 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3368 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3985 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    23181 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_competition.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2478 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12224 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/series_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11929 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/series_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5239 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4593 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2453 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2799 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3619 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6552 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6368 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7800 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2348 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3497 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3273 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/social_media.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2251 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sorting.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13470 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13444 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18626 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3666 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5377 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_building.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    15190 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configuration.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6236 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2510 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4863 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4577 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3702 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12112 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    21786 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4760 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12113 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    18150 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2380 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1792 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/success_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/success_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2638 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_component.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7501 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     7342 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9843 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5247 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_address.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     4571 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2790 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2578 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5340 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_historical_name.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10645 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10477 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12582 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2276 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model_site.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    10311 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_file_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2177 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_download_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_download_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    12235 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2389 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3558 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11761 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     5357 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3487 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3326 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     9482 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2477 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11477 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    11591 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py
--rw-r--r--   0 k.kieda    (502) staff       (20)    13678 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     2475 2024-04-24 22:13:08.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     3654 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:12:44.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/py.typed
--rw-r--r--   0 k.kieda    (502) staff       (20)    12752 2024-04-24 22:13:07.000000 atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/rest.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:33.317434 atriumsports_sdk-1.8.0/atriumsports/datacore_stream/
--rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.8.0/atriumsports/datacore_stream/__init__.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.8.0/atriumsports/datacore_stream/datacore_stream.py
--rw-r--r--   0 k.kieda    (502) staff       (20)     1951 2023-11-16 13:07:43.000000 atriumsports_sdk-1.8.0/atriumsports/endpoints.py
-drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-04-24 22:48:33.325827 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/
--rw-r--r--   0 k.kieda    (502) staff       (20)     5634 2024-04-24 22:48:31.000000 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/PKG-INFO
--rw-r--r--   0 k.kieda    (502) staff       (20)    32404 2024-04-24 22:48:31.000000 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)        1 2024-04-24 22:48:31.000000 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)      134 2024-04-24 22:48:31.000000 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/requires.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       13 2024-04-24 22:48:31.000000 atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/top_level.txt
--rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.8.0/pyproject.toml
--rw-r--r--   0 k.kieda    (502) staff       (20)       38 2024-04-24 22:48:33.327794 atriumsports_sdk-1.8.0/setup.cfg
--rw-r--r--   0 k.kieda    (502) staff       (20)      988 2024-04-24 22:12:37.000000 atriumsports_sdk-1.8.0/setup.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.339633 atriumsports_sdk-1.8.1/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1074 2023-03-17 13:13:15.000000 atriumsports_sdk-1.8.1/LICENSE
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5634 2024-05-23 08:52:28.338988 atriumsports_sdk-1.8.1/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4963 2023-06-16 15:49:48.000000 atriumsports_sdk-1.8.1/README.md
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.004203 atriumsports_sdk-1.8.1/atriumsports/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1097 2024-02-13 12:15:30.000000 atriumsports_sdk-1.8.1/atriumsports/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4294 2023-04-24 10:52:41.000000 atriumsports_sdk-1.8.1/atriumsports/atrium_response.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.005241 atriumsports_sdk-1.8.1/atriumsports/datacore/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2022-11-21 11:07:25.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7473 2024-05-23 08:48:47.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/datacore.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.008978 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    62423 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/__init__.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.071642 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5660 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   120734 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/awards_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59687 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/career_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18893 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/change_log_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    74964 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competition_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    96831 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competition_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127048 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competitions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77982 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conduct_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    74756 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conference_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   137447 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conferences_divisions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    74208 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/division_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    66129 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/download_video_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    91813 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73565 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    20995 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   127248 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    75127 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_group_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    69993 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_groups_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59298 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    74008 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11179 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_live_summary_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    59177 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   119124 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    86391 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_profiles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76500 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_progressions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    89126 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   447888 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixtures_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   271916 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/images_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70447 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73212 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leader_qualifiers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/league_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    69832 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leagues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73625 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/local_video_endpoints_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70029 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/merge_records_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    65837 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/organizations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    35882 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/partner_apis_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23514 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_fixture_history_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   134126 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    92819 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   107207 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/rankings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   157407 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/roles_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    94294 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entities_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    49499 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71417 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entity_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73548 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    44544 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_leaders_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    51478 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71412 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_person_placings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    77617 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_persons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    97550 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_roster_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    90055 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_series_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   177284 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_statistics_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   122831 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/seasons_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72966 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/site_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    68237 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/sites_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   229284 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   105183 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standing_adjustments_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    71524 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standing_configurations_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   136931 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standings_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    70919 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/transfers_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73204 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/venue_external_ids_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)   102524 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/venues_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    73804 2024-05-23 08:50:58.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_stream_inputs_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    76083 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    72199 2024-05-23 08:50:59.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_streams_available_api.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    28607 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api_client.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)      787 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    14726 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5302 2024-05-23 08:50:51.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/exceptions.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.327895 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/
+-rw-r--r--   0 k.kieda    (502) staff       (20)    42434 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6108 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/award_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5940 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/award_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10489 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2358 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3071 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/blank_model_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5055 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2558 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3776 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4462 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3546 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4419 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2549 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3763 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4838 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2918 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2676 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4316 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4415 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2549 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3763 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9610 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9381 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11979 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2344 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2404 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3581 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12235 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2464 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2524 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3727 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    24250 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2365 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2952 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_penalty_result.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19418 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19279 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5065 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2501 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3129 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2892 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3691 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5707 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5188 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7601 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2396 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3569 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3142 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/contact_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4985 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3083 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2856 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3667 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6123 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5690 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8560 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2380 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19002 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2362 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model_entity_group.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2371 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3533 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2524 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5255 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4677 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5296 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4885 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2510 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2926 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2682 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3704 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4890 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11302 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4236 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3420 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11133 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13249 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2405 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4850 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16495 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4172 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3362 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body_colors.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16373 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1957 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/environmental_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2863 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/error_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2839 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/error_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6958 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13584 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2384 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_division.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2346 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10136 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3618 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2761 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4714 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2517 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5207 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2573 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3809 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2258 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3715 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4729 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2477 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2828 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2606 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2717 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_live_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_live_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6439 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_participant.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10079 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2453 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7669 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7078 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3619 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4500 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2390 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2674 2023-09-07 13:28:45.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3558 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7638 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2517 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6104 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2574 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3152 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3809 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4781 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3715 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10885 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2444 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2337 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model_person.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7941 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23517 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3974 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2452 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2664 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2407 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3618 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3560 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progression_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3239 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progression_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5984 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2392 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3666 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23389 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7178 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2414 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4330 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3215 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    29959 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3691 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_competition_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    29919 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    29855 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2385 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2372 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2318 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_round.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2331 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_series.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2302 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_venue.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3533 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4993 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3595 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7695 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2415 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3595 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1911 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_identification.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2063 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_resolution.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2513 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9721 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2357 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1771 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2475 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1904 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/included_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3214 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2443 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2099 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1851 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3824 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3649 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5881 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2470 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2458 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3630 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2742 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_summary_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_summary_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4686 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2387 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model_league.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6666 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6544 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8607 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6008 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organization_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5798 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organization_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7133 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organizations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3593 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organizations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5700 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_additional_details.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4673 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5847 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2570 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_list_default_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13384 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5748 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13329 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15357 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6117 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/pool_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5693 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/pool_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5578 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4632 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4472 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3570 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2214 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/response_links.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3451 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/response_meta_data.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11652 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/role_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11531 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/role_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15539 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2348 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3497 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7071 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/round_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6641 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/round_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8862 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2472 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9032 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5638 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3606 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6507 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3964 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3752 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4073 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3679 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5255 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4693 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2809 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6236 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2554 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2468 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2478 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3786 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7190 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2542 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4144 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3752 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4073 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_placings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3679 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_placings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5745 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6209 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3797 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3703 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5119 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2550 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3764 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6850 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2464 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7020 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4086 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3594 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     8515 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2390 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3570 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19143 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    19295 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10471 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2406 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5995 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10010 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2398 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4480 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_competitor.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    16347 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2399 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5747 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stage_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5262 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stage_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7551 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2405 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3582 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5302 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2570 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3810 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5304 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11016 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2456 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3557 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3368 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3557 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3368 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3985 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonroster_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    23181 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2354 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_competition.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2377 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2364 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2478 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12224 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/series_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11929 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/series_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5239 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4593 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2453 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2351 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2799 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2592 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3619 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6552 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6368 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7800 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2348 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3497 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3273 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/social_media.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2251 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sorting.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13470 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13444 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18626 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2485 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3666 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5377 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_building.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    15190 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configuration.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6236 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2510 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4863 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4577 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3702 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12112 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    21786 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4760 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body_points_value.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12113 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    18150 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2380 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1792 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/success_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3521 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/success_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2638 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_component.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7501 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     7342 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9843 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2382 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3545 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5247 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_address.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     4571 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2790 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2578 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5340 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_historical_name.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10645 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10477 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12582 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2356 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2276 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model_site.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3509 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    10311 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_file_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2177 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_download_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_download_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12235 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2389 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3558 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11761 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2469 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3643 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5357 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2461 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3487 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3326 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3631 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     9482 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2477 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3655 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11477 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscription_post_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    11591 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscription_put_body.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)    13678 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_model.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     2475 2024-05-23 08:50:57.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     3654 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_response.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:50:38.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/py.typed
+-rw-r--r--   0 k.kieda    (502) staff       (20)    12752 2024-05-23 08:50:56.000000 atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/rest.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.329009 atriumsports_sdk-1.8.1/atriumsports/datacore_stream/
+-rw-r--r--   0 k.kieda    (502) staff       (20)        0 2023-03-17 13:13:17.000000 atriumsports_sdk-1.8.1/atriumsports/datacore_stream/__init__.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     6124 2023-04-24 10:52:46.000000 atriumsports_sdk-1.8.1/atriumsports/datacore_stream/datacore_stream.py
+-rw-r--r--   0 k.kieda    (502) staff       (20)     1951 2023-11-16 13:07:43.000000 atriumsports_sdk-1.8.1/atriumsports/endpoints.py
+drwxr-xr-x   0 k.kieda    (502) staff       (20)        0 2024-05-23 08:52:28.338275 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/
+-rw-r--r--   0 k.kieda    (502) staff       (20)     5634 2024-05-23 08:52:27.000000 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 k.kieda    (502) staff       (20)    32404 2024-05-23 08:52:27.000000 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)        1 2024-05-23 08:52:27.000000 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)      134 2024-05-23 08:52:27.000000 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/requires.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       13 2024-05-23 08:52:27.000000 atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/top_level.txt
+-rw-r--r--   0 k.kieda    (502) staff       (20)       80 2023-04-24 10:51:20.000000 atriumsports_sdk-1.8.1/pyproject.toml
+-rw-r--r--   0 k.kieda    (502) staff       (20)       38 2024-05-23 08:52:28.339692 atriumsports_sdk-1.8.1/setup.cfg
+-rw-r--r--   0 k.kieda    (502) staff       (20)      988 2024-05-23 08:50:24.000000 atriumsports_sdk-1.8.1/setup.py
```

### Comparing `atriumsports_sdk-1.8.0/LICENSE` & `atriumsports_sdk-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/PKG-INFO` & `atriumsports_sdk-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports_sdk
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.8.0/README.md` & `atriumsports_sdk-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/__init__.py` & `atriumsports_sdk-1.8.1/atriumsports/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/atrium_response.py` & `atriumsports_sdk-1.8.1/atriumsports/atrium_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/datacore.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/datacore.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     pass
 
 
 class DatacoreAPI:
     """A class to handle the connection to AtriumSports Datacore"""
 
     DEFAULT_LIMIT = 10
-    MAX_LIMIT = 200
+    DEFAULT_PAGE_LIMIT = 200
 
     def __init__(self, options):
         """initialise the class"""
         self._sport = options.get("sport", "basketball")
         self._credential_id = options.get("credential_id", "")
         self._credential_secret = options.get("credential_secret", "")
         self._org_group = options.get("org_group")
@@ -138,15 +138,16 @@
         except jwt.exceptions.ExpiredSignatureError:
             return True
 
     def call(self, method, url, **kwargs):
         url = self._get_api_url(url)
 
         limit = kwargs.get("limit", self.DEFAULT_LIMIT)
-        kwargs["limit"] = self._get_limit(limit)
+        page_limit = kwargs.pop("page_limit", self.DEFAULT_PAGE_LIMIT)
+        kwargs["limit"] = self._get_call_limit(limit, page_limit)
         kwargs["headers"] = self._get_headers(kwargs.get("headers"))
 
         response = AtriumResponse()
         while True:
             resp = self._api_call_internal(method, url, **kwargs)
             response.merge(resp)
             if not resp.success():
@@ -156,23 +157,22 @@
                 break
             # don't pass offset or limit params to next page call if it's already in the url
             if "offset=" in next_page_url and "offset" in kwargs:
                 kwargs.pop("offset")
             if "limit=" in next_page_url and "limit" in kwargs:
                 kwargs.pop("limit")
             url = next_page_url
-            call_limit = self._get_limit(limit - response.data_count())
+            call_limit = self._get_call_limit(limit - response.data_count(), page_limit)
             if call_limit <= 0:
                 break
 
         return response
 
-    def _get_limit(self, limit):
-        """make sure limit doesn't exceed MAX_LIMIT"""
-        return min(limit, self.MAX_LIMIT)
+    def _get_call_limit(self, limit, page_limit):
+        return min(limit, page_limit)
 
     def _get_headers(self, headers=None):
         result_headers = self._headers.copy()
         result_headers.update(headers or {})
         result_headers["Authorization"] = "Bearer {}".format(self.auth_token)
         result_headers["Content-Type"] = "application/json"
         return result_headers
```

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/__init__.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,15 +239,15 @@
 
 This **access token** must then be sent in the `Authorization` header for each subsequent API call.  Access tokens have a finite life and will expire. When the token expires you will need to create a new token to make more API calls.  Creation of tokens is rate-limited, so you should use the existing token as long as possible.
 
 <!-- ReDoc-Inject: <security-definitions> -->
   # noqa: E501
 """
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
 
 # import apis into sdk package
 from atriumsports.datacore.openapi.api.awards_api import AwardsApi
 from atriumsports.datacore.openapi.api.career_statistics_api import CareerStatisticsApi
 from atriumsports.datacore.openapi.api.change_log_api import ChangeLogApi
 from atriumsports.datacore.openapi.api.competition_external_ids_api import CompetitionExternalIDsApi
 from atriumsports.datacore.openapi.api.competition_statistics_api import CompetitionStatisticsApi
```

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/__init__.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/awards_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/awards_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/career_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/career_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/change_log_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/change_log_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competition_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competition_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competition_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competition_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/competitions_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/competitions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conduct_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conduct_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conference_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conference_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/conferences_divisions_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/conferences_divisions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/division_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/division_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/download_video_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/download_video_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entities_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_fixture_history_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_group_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_group_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/entity_groups_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/entity_groups_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_entities_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_live_summary_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_live_summary_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_persons_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_playbyplay_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_profiles_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_profiles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_progressions_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_progressions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixture_roster_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixture_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/fixtures_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/fixtures_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/images_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/images_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leader_criteria_sets_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leader_qualifiers_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leader_qualifiers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/league_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/league_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/leagues_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/leagues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/local_video_endpoints_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/local_video_endpoints_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/merge_records_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/merge_records_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/organizations_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/organizations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/partner_apis_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/partner_apis_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_fixture_history_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_fixture_history_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/person_fixture_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/persons_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/rankings_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/rankings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/roles_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entities_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entities_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entity_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_entity_placings_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_entity_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_leaders_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_leaders_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_person_base_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_person_placings_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_person_placings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_persons_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_persons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_roster_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_roster_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_series_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_series_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/season_statistics_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/season_statistics_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/seasons_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/seasons_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/site_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/site_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/sites_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/sites_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/stages_pools_rounds_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standing_adjustments_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standing_adjustments_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standing_configurations_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standing_configurations_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/standings_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/standings_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/transfers_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/transfers_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/venue_external_ids_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/venue_external_ids_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/venues_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/venues_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_stream_inputs_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_stream_inputs_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_stream_subscriptions_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api/video_streams_available_api.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api/video_streams_available_api.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api_client.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = "AtriumSportsSDK/1.8.0"
+        self.user_agent = "AtriumSportsSDK/1.8.1"
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/api_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/api_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/configuration.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
         :return: The report for debugging.
         """
         return (
             "Python SDK Debug Report:\n"
             "OS: {env}\n"
             "Python Version: {pyversion}\n"
             "Version of the API: v1\n"
-            "SDK Package Version: 1.8.0".format(env=sys.platform, pyversion=sys.version)
+            "SDK Package Version: 1.8.1".format(env=sys.platform, pyversion=sys.version)
         )
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/exceptions.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/__init__.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/award_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/award_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/award_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/award_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/awards_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/awards_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/blank_model_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/blank_model_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_season_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/career_person_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/career_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/change_log_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/change_log_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_historical_name.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_person_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competition_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competition_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model_league.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/competitions_season_status_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/competitions_season_status_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_penalty_result.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_penalty_result.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conduct_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conduct_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conference_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conference_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/conferences_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/conferences_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/contact_details.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/contact_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/division_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/division_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/divisions_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/divisions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model_entity_group.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model_entity_group.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entities_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_additional_details.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_address.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_address.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_historical_name.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_group_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_group_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_groups_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_groups_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_historical_name.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body_additional_names.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_post_body_colors.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_post_body_colors.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/entity_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/entity_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/environmental_details.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/environmental_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/error_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/error_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/error_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/error_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_competitor.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_conference.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_division.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_division.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_entity.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entities_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_period_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_live_summary_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_live_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_live_summary_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_live_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_participant.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_participant.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_event_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_pbp_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_pbp_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_model_person.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_model_person.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_persons_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_profiles_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_profiles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progression_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progression_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progression_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progression_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_fixture.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_model_season.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_progressions_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_progressions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_roster_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixture_videosteam_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_competition_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_competition_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_competition_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_by_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_round.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_round.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_series.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_series.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_model_venue.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_model_venue.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/fixtures_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/fixtures_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_entity_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_entity_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/game_log_person_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/game_log_person_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_identification.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_identification.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_identification_for_subsequent_checks.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_resolution.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_resolution.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/head_to_head_resolution_for_extra_depth_h2h_s.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/images_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/images_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/included_data.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/included_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_criteria_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_criteria_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifier_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifier_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_leaders_criteria.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_qualifiers_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_qualifiers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_summary_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_summary_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leader_summary_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leader_summary_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model_league.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model_league.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/league_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/league_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/leagues_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/leagues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organization_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organization_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organization_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organization_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organizations_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organizations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/organizations_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/organizations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_additional_details.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_additional_details.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_historical_name.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_list_default_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_list_default_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_post_body_additional_names_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/person_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/person_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/persons_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/pool_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/pool_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/pool_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/pool_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/ranking_rows_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/ranking_rows_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/response_links.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/response_links.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/response_meta_data.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/response_meta_data.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/role_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/role_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/role_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/role_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/roles_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/roles_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/round_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/round_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/round_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/round_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_list_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entities_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entities_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_placings_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_placings_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_entity_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_entity_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_pool.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_model_stage.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_fixture_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_base_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_placings_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_placings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_placings_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_placings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_periods_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_person_total_statistics_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_list_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_persons_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_persons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_pools_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_pools_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_roster_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_roster_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_rounds_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_rounds_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_competitor.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_competitor.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_series_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_series_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stage_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stage_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stage_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stage_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_stages_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_stages_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_standings_stages_pools_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_address.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_model_site.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/season_venues_list_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/season_venues_list_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonentity_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonentity_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonperson_placings_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonperson_placings_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasonroster_configuration.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasonroster_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_competition.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_competition.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_fixture_profile.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_model_standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/seasons_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/seasons_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/series_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/series_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/series_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/series_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_address.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_model_site.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/site_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/site_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sites_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sites_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/social_media.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/social_media.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/sorting.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/sorting.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustment_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustment_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_adjustments_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_adjustments_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_building.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_building.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configuration.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configuration.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_configurations_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_configurations_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body_calculated_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_post_body_points_value.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_post_body_points_value.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standing_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standing_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/standings_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/standings_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/success_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/success_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/success_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/success_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_component.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_component.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfer_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfer_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/transfers_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/transfers_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_address.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_address.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_external_ids_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_external_ids_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_historical_name.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_historical_name.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venue_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venue_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_model_site.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_model_site.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/venues_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/venues_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_file_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_file_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_download_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_download_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_download_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_download_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_files_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_files_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_inputs_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_inputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_local_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_local_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_stream_outputs_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_stream_outputs_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscription_post_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscription_post_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscription_put_body.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscription_put_body.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_model.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_model.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_model_organization.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/models/video_subscriptions_response.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/models/video_subscriptions_response.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore/openapi/rest.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore/openapi/rest.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/datacore_stream/datacore_stream.py` & `atriumsports_sdk-1.8.1/atriumsports/datacore_stream/datacore_stream.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports/endpoints.py` & `atriumsports_sdk-1.8.1/atriumsports/endpoints.py`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/PKG-INFO` & `atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atriumsports_sdk
-Version: 1.8.0
+Version: 1.8.1
 Summary: Python module for integration to Atrium Sports APIs
 Author: Atrium Sports
 Author-email: python_dev@atriumsports.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atriumsports_sdk-1.8.0/atriumsports_sdk.egg-info/SOURCES.txt` & `atriumsports_sdk-1.8.1/atriumsports_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atriumsports_sdk-1.8.0/setup.py` & `atriumsports_sdk-1.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
     setuptools.setup(
         name="atriumsports_sdk",
-        version="1.8.0",
+        version="1.8.1",
         author="Atrium Sports",
         author_email="python_dev@atriumsports.com",
         description="Python module for integration to Atrium Sports APIs",
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=setuptools.find_packages(),
         classifiers=[
```

