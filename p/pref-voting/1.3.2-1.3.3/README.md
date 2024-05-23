# Comparing `tmp/pref_voting-1.3.2.tar.gz` & `tmp/pref_voting-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-1.3.2.tar", max compression
+gzip compressed data, was "pref_voting-1.3.3.tar", max compression
```

## Comparing `pref_voting-1.3.2.tar` & `pref_voting-1.3.3.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.2/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.2/README.md
--rw-r--r--   0        0        0       22 2024-05-10 21:47:10.807987 pref_voting-1.3.2/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-1.3.2/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.2/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.2/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.2/pref_voting/axioms.py
--rw-r--r--   0        0        0    36988 2024-05-05 11:00:01.290334 pref_voting-1.3.2/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    17962 2024-05-05 11:00:01.291557 pref_voting-1.3.2/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.2/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.2/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.2/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.2/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-1.3.2/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.2/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.2/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.2/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.2/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.2/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.2/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.2/pref_voting/io/writers.py
--rw-r--r--   0        0        0    99843 2024-05-06 20:13:55.325756 pref_voting-1.3.2/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.2/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-1.3.2/pref_voting/mappings.py
--rw-r--r--   0        0        0    79313 2024-05-10 21:46:49.192278 pref_voting-1.3.2/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.2/pref_voting/margin_based_methods_old.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.2/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    30314 2024-05-05 11:00:01.294267 pref_voting-1.3.2/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.2/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.2/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-05-06 22:04:52.586763 pref_voting-1.3.2/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.2/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.2/pref_voting/rankings.py
--rw-r--r--   0        0        0    23114 2024-05-05 11:00:01.294774 pref_voting-1.3.2/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.2/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.2/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.2/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.2/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.2/pref_voting/swf_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.2/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.2/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.2/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.2/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.2/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.2/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.2/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.2/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.2/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.2/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.2/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.2/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.2/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.2/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.2/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.2/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.2/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.2/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.2/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.2/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.2/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.2/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.2/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.2/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.2/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.2/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-1.3.2/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.2/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.2/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     7222 2024-05-09 10:50:06.223765 pref_voting-1.3.2/pref_voting/voting_method.py
--rw-r--r--   0        0        0     1341 2024-04-30 00:59:45.610622 pref_voting-1.3.2/pref_voting/voting_method_properties.py
--rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.2/pref_voting/voting_methods.py
--rw-r--r--   0        0        0     4679 2024-05-04 21:29:02.086406 pref_voting-1.3.2/pref_voting/voting_methods_registry.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.2/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-05-10 21:47:10.806547 pref_voting-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.3.2/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-24 21:45:43.110237 pref_voting-1.3.3/README.md
+-rw-r--r--   0        0        0       22 2024-05-23 20:04:35.392645 pref_voting-1.3.3/pref_voting/__init__.py
+-rw-r--r--   0        0        0    22307 2024-05-10 21:48:51.212907 pref_voting-1.3.3/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-1.3.3/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-1.3.3/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-1.3.3/pref_voting/axioms.py
+-rw-r--r--   0        0        0    34812 2024-05-23 19:59:31.870067 pref_voting-1.3.3/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15607 2024-05-23 19:52:35.351135 pref_voting-1.3.3/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12837 2024-05-03 10:23:29.480445 pref_voting-1.3.3/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-1.3.3/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-1.3.3/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-1.3.3/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12631 2024-05-10 21:48:51.214555 pref_voting-1.3.3/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-1.3.3/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-1.3.3/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8058 2024-05-05 11:00:01.292540 pref_voting-1.3.3/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-1.3.3/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-1.3.3/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-1.3.3/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-1.3.3/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    94636 2024-05-23 19:57:51.201863 pref_voting-1.3.3/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-1.3.3/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    23485 2024-05-23 19:37:48.841243 pref_voting-1.3.3/pref_voting/mappings.py
+-rw-r--r--   0        0        0    76503 2024-05-23 19:59:35.003643 pref_voting-1.3.3/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    70814 2024-04-27 22:10:28.624211 pref_voting-1.3.3/pref_voting/margin_based_methods_old.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-1.3.3/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    28588 2024-05-23 19:59:33.435734 pref_voting-1.3.3/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-1.3.3/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-1.3.3/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30689 2024-05-23 18:59:19.624131 pref_voting-1.3.3/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-1.3.3/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-1.3.3/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21877 2024-05-23 19:59:30.042191 pref_voting-1.3.3/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-1.3.3/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-1.3.3/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-1.3.3/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-30 00:43:41.503635 pref_voting-1.3.3/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0     7881 2024-05-01 10:27:56.905820 pref_voting-1.3.3/pref_voting/swf_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-1.3.3/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      745 2024-04-28 20:04:29.865701 pref_voting-1.3.3/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5690 2024-04-28 20:01:53.768645 pref_voting-1.3.3/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     3092 2024-04-28 20:01:53.768816 pref_voting-1.3.3/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-1.3.3/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-1.3.3/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-1.3.3/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0    11606 2024-04-28 20:41:27.682198 pref_voting-1.3.3/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-1.3.3/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-1.3.3/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0    10335 2024-04-28 12:01:51.077156 pref_voting-1.3.3/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-1.3.3/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-1.3.3/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-1.3.3/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-1.3.3/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-1.3.3/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-1.3.3/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     6234 2024-04-28 20:40:55.278187 pref_voting-1.3.3/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-1.3.3/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-1.3.3/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-1.3.3/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-1.3.3/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-1.3.3/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-1.3.3/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-1.3.3/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-1.3.3/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12849 2024-05-23 18:23:59.371156 pref_voting-1.3.3/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-1.3.3/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    91144 2024-05-03 10:23:29.483544 pref_voting-1.3.3/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     9035 2024-05-23 20:01:10.062042 pref_voting-1.3.3/pref_voting/voting_method.py
+-rw-r--r--   0        0        0     1268 2024-05-23 19:41:55.077984 pref_voting-1.3.3/pref_voting/voting_method_properties.py
+-rw-r--r--   0        0        0      254 2024-05-04 20:05:10.058403 pref_voting-1.3.3/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0     4740 2024-05-23 20:04:13.303998 pref_voting-1.3.3/pref_voting/voting_methods_registry.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-1.3.3/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-05-23 20:04:35.390873 pref_voting-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-1.3.3/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-1.3.3/PKG-INFO
```

### Comparing `pref_voting-1.3.2/LICENSE` & `pref_voting-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/README.md` & `pref_voting-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/analysis.py` & `pref_voting-1.3.3/pref_voting/analysis.py`

 * *Files 13% similar despite different names*

```diff
@@ -162,14 +162,104 @@
                     )
                     data_for_df["condorcet_efficiency"].append(
                         num_choose_cw[vm.name] / num_cw
                     )
 
     return pd.DataFrame(data_for_df)
 
+def record_num_winners_data(vms, num_cands, num_voters, probmod, probmod_param, t):
+
+    prof = generate_profile(num_cands, num_voters, probmod=probmod, probmod_param=probmod_param)
+
+    return {
+        "num_winners": {vm.name: len(vm(prof)) for vm in vms},
+    }
+
+def resoluteness_data(
+    vms,
+    numbers_of_candidates=[3, 4, 5],
+    numbers_of_voters=[4, 10, 20, 50, 100, 500, 1000],
+    probmods=["IC"],
+    probmod_params=None,
+    num_trials=10000,
+    use_parallel=True,
+    num_cpus=12,
+):
+    """
+    Returns a Pandas DataFrame with resoluteness data for a list of voting methods.
+
+    Args:
+        vms (list(functions)): A list of voting methods,
+        numbers_of_candidates (list(int), default = [3, 4, 5]): The numbers of candidates to check.
+        numbers_of_voters (list(int), default = [5, 25, 50, 100]): The numbers of voters to check.
+        probmod (str, default="IC"): The probability model to be passed to the ``generate_profile`` method
+        num_trials (int, default=10000): The number of profiles to check for different winning sets.
+        use_parallel (bool, default=True): If True, then use parallel processing.
+        num_cpus (int, default=12): The number of (virtual) cpus to use if using parallel processing.
+
+    """
+
+    probmod_params_list = [None]*len(probmods) if probmod_params is None else probmod_params
+
+    assert len(probmod_params_list) == len(probmods), "probmod_params must be a list of the same length as probmods"
+
+    if use_parallel:
+        pool = Pool(num_cpus)
+
+    data_for_df = {
+        "vm": list(),
+        "num_cands": list(),
+        "num_voters": list(),
+        "probmod": list(),
+        "probmod_param":list(),
+        "num_trials": list(),
+        "avg_num_winners": list(),
+        "avg_percent_winners": list(),
+    }
+    for probmod,probmod_param in zip(probmods, probmod_params_list):
+        for num_cands in numbers_of_candidates:
+            for num_voters in numbers_of_voters:
+
+                print(f"{num_cands} candidates, {num_voters} voters")
+                get_data = partial(
+                    record_num_winners_data,
+                    vms,
+                    num_cands,
+                    num_voters,
+                    probmod,
+                    probmod_param
+                )
+
+                if use_parallel:
+                    data = pool.map(get_data, range(num_trials))
+                else:
+                    data = list(map(get_data, range(num_trials)))
+                    
+                num_winners = {vm.name: 0 for vm in vms}
+
+                for d in data:
+                    for vm in vms:
+                        num_winners[vm.name] += int(d["num_winners"][vm.name])
+
+                for vm in vms:
+                    data_for_df["vm"].append(vm.name)
+                    data_for_df["num_cands"].append(num_cands)
+                    data_for_df["num_voters"].append(num_voters)
+                    data_for_df["probmod"].append(probmod)
+                    data_for_df["probmod_param"].append(probmod_param)
+                    data_for_df["num_trials"].append(num_trials)
+                    data_for_df["avg_num_winners"].append(
+                        num_winners[vm.name] / num_trials
+                    )
+                    data_for_df["avg_percent_winners"].append(
+                        (num_winners[vm.name] / (num_cands * num_trials))
+                    )
+
+    return pd.DataFrame(data_for_df)
+
 # helper function for axiom_violations_data
 def record_axiom_violation_data(
     axioms, 
     vms, 
     num_cands, 
     num_voters, 
     probmod,
```

### Comparing `pref_voting-1.3.2/pref_voting/axiom.py` & `pref_voting-1.3.3/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/c1_methods.py` & `pref_voting-1.3.3/pref_voting/c1_methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,24 +14,17 @@
 from pref_voting.rankings import Ranking, break_ties_alphabetically
 from pref_voting.social_welfare_function import swf
 import copy
 import math
 from itertools import product, permutations, combinations, chain
 import networkx as nx
 import matplotlib.pyplot as plt
-from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
+from pref_voting.voting_method_properties import ElectionTypes
 
-condorcet_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=False,
-    pareto_dominance=False,
-    positive_involvement=False,
-    )
 @vm(name = "Condorcet",
-    properties = condorcet_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def condorcet(edata, curr_cands = None):
     """
     Return the Condorcet winner if one exists, otherwise return all the candidates.  A Condorcet winner is a candidate :math:`c` that is majority preferred to every other candidate. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `condorcet_winner` method. 
@@ -70,22 +63,15 @@
     """
    
     candidates = edata.candidates if curr_cands is None else curr_cands
     cond_winner = edata.condorcet_winner(curr_cands = curr_cands)
     
     return [cond_winner] if cond_winner is not None else sorted(candidates)
 
-copeland_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Copeland",
-    properties = copeland_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def copeland(edata, curr_cands = None):
     """The Copeland score for c is the number of candidates that c is majority preferred to minus the number of candidates majority preferred to c.  The Copeland winners are the candidates with the maximum Copeland score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -159,22 +145,15 @@
 
     if tie_breaking == "alphabetic":
         copeland_ranking = break_ties_alphabetically(copeland_ranking)
 
     return copeland_ranking
 
 
-llull_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Llull",
-    properties = llull_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def llull(edata, curr_cands = None):
     """The Llull score for a candidate :math:`c` is the number of candidates that :math:`c` is weakly majority preferred to.  This is equivalent to calculating the Copeland scores for a candidate :math:`c` with 1 point for each candidate that :math:`c` is majority preferred to, 1/2 point for each candidate that :math:`c` is tied with, and 0 points for each candidate that is majority preferred to :math:`c`.  The Llull winners are the candidates with the maximum Llull score in the profile restricted to ``curr_cands``. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `copeland_scores` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -226,21 +205,15 @@
 
 def right_covers(dom, c1, c2):
     # right covers: c1 right covers c2 when all the candidates that c2  majority preferrs are majority
     # preferred by c1
       
     return dom[c2].issubset(dom[c1])
 
-uc_gill_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
-
 @vm(name = "Uncovered Set",
-    properties = uc_gill_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_gill(edata, curr_cands = None): 
     """Uncovered Set (Gillies version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` defeats :math:`b` in the election if :math:`a` is majority preferred to :math:`b` and :math:`a` left covers :math:`b`: i.e., for all :math:`c`, if :math:`c` is majority preferred to :math:`a`,  then :math:`c` majority preferred to :math:`b`. The winners are the set of candidates who are undefeated in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `dominators` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -324,20 +297,15 @@
         for c2 in edata.dominators(c1, curr_cands = curr_cands): # consider only c2 predecessors
             if c1 != c2:
                 # check if c2 left covers  c1 
                 if left_covers(dom, c2, c1):
                     defeat.add_edge(c2, c1)
     return defeat
 
-uc_fish_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Uncovered Set - Fishburn",
-    properties = uc_fish_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_fish(edata, curr_cands = None): 
     """Uncovered Set (Fishburn version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` defeats :math:`b` in the election :math:`a` left covers :math:`b`: i.e., for all :math:`c`, if :math:`c` is majority preferred to :math:`a`,  then :math:`c` majority preferred to :math:`b`. The winners are the set of candidates who are undefeated in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `dominators` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -420,20 +388,15 @@
         for c2 in candidates:
             if c1 != c2:
                 # check if c2 left covers  c1 but c1 does not left cover c2
                 if left_covers(dom, c2, c1)  and not left_covers(dom, c1, c2):
                     defeat.add_edge(c2, c1)
     return defeat
 
-uc_bordes_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Uncovered Set - Bordes",
-    properties = uc_fish_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_bordes(edata, curr_cands = None): 
     """Uncovered Set (Bordes version):  Given candidates :math:`a` and :math:`b`, say that :math:`a` Bordes covers :math:`b` if :math:`a` is majority preferred to :math:`b` and for all :math:`c`, if :math:`c` is majority preferred or tied with :math:`a`, then :math:`c` is majority preferred to or tied with :math:`b`. The winners are the set of candidates who are not Bordes covered in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has  `dominators` and `majority_prefers` methods. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -483,20 +446,15 @@
                 # check if c2 left covers  c1 
                 if left_covers(dom, c2, c1):
                     is_in_ucs = False
         if is_in_ucs:
             uc_set.append(c1)
     return list(sorted(uc_set))  
 
-uc_mckelvey_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Uncovered Set - McKelvey",
-    properties = uc_fish_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def uc_mckelvey(edata, curr_cands = None): 
     """Uncovered Set (McKelvey version):  Given candidates :math:`a` and :math:`b`, say that  :math:`a` McKelvey covers :math:`b` if a Gillies covers :math:`b` and :math:`a` Bordes covers :math:`b`. The winners are the set of candidates who are not McKelvey covered in the election restricted to ``curr_cands``. 
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has  `dominators` and `majority_prefers` methods. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -544,22 +502,15 @@
                 # check if c2 left covers  c1 
                 if left_covers(strict_dom, c2, c1) and left_covers(weak_dom, c2, c1):
                     is_in_ucs = False
         if is_in_ucs:
             uc_set.append(c1)
     return list(sorted(uc_set))      
 
-top_cycle_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Top Cycle",
-    properties = top_cycle_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def top_cycle(edata, curr_cands = None):
     """The smallest set of candidates such that every candidate inside the set is majority preferred to every candidate outside the set.  
     
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `majority_prefers` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -647,22 +598,15 @@
     candidates = edata.candidates if curr_cands is None else curr_cands
     smith_set = top_cycle(edata, curr_cands = candidates)
     
     defeat.add_nodes_from(candidates)
     defeat.add_edges_from([(a, b) for a in candidates for b in candidates if a != b and a in smith_set and b not in smith_set])
     return defeat
 
-gocha_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "GOCHA",
-    properties = gocha_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def gocha(edata, curr_cands = None):
     """The GOCHA set (also known as the Schwartz set) is the set of all candidates x such that if y can reach x in the transitive closer of the majority relation, then x can reach y in the transitive closer of the majority relation.
       
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `majority_prefers` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -734,20 +678,15 @@
                 return False
     return True
 
 def is_subsequence(x, y):
     it = iter(y)
     return all(any(c == ch for c in it) for ch in x)
 
-banks_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Banks",
-    properties = banks_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def banks(edata, curr_cands = None): 
     """ Say that a *chain* in majority graph is a subset of candidates that is linearly ordered by the majority relation. Then a candidate :math:`a` if :math:`a` is the maximum element with respect to the majority relation of some maximal chain in the majority graph.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -921,20 +860,15 @@
         if dist < min_dist: 
             min_dist = dist
             rankings = [lin_order]
         elif dist == min_dist: 
             rankings.append(lin_order)
     return rankings, min_dist
 
-slater_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Slater",
-    properties = slater_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def slater(edata, curr_cands = None): 
     """A Slater ranking is a linear order :math:`R` of the candidates that minimizes the number of edges in the majority graph we have to turn around before we obtain :math:`R`.   A candidate is a Slater winner if the candidate is the top element of some Slater ranking.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -968,20 +902,15 @@
         slater.display(mg)
 
     """    
     rankings, dist = slater_rankings(edata, curr_cands = curr_cands)
     
     return sorted(list(set([r[0] for r in rankings])))
 
-bipartisan_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,)
 @vm(name = "Bipartisan Set",
-    properties = bipartisan_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def bipartisan(edata, curr_cands = None, threshold = 0.0000001): 
     """The Bipartisan Set is the support of the (chosen) C1 maximal lottery.
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `margin_matrix` attribute.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
```

### Comparing `pref_voting-1.3.2/pref_voting/dominance_axioms.py` & `pref_voting-1.3.3/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/generate_profiles.py` & `pref_voting-1.3.3/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/generate_spatial_profiles.py` & `pref_voting-1.3.3/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/generate_utility_profiles.py` & `pref_voting-1.3.3/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-1.3.3/pref_voting/generate_weighted_majority_graphs.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,34 +25,31 @@
 
     .. note:: This function randomly generates a tournament with a linear order over the edges.  A **tournament** is an asymmetric directed graph with an edge between every two nodes.  The linear order of the edges is represented by assigning to each edge a number  :math:`2, \ldots, 2*n`, where :math:`n` is the number of the edges. 
     """
 
     assert parity in ["even", "odd"], "The parity should be either 'even' or 'odd'."
 
     mg = nx.DiGraph()
-    mg.add_nodes_from(list(range(num_cands)))
-    candidates = list(range(num_cands))
+    mg.add_nodes_from(range(num_cands))
     _edges = list()
-    for c1 in candidates: 
-        for c2 in candidates: 
-            if c1 != c2: 
-                if (c1, c2) not in _edges and (c2, c1) not in _edges:
-                    if np.random.choice([True, False]): 
-                        _edges.append((c1, c2))
-                    else: 
-                        _edges.append((c2, c1))
+    for c1 in range(num_cands): 
+        for c2 in range(c1+1, num_cands): 
+            if np.random.choice([True, False]): 
+                _edges.append((c1, c2))
+            else: 
+                _edges.append((c2, c1))
                    
     edges = list()
     edge_indices = list(range(len(_edges)))
     np.random.shuffle(edge_indices)
     
     for i, e_idx in enumerate(edge_indices):
         edges.append((_edges[e_idx][0], _edges[e_idx][1], 2 * (i+1) if parity == 'even' else 2 * i+1)) 
     
-    return MarginGraph(candidates, edges)
+    return MarginGraph(range(num_cands), edges)
 
 def generate_margin_graph(num_cands, weight_domain = None, parity = 'even'): 
     """Generate a random MarginGraph (allowing for ties in the margins) for ``num_cands`` candidates.  
 
     Args:
         num_cands (int): the number of candidates
```

### Comparing `pref_voting-1.3.2/pref_voting/grade_methods.py` & `pref_voting-1.3.3/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/grade_profiles.py` & `pref_voting-1.3.3/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/helper.py` & `pref_voting-1.3.3/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/invariance_axioms.py` & `pref_voting-1.3.3/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/io/readers.py` & `pref_voting-1.3.3/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/io/writers.py` & `pref_voting-1.3.3/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/iterative_methods.py` & `pref_voting-1.3.3/pref_voting/iterative_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pref_voting.margin_based_methods import split_cycle, minimax_scores
 from pref_voting.c1_methods import top_cycle, gocha
 from pref_voting.rankings import Ranking
 from pref_voting.social_welfare_function import swf
 import copy
 from itertools import permutations, product
 import numpy as np
-from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
+from pref_voting.voting_method_properties import ElectionTypes
 
 
 def _instant_runoff_basic(profile,curr_cands = None):
     "The basic implementation of instant runoff"
     # need the total number of all candidates in a profile to check when all candidates have been removed   
     num_cands = profile.num_cands 
     
@@ -63,22 +63,15 @@
 
     if len(lowest_first_place_votes) == len(candidates):
         return sorted(lowest_first_place_votes)
     
     else:
         return _instant_runoff_recursive(profile, [c for c in candidates if c not in lowest_first_place_votes])
 
-irv_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=True, 
-    positive_involvement=True,
-    )
 @vm(name = "Instant Runoff",
-    properties=irv_properties,
     input_types=[ElectionTypes.PROFILE])
 def instant_runoff(profile, curr_cands = None, algorithm = "basic"):
     """
     If there is a majority winner then that candidate is the winner. If there is no majority winner, then remove all candidates that are ranked first by the fewest number of voters. Continue removing candidates with the fewest number first-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
         If there is more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
@@ -165,21 +158,15 @@
         rec_ranking = instant_runoff_ranking(profile, [c for c in candidates if c not in lowest_first_place_votes])
         max_rank = max(rec_ranking.ranks)
         rec_ranking_dict = rec_ranking.rmap
         ranking = Ranking({c: rec_ranking_dict[c] if not isin(lowest_first_place_votes,c) else max_rank+1 for c in candidates})
 
         return ranking
 
-irv_tb_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=None,
-    pareto_dominance=True, 
-    )
 @vm(name = "Instant Runoff TB",
-    properties=irv_tb_properties,
     input_types=[ElectionTypes.PROFILE])
 def instant_runoff_tb(profile, curr_cands = None, tie_breaker = None):
     """Instant Runoff (``instant_runoff``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -240,22 +227,15 @@
             winners = sorted(lowest_first_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners)
 
-irv_put_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=None,
-    pareto_dominance=True, 
-    positive_involvement=True,
-    )
 @vm(name = "Instant Runoff PUT",
-    properties=irv_put_properties,
     input_types=[ElectionTypes.PROFILE])
 def instant_runoff_put(profile, curr_cands = None):
     """
     Instant Runoff (:func:`instant_runoff`) with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the IRV-PUT winner; otherwise a candidate x is an IRV-PUT winner if there is some candidate y with a minimal number of first-place votes such that after removing y from the profile, x is an IRV-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -411,21 +391,15 @@
             winners = sorted(lowest_first_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners), elims_list
 
-irv_truncated_lo_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=None, 
-    )
 @vm(name="Instant Runoff",
-    properties=irv_truncated_lo_properties,
     input_types=[ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def instant_runoff_for_truncated_linear_orders(profile, curr_cands = None, threshold = None, hide_warnings = True): 
     """
     Instant Runoff for Truncated Linear Orders.  Iteratively remove the candidates with the fewest number of first place votes, until there is a candidate with more than the threshold number of first-place votes. 
     If a threshold is not set, then it is strictly more than half of the non-empty ballots. 
     
     Args:
@@ -509,22 +483,15 @@
         
     pl_scores = reduced_prof.plurality_scores()
     
     max_pl_score = max(pl_scores.values())
     
     return sorted([c for c in pl_scores.keys() if pl_scores[c] == max_pl_score])
 
-bottom_two_runoff_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=False,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name="Bottom-Two-Runoff Instant Runoff",
-    properties=bottom_two_runoff_properties,
     input_types=[ElectionTypes.PROFILE])
 def bottom_two_runoff_instant_runoff(profile, curr_cands = None):
     """Find the two candidates with the lowest two plurality scores, remove the one who loses head-to-head to the other, and repeat until a single candidate remains. 
     
     If there is a tie for lowest or second lowest plurality score, consider all head-to-head matches between a candidate with lowest and a candidate with second lowest plurality score, and remove all the losers of the head-to-head matches, unless this would remove all candidates.
 
     .. note:: 
@@ -567,22 +534,15 @@
                     cands_to_remove.append(c2)
     
     if len(set(cands_to_remove)) == len(candidates):
         return candidates
     else:
         return bottom_two_runoff_instant_runoff(profile, [cand for cand in candidates if cand not in set(cands_to_remove)])
 
-bottom_two_runoff_put_properties = VotingMethodProperties(
-    condorcet_winner=None, 
-    condorcet_loser=False,
-    pareto_dominance=None, 
-    positive_involvement=False,
-    )
 @vm(name="Bottom-Two-Runoff Instant Runoff PUT",
-    properties=bottom_two_runoff_put_properties,
     input_types=[ElectionTypes.PROFILE])
 def bottom_two_runoff_instant_runoff_put(profile, curr_cands = None):
     """Find the two candidates with the lowest two plurality scores, remove the one who loses head-to-head to the other, and repeat until a single candidate remains. Parallel-universe tiebreaking is used to break ties for lowest or second lowest plurality scores. 
 
     .. note:: 
         BTR-IRV is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then BTR-IRV will elect the Condorcet winner. 
 
@@ -619,22 +579,15 @@
                     additional_winners = bottom_two_runoff_instant_runoff_put(profile, curr_cands = [c for c in candidates if not c == c2])
                 
                 winners = winners + additional_winners
     
     return sorted(set(winners))
     
 
-pl_w_runoff_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=True,
-    pareto_dominance=None, 
-    positive_involvement=True,
-    )
 @vm(name = "PluralityWRunoff PUT",
-    properties=pl_w_runoff_properties,
     input_types=[ElectionTypes.PROFILE])
 def plurality_with_runoff_put(profile, curr_cands = None):
     """If there is a majority winner then that candidate is the Plurality with Runoff winner. Otherwise hold a runoff between the top two candidates: the candidate with the most first place votes and the candidate with the 2nd most first place votes (or perhaps tied for the most first place votes). In the case of multiple candidates tied for the most or 2nd most first place votes, use parallel-universe tiebreaking: a candidate is a Plurality with Runoff winner if it is a winner in some runoff as described. If the candidates are all tied for the most first place votes, then all candidates are winners.
         
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -734,22 +687,15 @@
             winners.append(c2)
         elif profile.margin(c1,c2) == 0:
             winners.append(c1)
             winners.append(c2)
     
     return sorted(list(set(winners))), list(all_runoff_pairs)
 
-coombs_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Coombs",
-    properties=coombs_properties,
     input_types=[ElectionTypes.PROFILE])
 def coombs(profile, curr_cands = None):
     """If there is a majority winner then that candidate is the Coombs winner.   If there is no majority winner, then remove all candidates that are ranked last by the greatest number of voters.  Continue removing candidates with the most last-place votes until there is a candidate with a majority of first place votes.  
     
     .. important::
         If there is  more than one candidate with the largest number of last-place votes, then *all* such candidates are removed from the profile. 
     
@@ -807,22 +753,15 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners)
 
-coombs_tb_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=None,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Coombs TB",
-    properties=coombs_tb_properties,
     input_types=[ElectionTypes.PROFILE])
 def coombs_tb(profile, curr_cands = None, tie_breaker=None):
     """
     Coombs with a fixed tie-breaking rule: The tie-breaking rule is any linear order (i.e., list) of the candidates.  The default rule is to order the candidates as follows: 0,....,num_cands-1.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -885,22 +824,15 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners)
 
-coombs_put_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=None,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Coombs PUT",
-    properties=coombs_put_properties,
     input_types=[ElectionTypes.PROFILE])
 def coombs_put(profile, curr_cands = None):
     """Coombs with parallel universe tie-breaking (PUT), defined recursively: if there is a candidate with a strict majority of first-place votes, that candidate is the Coombs-PUT winner; otherwise a candidate x is a Coombs-PUT winner if there is some candidate y with a maximal number of last-place votes such that after removing y from the profile, x is a Coombs-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -1025,22 +957,15 @@
             winners = list(greatest_last_place_votes)
         else:
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     return sorted(winners), elims_list
 
-baldwin_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Baldwin",
-    properties=baldwin_properties,
     input_types=[ElectionTypes.PROFILE])
 def baldwin(profile, curr_cands = None):
     """Iteratively remove all candidates with the lowest Borda score until a single candidate remains.  If, at any stage, all  candidates have the same Borda score,  then all (remaining) candidates are winners.
 
     .. note:: 
         Baldwin is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Baldwin will elect the Condorcet winner. 
 
@@ -1100,22 +1025,15 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners)
 
-baldwin_tb_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Baldwin TB",
-    properties=coombs_tb_properties,
     input_types=[ElectionTypes.PROFILE])
 def baldwin_tb(profile, curr_cands = None, tie_breaker=None):
     """
     Baldwin with a fixed tie-breaking rule: The tie-breaking rule is any linear order (i.e., list) of the candidates.  The default rule is to order the candidates as follows: 0,....,num_cands-1.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -1191,22 +1109,15 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners)
 
-baldwin_put_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Baldwin PUT",
-    properties=baldwin_put_properties,
     input_types=[ElectionTypes.PROFILE])
 def baldwin_put(profile, curr_cands=None):
     """Baldwin with parallel universe tie-breaking (PUT), defined recursively: if there is a single candidate in the profile, that candidate wins; otherwise a candidate x is a Baldwin-PUT winner if there is some candidate y with a minimal Borda score such that after removing y from the profile, x is a Baldwin-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -1339,22 +1250,15 @@
             winners = sorted(last_place_borda_scores)
         elif num_cands - cands_to_ignore.shape[0] ==  1: # only one candidate remains
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else: 
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
     return sorted(winners), elims_list
 
-strict_nanson_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Strict Nanson",
-    properties=strict_nanson_properties,
     input_types=[ElectionTypes.PROFILE])
 def strict_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with the  Borda score strictly below the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
         
         Strict Nanson is a Condorcet consistent voting method, i.e., if a Condorcet winner exists, then Strict Nanson will elect the Condorcet winner. 
@@ -1490,22 +1394,15 @@
         if (len(below_borda_avg_candidates) == 0) or ((all_num_cands - cands_to_ignore.shape[0]) == 1):
             winners = sorted([c for c in candidates if c not in cands_to_ignore])
         else:
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners, elim_list
 
-weak_nanson_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=True,
-    pareto_dominance=True, 
-    positive_involvement=False,
-    )
 @vm(name = "Weak Nanson",
-    properties=weak_nanson_properties,
     input_types=[ElectionTypes.PROFILE])
 def weak_nanson(profile, curr_cands = None):
     """Iteratively remove all candidates with Borda score less than or equal the average Borda score until one candidate remains.  If, at any stage, all  candidates have the same Borda score, then all (remaining) candidates are winners.
 
     .. note:: 
 
         Weak Nanson is a Condorcet consistent voting method, i.e.,  if a Condorcet winner exists, then Weak Nanson will elect the Condorcet winner. 
@@ -1663,22 +1560,15 @@
             winners = [c for c in candidates if not isin(cands_to_ignore, c)]
         else:
             updated_rankings = _find_updated_profile(rankings, cands_to_ignore, num_cands)
             
     return winners, elim_list
 
 
-it_condorcet_loser_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=True,
-    pareto_dominance=False, 
-    positive_involvement=False,
-    )
 @vm(name = "Iterated Removal Condorcet Loser",
-    properties=it_condorcet_loser_properties,
     input_types=[ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MAJORITY_GRAPH, ElectionTypes.MARGIN_GRAPH])
 def iterated_removal_cl(edata, curr_cands = None):
     """
     Iteratively remove candidates that are Condorcet losers until there are no Condorcet losers.   A candidate :math:`c` is a **Condorcet loser** when every other candidate is majority preferred to :math:`c`. 
 
     Args:
         edata (Profile, ProfileWithTies, MajorityGraph, MarginGraph): Any election data that has a `condorcet_loser` method. 
@@ -1767,22 +1657,15 @@
     worst_m_score = min([m_scores[c] for c in curr_cands])
     worst_losers = [c for c in curr_cands if m_scores[c] == worst_m_score]
     if len(worst_losers) == len(curr_cands):
         return curr_cands
     else:
         return [c for c in curr_cands if c not in worst_losers]
 
-raynaud_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=False,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Raynaud",
-    properties=raynaud_properties,
     input_types=[ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES, ElectionTypes.MARGIN_GRAPH])
 def raynaud(edata, curr_cands=None, score_method = "margins"):
     """Iteratively remove the candidate(s) whose worst loss is biggest, unless all candidates have the same worst loss. See https://electowiki.org/wiki/Raynaud.
     
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``.
@@ -1794,22 +1677,15 @@
     candidates = edata.candidates if curr_cands is None else curr_cands
     new_cands = _remove_worst_losers(edata,candidates,score_method)
     while not new_cands == candidates:
         candidates = new_cands
         new_cands = _remove_worst_losers(edata,candidates,score_method)
     return sorted(candidates)
 
-benham_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=False,
-    pareto_dominance=True,
-    benham=False, 
-    )
 @vm(name = "Benham",
-    properties=benham_properties,
     input_types=[ElectionTypes.PROFILE])
 def benham(profile, curr_cands = None):
     """
     As long as the profile has no Condorcet winner, eliminate the candidate with the lowest plurality score.
     
     .. important::
         If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
@@ -1854,22 +1730,15 @@
         else:
             cw = profile.condorcet_winner([c for c in profile.candidates if not isin(cands_to_ignore, c)])
             if cw is not None: 
                 winners = [cw]
 
     return sorted(winners)
 
-benham_tb_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=None,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Benham TB",
-    properties=benham_tb_properties,
     input_types=[ElectionTypes.PROFILE])
 def benham_tb(profile, curr_cands = None, tie_breaker = None):
     """Benham (``benham``) with tie breaking:  If there is  more than one candidate with the fewest number of first-place votes, then remove the candidate with lowest in the tie_breaker ranking from the profile.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -1913,22 +1782,15 @@
         else:
             cw = profile.condorcet_winner(curr_cands = [c for c in profile.candidates if not isin(cands_to_ignore, c)])
             if cw is not None: 
                 winners = [cw]
     return sorted(winners)
 
 
-benham_tb_properties = VotingMethodProperties(
-    condorcet_winner=True, 
-    condorcet_loser=None,
-    pareto_dominance=True,
-    positive_involvement=False,
-    )
 @vm(name = "Benham PUT",
-    properties=benham_tb_properties,
     input_types=[ElectionTypes.PROFILE])
 def benham_put(profile, curr_cands = None):
     """Benham (:func:`benham`) with parallel universe tie-breaking (PUT), defined recursively: if there is a Condorcet winner, that candidate is the Benham-PUT winner; otherwise a candidate x is a Benham-PUT winner if there is some candidate y with minimal plurality score such that after removing y from the profile, x is a Benham-PUT winner.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -2009,32 +1871,20 @@
             return vm_ws
             
         else:
             return _ta(profile, curr_cands = [c for c in candidates if not c in cands_to_remove])
 
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name}")
 
-ta_smith_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 tideman_alternative_smith = tideman_alternative(top_cycle)
-tideman_alternative_smith.properties = ta_smith_properties
+tideman_alternative_smith.load_properties()
 tideman_alternative_smith.input_types = [ElectionTypes.PROFILE]
 
-ta_schwartz_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 tideman_alternative_schwartz = tideman_alternative(gocha)
-tideman_alternative_schwartz.properties = ta_schwartz_properties
+tideman_alternative_schwartz.load_properties()
 tideman_alternative_schwartz.input_types = [ElectionTypes.PROFILE]
 
 def tideman_alternative_put(vm):
     """Given a voting method vm, returns a voting method that restricts the profile to the set of vm winners, then eliminates the candidate with the fewest first-place votes, and then repeats until there is only one vm winner. Parallel-universe tiebreaking is used when there are multiple candidates with the fewest first-place votes.
 
     Args:
         vm (VotingMethod): A voting method.
@@ -2064,43 +1914,24 @@
                 winners = winners + additional_winners
 
         return sorted(set(winners))
 
     return VotingMethod(_ta, name=f"Tideman Alternative {vm.name} PUT")
 
 
-ta_smith_put_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 tideman_alternative_smith_put = tideman_alternative_put(top_cycle)
-tideman_alternative_smith_put.properties = ta_smith_put_properties
+tideman_alternative_smith_put.load_properties()
 tideman_alternative_smith_put.input_types = [ElectionTypes.PROFILE]
 
-ta_schwartz_put_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 tideman_alternative_schwartz_put = tideman_alternative_put(gocha)
-tideman_alternative_schwartz_put.properties = ta_schwartz_put_properties
+tideman_alternative_schwartz_put.load_properties()
 tideman_alternative_schwartz_put.input_types = [ElectionTypes.PROFILE]
 
 
-woodall_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Woodall",
-    properties=woodall_properties,
     input_types=[ElectionTypes.PROFILE])
 def woodall(profile, curr_cands = None):
     """
     If there is a single member of the Smith Set (i.e., a Condorcet winner) then that candidate is the winner.  If there the Smith Set contains more than one candidate, then remove all candidates that are ranked first by the fewest number of voters.  Continue removing candidates with the fewest number first-place votes until there is a single member of the originally Smith Set remaining.  
     
     .. important::
         If there is  more than one candidate with the fewest number of first-place votes, then *all* such candidates are removed from the profile. 
@@ -2154,22 +1985,15 @@
         if len(new_remaining_cands_in_smith_set) == 1:
             winners = new_remaining_cands_in_smith_set 
      
         cands_to_ignore = new_cands_to_ignore
 
     return sorted(winners)
 
-knockout_properties = VotingMethodProperties(
-    condorcet_winner=None,
-    condorcet_loser=None,
-    pareto_dominance=None,
-    positive_involvement=False,
-)
 @vm(name = "Knockout Voting",
-    properties=knockout_properties,
     input_types=[ElectionTypes.PROFILE])
 def knockout(profile, curr_cands=None):
     """Find the two candidates in curr_cands with the lowest and second lowest Borda scores among any candidates in curr_cands. Then remove from curr_cands whichever one loses to the other in a head-to-head majority comparison. Repeat this process, always using the original Borda score (i.e., the Borda scores calculated with respect to all candidates in the profile, not with respect to curr_cands as for Baldwin and Nanson) until only one candidate remains in curr_cands. Parallel universe tie-breaking (PUT) is used when there are ties in lowest or second lowest Borda scores.
 
     .. note::
         Proposed by Edward B. Foley (with unspecified handling of ties in Borda scores, so PUT is used here as an example).
```

### Comparing `pref_voting-1.3.2/pref_voting/maj_graph_ex1.png` & `pref_voting-1.3.3/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/mappings.py` & `pref_voting-1.3.3/pref_voting/mappings.py`

 * *Files 3% similar despite different names*

```diff
@@ -459,14 +459,40 @@
     def expectation(self, prob):
         """Return the expected utility given a probability distribution ``prob``."""
 
         assert all([x in self.domain for x in prob.keys()]), "The domain of the probability distribution must be a subset of the domain of the utility function."
 
         return sum([prob[x] * self.util(x) for x in self.domain if x in prob.keys() and self.has_utility(x)])
 
+    @classmethod
+    def from_linear_ranking(cls, ranking, seed=None):
+        """
+        Return a utility function that represents the linear ranking.
+
+        Parameters:
+        ranking (List[int]): A list representing the linear ranking.
+        seed (Optional[int]): An optional seed for random number generation.
+
+        Returns:
+        Utility: An instance of the Utility class.
+        """
+
+        if not (isinstance(ranking, list) or isinstance(ranking, tuple)):
+            raise ValueError("Ranking must be a list.")
+        if not len(set(ranking)) == len(ranking):
+            raise ValueError("Ranking must be a list of unique numbers.")
+
+        num_cands = len(ranking)
+        rng = np.random.default_rng(seed)
+        
+        utilities = sorted(rng.random(size=num_cands), reverse=True)
+        u_dict = {c: u for c, u in zip(ranking, utilities)}
+
+        return cls(u_dict)
+
     def __str__(self):
         return self.display_str("U")
 
 ######
 # Grade Functions
 ######
```

### Comparing `pref_voting-1.3.2/pref_voting/margin_based_methods.py` & `pref_voting-1.3.3/pref_voting/margin_based_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,4924 +35,4748 @@
 00000220: 2069 6d70 6f72 7420 7072 6f64 7563 742c   import product,
 00000230: 2070 6572 6d75 7461 7469 6f6e 732c 2063   permutations, c
 00000240: 6f6d 6269 6e61 7469 6f6e 732c 2063 6861  ombinations, cha
 00000250: 696e 0a69 6d70 6f72 7420 6e65 7477 6f72  in.import networ
 00000260: 6b78 2061 7320 6e78 0a66 726f 6d20 7072  kx as nx.from pr
 00000270: 6566 5f76 6f74 696e 672e 766f 7469 6e67  ef_voting.voting
 00000280: 5f6d 6574 686f 645f 7072 6f70 6572 7469  _method_properti
-00000290: 6573 2069 6d70 6f72 7420 566f 7469 6e67  es import Voting
-000002a0: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
-000002b0: 2c20 456c 6563 7469 6f6e 5479 7065 730a  , ElectionTypes.
-000002c0: 696d 706f 7274 206d 756c 7469 7072 6f63  import multiproc
-000002d0: 6573 7369 6e67 2061 7320 6d70 0a66 726f  essing as mp.fro
-000002e0: 6d20 6d75 6c74 6970 726f 6365 7373 696e  m multiprocessin
-000002f0: 6720 696d 706f 7274 2050 6f6f 6c0a 6672  g import Pool.fr
-00000300: 6f6d 2066 756e 6374 6f6f 6c73 2069 6d70  om functools imp
-00000310: 6f72 7420 7061 7274 6961 6c0a 0a6d 696e  ort partial..min
-00000320: 696d 6178 5f70 726f 7065 7274 6965 7320  imax_properties 
-00000330: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
-00000340: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
-00000350: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
-00000360: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
-00000370: 6365 745f 6c6f 7365 723d 4661 6c73 652c  cet_loser=False,
-00000380: 0a20 2020 2070 6172 6574 6f5f 646f 6d69  .    pareto_domi
-00000390: 6e61 6e63 653d 5472 7565 2c0a 2020 2020  nance=True,.    
-000003a0: 706f 7369 7469 7665 5f69 6e76 6f6c 7665  positive_involve
-000003b0: 6d65 6e74 3d54 7275 652c 200a 2020 2020  ment=True, .    
-000003c0: 290a 4076 6d28 6e61 6d65 203d 2022 4d69  ).@vm(name = "Mi
-000003d0: 6e69 6d61 7822 2c0a 2020 2020 7072 6f70  nimax",.    prop
-000003e0: 6572 7469 6573 3d6d 696e 696d 6178 5f70  erties=minimax_p
-000003f0: 726f 7065 7274 6965 732c 0a20 2020 2069  roperties,.    i
-00000400: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
-00000410: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
-00000420: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
-00000430: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
-00000440: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
-00000450: 732e 4d41 5247 494e 5f47 5241 5048 5d0a  s.MARGIN_GRAPH].
-00000460: 2020 2020 290a 6465 6620 6d69 6e69 6d61      ).def minima
-00000470: 7828 6564 6174 612c 2063 7572 725f 6361  x(edata, curr_ca
-00000480: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
-00000490: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-000004a0: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
-000004b0: 220a 2020 2020 5468 6520 4d69 6e69 6d61  ".    The Minima
-000004c0: 7820 7769 6e6e 6572 7320 6172 6520 7468  x winners are th
-000004d0: 6520 6361 6e64 6964 6174 6573 2077 6974  e candidates wit
-000004e0: 6820 7468 6520 736d 616c 6c65 7374 206d  h the smallest m
-000004f0: 6178 696d 756d 2070 6169 7277 6973 6520  aximum pairwise 
-00000500: 6c6f 7373 2e20 2054 6861 7420 6973 2c20  loss.  That is, 
-00000510: 666f 7220 6561 6368 2063 616e 6469 6461  for each candida
-00000520: 7465 203a 6d61 7468 3a60 6160 2c20 6669  te :math:`a`, fi
-00000530: 6e64 2074 6865 2062 6967 6765 7374 206d  nd the biggest m
-00000540: 6172 6769 6e20 6f66 2061 2063 616e 6469  argin of a candi
-00000550: 6461 7465 203a 6d61 7468 3a60 6260 206f  date :math:`b` o
-00000560: 7665 7220 3a6d 6174 683a 6061 602c 2074  ver :math:`a`, t
-00000570: 6865 6e20 656c 6563 7420 7468 6520 6361  hen elect the ca
-00000580: 6e64 6964 6174 6528 7329 2077 6974 6820  ndidate(s) with 
-00000590: 7468 6520 736d 616c 6c65 7374 2073 7563  the smallest suc
-000005a0: 6820 6c6f 7373 2e20 416c 736f 206b 6e6f  h loss. Also kno
-000005b0: 776e 2061 7320 7468 6520 5369 6d70 736f  wn as the Simpso
-000005c0: 6e2d 4b72 616d 6572 2052 756c 652e 0a20  n-Kramer Rule.. 
-000005d0: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
-000005e0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-000005f0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-00000600: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-00000610: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-00000620: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-00000630: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-00000640: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-00000650: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-00000660: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-00000670: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-00000680: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-00000690: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-000006a0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-000006b0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-000006c0: 7272 5f63 616e 6473 6060 0a0a 2020 2020  rr_cands``..    
-000006d0: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-000006e0: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-000006f0: 6f66 2063 616e 6469 6461 7465 730a 0a20  of candidates.. 
-00000700: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
-00000710: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-00000720: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00000730: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00000740: 2e6d 696e 696d 6178 5f73 636f 7265 7360  .minimax_scores`
-00000750: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
-00000760: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
-00000770: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
-00000780: 7861 6d70 6c65 732f 6d67 5f65 785f 6d69  xamples/mg_ex_mi
-00000790: 6e69 6d61 782e 7079 0a20 2020 2020 2020  nimax.py.       
-000007a0: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
-000007b0: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
-000007c0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
-000007d0: 0a0a 0a20 2020 202e 2e20 636f 6465 2d62  ...    .. code-b
-000007e0: 6c6f 636b 3a3a 200a 0a20 2020 2020 2020  lock:: ..       
-000007f0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00000800: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00000810: 6574 686f 6473 2069 6d70 6f72 7420 6d69  ethods import mi
-00000820: 6e69 6d61 780a 0a20 2020 2020 2020 206d  nimax..        m
-00000830: 696e 696d 6178 2e64 6973 706c 6179 2870  inimax.display(p
-00000840: 726f 6629 0a0a 0a20 2020 202e 2e20 6578  rof)...    .. ex
-00000850: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
-00000860: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
-00000870: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00000880: 665f 766f 7469 6e67 2e70 726f 6669 6c65  f_voting.profile
-00000890: 7320 696d 706f 7274 2050 726f 6669 6c65  s import Profile
-000008a0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
-000008b0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-000008c0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
-000008d0: 6d70 6f72 7420 6d69 6e69 6d61 780a 2020  mport minimax.  
-000008e0: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
-000008f0: 726f 6620 3d20 5072 6f66 696c 6528 5b5b  rof = Profile([[
-00000900: 332c 2030 2c20 312c 2032 5d2c 205b 312c  3, 0, 1, 2], [1,
-00000910: 2033 2c20 322c 2030 5d2c 205b 312c 2033   3, 2, 0], [1, 3
-00000920: 2c20 302c 2032 5d2c 205b 312c 2032 2c20  , 0, 2], [1, 2, 
-00000930: 302c 2033 5d2c 205b 332c 2032 2c20 302c  0, 3], [3, 2, 0,
-00000940: 2031 5d2c 205b 302c 2032 2c20 312c 2033   1], [0, 2, 1, 3
-00000950: 5d5d 2c20 5b31 2c20 312c 2031 2c20 312c  ]], [1, 1, 1, 1,
-00000960: 2032 2c20 315d 290a 0a20 2020 2020 2020   2, 1])..       
-00000970: 206d 696e 696d 6178 2e64 6973 706c 6179   minimax.display
-00000980: 2870 726f 6629 0a0a 2020 2020 2222 220a  (prof)..    """.
-00000990: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
-000009a0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
-000009b0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
-000009c0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
-000009d0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
-000009e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000009f0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
-00000a00: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
-00000a10: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
-00000a20: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
-00000a30: 6374 696f 6e0a 0a20 2020 2073 636f 7265  ction..    score
-00000a40: 7320 3d20 7b63 3a20 6d61 7828 5b73 7472  s = {c: max([str
-00000a50: 656e 6774 685f 6675 6e63 7469 6f6e 285f  ength_function(_
-00000a60: 632c 2063 2920 666f 7220 5f63 2069 6e20  c, c) for _c in 
-00000a70: 6564 6174 612e 646f 6d69 6e61 746f 7273  edata.dominators
-00000a80: 2863 2920 6966 205f 6320 696e 2063 616e  (c) if _c in can
-00000a90: 6469 6461 7465 735d 2920 6966 2061 6e79  didates]) if any
-00000aa0: 285b 5f63 2069 6e20 6564 6174 612e 646f  ([_c in edata.do
-00000ab0: 6d69 6e61 746f 7273 2863 2920 666f 7220  minators(c) for 
-00000ac0: 5f63 2069 6e20 6361 6e64 6964 6174 6573  _c in candidates
-00000ad0: 5d29 2065 6c73 6520 3020 0a20 2020 2020  ]) else 0 .     
-00000ae0: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
-00000af0: 6e20 6361 6e64 6964 6174 6573 7d0a 2020  n candidates}.  
-00000b00: 2020 6d69 6e5f 7363 6f72 6520 3d20 6d69    min_score = mi
-00000b10: 6e28 7363 6f72 6573 2e76 616c 7565 7328  n(scores.values(
-00000b20: 2929 0a20 2020 2072 6574 7572 6e20 736f  )).    return so
-00000b30: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
-00000b40: 2063 616e 6469 6461 7465 7320 6966 2073   candidates if s
-00000b50: 636f 7265 735b 635d 203d 3d20 6d69 6e5f  cores[c] == min_
-00000b60: 7363 6f72 655d 290a 0a0a 6465 6620 6d69  score])...def mi
-00000b70: 6e69 6d61 785f 7363 6f72 6573 2865 6461  nimax_scores(eda
-00000b80: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-00000b90: 204e 6f6e 652c 2073 636f 7265 5f6d 6574   None, score_met
-00000ba0: 686f 643d 226d 6172 6769 6e73 2229 3a0a  hod="margins"):.
-00000bb0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
-00000bc0: 6520 6d69 6e69 6d61 7820 7363 6f72 6573  e minimax scores
-00000bd0: 2066 6f72 2065 6163 6820 6361 6e64 6964   for each candid
-00000be0: 6174 652c 2077 6865 7265 2074 6865 206d  ate, where the m
-00000bf0: 696e 696d 6178 2073 636f 7265 2066 6f72  inimax score for
-00000c00: 203a 6d61 7468 3a60 6360 2069 7320 2d31   :math:`c` is -1
-00000c10: 202a 2074 6865 206d 6178 696d 756d 2070   * the maximum p
-00000c20: 6169 7277 6973 6520 6d61 6a6f 7269 7479  airwise majority
-00000c30: 206c 6f73 732e 200a 0a20 2020 2041 7267   loss. ..    Arg
-00000c40: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00000c50: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00000c60: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00000c70: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00000c80: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00000c90: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00000ca0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-00000cb0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00000cc0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00000cd0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00000ce0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00000cf0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00000d00: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00000d10: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00000d20: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00000d30: 2020 2020 2020 2020 7363 6f72 655f 6d65          score_me
-00000d40: 7468 6f64 2028 7374 722c 206f 7074 696f  thod (str, optio
-00000d50: 6e61 6c29 3a20 4f70 7469 6f6e 7320 696e  nal): Options in
-00000d60: 636c 7564 6520 226d 6172 6769 6e73 2220  clude "margins" 
-00000d70: 2874 6865 2064 6566 6175 6c74 292c 2022  (the default), "
-00000d80: 7769 6e6e 696e 6722 2061 7373 6967 6e73  winning" assigns
-00000d90: 2074 6f20 6561 6368 2063 616e 6469 6461   to each candida
-00000da0: 7465 203a 6d61 7468 3a60 6360 2074 6865  te :math:`c` the
-00000db0: 206d 6178 696d 756d 2073 7570 706f 7274   maximum support
-00000dc0: 206f 6620 6120 6361 6e64 6964 6174 6520   of a candidate 
-00000dd0: 6d61 6a6f 7269 7479 2070 7265 6665 7272  majority preferr
-00000de0: 6564 2074 6f20 3a6d 6174 683a 6063 602c  ed to :math:`c`,
-00000df0: 2020 616e 6420 2270 6169 7277 6973 655f    and "pairwise_
-00000e00: 6f70 706f 7369 7469 6f6e 2220 6173 7369  opposition" assi
-00000e10: 676e 7320 746f 2065 6163 6820 6361 6e64  gns to each cand
-00000e20: 6964 6174 6520 3a6d 6174 683a 6063 6020  idate :math:`c` 
-00000e30: 7468 6520 6d61 7869 6d75 6d20 7375 7070  the maximum supp
-00000e40: 6f72 7420 6f66 2061 6e79 2063 616e 6469  ort of any candi
-00000e50: 6461 7465 206f 7665 7220 3a6d 6174 683a  date over :math:
-00000e60: 6063 602e 2020 2054 6865 7365 2073 636f  `c`.   These sco
-00000e70: 7265 7320 6f6e 6c79 206c 6561 6420 746f  res only lead to
-00000e80: 2064 6966 6665 7265 6e74 2072 6573 756c   different resul
-00000e90: 7473 206f 6e20 6e6f 6e2d 6c69 6e65 6172  ts on non-linear
-00000ea0: 2070 726f 6669 6c65 732e 200a 0a20 2020   profiles. ..   
-00000eb0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-00000ec0: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
-00000ed0: 6173 736f 6369 6174 696e 6720 6561 6368  associating each
-00000ee0: 2063 616e 6469 6461 7465 2077 6974 6820   candidate with 
-00000ef0: 6974 7320 6d69 6e69 6d61 7820 7363 6f72  its minimax scor
-00000f00: 652e 0a0a 2020 2020 2e2e 2073 6565 616c  e...    .. seeal
-00000f10: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-00000f20: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-00000f30: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-00000f40: 7468 6f64 732e 6d69 6e69 6d61 7860 0a0a  thods.minimax`..
-00000f50: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
-00000f60: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
-00000f70: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
-00000f80: 6d70 6c65 732f 6d67 5f65 785f 6d69 6e69  mples/mg_ex_mini
-00000f90: 6d61 782e 7079 0a20 2020 2020 2020 203a  max.py.        :
-00000fa0: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
-00000fb0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
-00000fc0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
-00000fd0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
-00000fe0: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
-00000ff0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-00001000: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00001010: 686f 6473 2069 6d70 6f72 7420 6d69 6e69  hods import mini
-00001020: 6d61 785f 7363 6f72 6573 2c20 6d69 6e69  max_scores, mini
-00001030: 6d61 780a 0a20 2020 2020 2020 206d 696e  max..        min
-00001040: 696d 6178 2e64 6973 706c 6179 2870 726f  imax.display(pro
-00001050: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
-00001060: 286d 696e 696d 6178 5f73 636f 7265 7328  (minimax_scores(
-00001070: 7072 6f66 2929 0a0a 0a20 2020 202e 2e20  prof))...    .. 
-00001080: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
-00001090: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
-000010a0: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
-000010b0: 7265 665f 766f 7469 6e67 2e70 726f 6669  ref_voting.profi
-000010c0: 6c65 7320 696d 706f 7274 2050 726f 6669  les import Profi
-000010d0: 6c65 0a20 2020 2020 2020 2066 726f 6d20  le.        from 
-000010e0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-000010f0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00001100: 2069 6d70 6f72 7420 6d69 6e69 6d61 782c   import minimax,
-00001110: 206d 696e 696d 6178 5f73 636f 7265 730a   minimax_scores.
-00001120: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
-00001130: 2070 726f 6620 3d20 5072 6f66 696c 6528   prof = Profile(
-00001140: 5b5b 332c 2030 2c20 312c 2032 5d2c 205b  [[3, 0, 1, 2], [
-00001150: 312c 2033 2c20 322c 2030 5d2c 205b 312c  1, 3, 2, 0], [1,
-00001160: 2033 2c20 302c 2032 5d2c 205b 312c 2032   3, 0, 2], [1, 2
-00001170: 2c20 302c 2033 5d2c 205b 332c 2032 2c20  , 0, 3], [3, 2, 
-00001180: 302c 2031 5d2c 205b 302c 2032 2c20 312c  0, 1], [0, 2, 1,
-00001190: 2033 5d5d 2c20 5b31 2c20 312c 2031 2c20   3]], [1, 1, 1, 
-000011a0: 312c 2032 2c20 315d 290a 0a20 2020 2020  1, 2, 1])..     
-000011b0: 2020 206d 696e 696d 6178 2e64 6973 706c     minimax.displ
-000011c0: 6179 2870 726f 6629 0a20 2020 2020 2020  ay(prof).       
-000011d0: 2070 7269 6e74 286d 696e 696d 6178 5f73   print(minimax_s
-000011e0: 636f 7265 7328 7072 6f66 2929 0a0a 2020  cores(prof))..  
-000011f0: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
-00001200: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
-00001210: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
-00001220: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
-00001230: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
-00001240: 6473 0a0a 2020 2020 6966 206c 656e 2863  ds..    if len(c
-00001250: 616e 6469 6461 7465 7329 203d 3d20 313a  andidates) == 1:
-00001260: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001270: 7b63 3a20 3020 666f 7220 6320 696e 2063  {c: 0 for c in c
-00001280: 616e 6469 6461 7465 737d 0a20 2020 200a  andidates}.    .
-00001290: 2020 2020 2320 7468 6572 6520 6172 6520      # there are 
-000012a0: 6469 6666 6572 656e 7420 7363 6f72 696e  different scorin
-000012b0: 6720 6675 6e63 7469 6f6e 7320 7468 6174  g functions that
-000012c0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-000012d0: 6d65 6173 7572 6520 7468 6520 776f 7273  measure the wors
-000012e0: 6520 6c6f 7373 2066 6f72 2065 6163 6820  e loss for each 
-000012f0: 0a20 2020 2023 2063 616e 6469 6461 7465  .    # candidate
-00001300: 2e20 5468 6573 6520 616c 6c20 7072 6f64  . These all prod
-00001310: 7563 6520 7468 6520 7361 6d65 2073 6574  uce the same set
-00001320: 206f 6620 7769 6e6e 6572 7320 7768 656e   of winners when
-00001330: 2076 6f74 6572 7320 7375 626d 6974 206c   voters submit l
-00001340: 696e 6561 7220 6f72 6465 7273 2e20 0a20  inear orders. . 
-00001350: 2020 2073 636f 7265 5f66 756e 6374 696f     score_functio
-00001360: 6e73 203d 207b 0a20 2020 2020 2020 2022  ns = {.        "
-00001370: 7769 6e6e 696e 6722 3a20 6c61 6d62 6461  winning": lambda
-00001380: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
-00001390: 7461 2e73 7570 706f 7274 285f 632c 6329  ta.support(_c,c)
-000013a0: 2066 6f72 205f 6320 696e 2063 735d 2920   for _c in cs]) 
-000013b0: 6966 206c 656e 2863 7329 203e 2030 2065  if len(cs) > 0 e
-000013c0: 6c73 6520 302c 0a20 2020 2020 2020 2022  lse 0,.        "
-000013d0: 6d61 7267 696e 7322 3a20 6c61 6d62 6461  margins": lambda
-000013e0: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
-000013f0: 7461 2e6d 6172 6769 6e28 5f63 2c63 2920  ta.margin(_c,c) 
-00001400: 666f 7220 5f63 2069 6e20 6373 5d29 2069  for _c in cs]) i
-00001410: 6620 6c65 6e28 6373 2920 3e20 3020 656c  f len(cs) > 0 el
-00001420: 7365 2030 2c0a 2020 2020 2020 2020 2270  se 0,.        "p
-00001430: 6169 7277 6973 655f 6f70 706f 7369 7469  airwise_oppositi
-00001440: 6f6e 223a 206c 616d 6264 6120 6373 2c20  on": lambda cs, 
-00001450: 633a 206d 6178 285b 6564 6174 612e 7375  c: max([edata.su
-00001460: 7070 6f72 7428 5f63 2c63 2920 666f 7220  pport(_c,c) for 
-00001470: 5f63 2069 6e20 6373 5d29 0a20 2020 207d  _c in cs]).    }
-00001480: 200a 2020 2020 0a20 2020 2063 616e 6473   .    .    cands
-00001490: 203d 207b 0a20 2020 2020 2020 2022 7769   = {.        "wi
-000014a0: 6e6e 696e 6722 3a20 6c61 6d62 6461 2063  nning": lambda c
-000014b0: 3a20 6564 6174 612e 646f 6d69 6e61 746f  : edata.dominato
-000014c0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
-000014d0: 203d 2063 7572 725f 6361 6e64 7329 2c0a   = curr_cands),.
-000014e0: 2020 2020 2020 2020 226d 6172 6769 6e73          "margins
-000014f0: 223a 206c 616d 6264 6120 633a 2065 6461  ": lambda c: eda
-00001500: 7461 2e64 6f6d 696e 6174 6f72 7328 632c  ta.dominators(c,
-00001510: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00001520: 7272 5f63 616e 6473 292c 0a20 2020 2020  rr_cands),.     
-00001530: 2020 2022 7061 6972 7769 7365 5f6f 7070     "pairwise_opp
-00001540: 6f73 6974 696f 6e22 3a20 6c61 6d62 6461  osition": lambda
-00001550: 2063 3a20 5b5f 6320 666f 7220 5f63 2069   c: [_c for _c i
-00001560: 6e20 6361 6e64 6964 6174 6573 2069 6620  n candidates if 
-00001570: 5f63 2021 3d20 635d 0a20 2020 207d 200a  _c != c].    } .
-00001580: 0a20 2020 2072 6574 7572 6e20 7b63 3a20  .    return {c: 
-00001590: 2d31 202a 2073 636f 7265 5f66 756e 6374  -1 * score_funct
-000015a0: 696f 6e73 5b73 636f 7265 5f6d 6574 686f  ions[score_metho
-000015b0: 645d 2863 616e 6473 5b73 636f 7265 5f6d  d](cands[score_m
-000015c0: 6574 686f 645d 2863 292c 2063 2920 666f  ethod](c), c) fo
-000015d0: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
-000015e0: 737d 0a0a 0a64 6566 206d 6178 696d 616c  s}...def maximal
-000015f0: 5f65 6c65 6d65 6e74 7328 6729 3a20 0a20  _elements(g): . 
-00001600: 2020 2022 2222 7265 7475 726e 2074 6865     """return the
-00001610: 206e 6f64 6573 2069 6e20 6720 7769 7468   nodes in g with
-00001620: 206e 6f20 696e 636f 6d69 6e67 2061 7272   no incoming arr
-00001630: 6f77 732e 2222 220a 2020 2020 7265 7475  ows.""".    retu
-00001640: 726e 205b 6e20 666f 7220 6e20 696e 2067  rn [n for n in g
-00001650: 2e6e 6f64 6573 2069 6620 672e 696e 5f64  .nodes if g.in_d
-00001660: 6567 7265 6528 6e29 203d 3d20 305d 0a0a  egree(n) == 0]..
-00001670: 0a64 6566 205f 6265 6174 5f70 6174 685f  .def _beat_path_
-00001680: 6261 7369 6328 6564 6174 612c 200a 2020  basic(edata, .  
-00001690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016a0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-000016b0: 4e6f 6e65 2c20 0a20 2020 2020 2020 2020  None, .         
-000016c0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-000016d0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-000016e0: 4e6f 6e65 293a 200a 2020 2020 2222 2241  None): .    """A
-000016f0: 6e20 696d 706c 656d 656e 7461 7469 6f6e  n implementation
-00001700: 206f 6620 7468 6520 4265 6174 2050 6174   of the Beat Pat
-00001710: 6820 6d65 7468 6f64 2074 6861 7420 7573  h method that us
-00001720: 6573 2061 2062 6173 6963 2061 6c67 6f72  es a basic algor
-00001730: 6974 686d 2e20 2054 6869 7320 6973 206e  ithm.  This is n
-00001740: 6f74 2065 6666 6963 6965 6e74 2066 6f72  ot efficient for
-00001750: 206c 6172 6765 2067 7261 7068 732e 0a20   large graphs.. 
-00001760: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
-00001770: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-00001780: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-00001790: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-000017a0: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-000017b0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-000017c0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-000017d0: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
-000017e0: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
-000017f0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
-00001800: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
-00001810: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
-00001820: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
-00001830: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
-00001840: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
-00001850: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
-00001860: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-00001870: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
-00001880: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
-00001890: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
-000018a0: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
-000018b0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
-000018c0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
-000018d0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-000018e0: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
-000018f0: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
-00001900: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
-00001910: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
-00001920: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
-00001930: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
-00001940: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-00001950: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-00001960: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-00001970: 732e 200a 0a20 2020 2022 2222 0a20 2020  s. ..    """.   
-00001980: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
-00001990: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-000019a0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-000019b0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-000019c0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
-000019d0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-000019e0: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
-000019f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00001a00: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
-00001a10: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00001a20: 6e0a 2020 2020 0a20 2020 206d 6720 3d20  n.    .    mg = 
-00001a30: 6765 745f 6d67 2865 6461 7461 2c20 6375  get_mg(edata, cu
-00001a40: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
-00001a50: 6361 6e64 7329 0a20 2020 200a 2020 2020  cands).    .    
-00001a60: 6265 6174 5f70 6174 6873 5f77 6569 6768  beat_paths_weigh
-00001a70: 7473 203d 207b 633a 207b 6332 3a30 2066  ts = {c: {c2:0 f
-00001a80: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
-00001a90: 7465 7320 6966 2063 3220 213d 2063 7d20  tes if c2 != c} 
-00001aa0: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
-00001ab0: 7465 737d 0a20 2020 2066 6f72 2063 2069  tes}.    for c i
-00001ac0: 6e20 6361 6e64 6964 6174 6573 3a20 0a20  n candidates: . 
-00001ad0: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
-00001ae0: 5f63 2069 6e20 6265 6174 5f70 6174 6873  _c in beat_paths
-00001af0: 5f77 6569 6768 7473 5b63 5d2e 6b65 7973  _weights[c].keys
-00001b00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00001b10: 616c 6c5f 7061 7468 7320 3d20 206c 6973  all_paths =  lis
-00001b20: 7428 6e78 2e61 6c6c 5f73 696d 706c 655f  t(nx.all_simple_
-00001b30: 7061 7468 7328 6d67 2c20 632c 206f 7468  paths(mg, c, oth
-00001b40: 6572 5f63 2929 0a20 2020 2020 2020 2020  er_c)).         
-00001b50: 2020 2069 6620 6c65 6e28 616c 6c5f 7061     if len(all_pa
-00001b60: 7468 7329 203e 2030 3a0a 2020 2020 2020  ths) > 0:.      
-00001b70: 2020 2020 2020 2020 2020 6265 6174 5f70            beat_p
-00001b80: 6174 6873 5f77 6569 6768 7473 5b63 5d5b  aths_weights[c][
-00001b90: 6f74 6865 725f 635d 203d 206d 6178 285b  other_c] = max([
-00001ba0: 6d69 6e28 5b73 7472 656e 6774 685f 6675  min([strength_fu
-00001bb0: 6e63 7469 6f6e 2870 5b69 5d2c 2070 5b69  nction(p[i], p[i
-00001bc0: 2b31 5d29 200a 2020 2020 2020 2020 2020  +1]) .          
-00001bd0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
-00001be0: 616e 6765 2830 2c6c 656e 2870 292d 3129  ange(0,len(p)-1)
-00001bf0: 5d29 200a 2020 2020 2020 2020 2020 2020  ]) .            
-00001c00: 2020 2020 666f 7220 7020 696e 2061 6c6c      for p in all
-00001c10: 5f70 6174 6873 5d29 0a20 2020 200a 2020  _paths]).    .  
-00001c20: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
-00001c30: 2829 0a20 2020 2066 6f72 2063 2069 6e20  ().    for c in 
-00001c40: 6361 6e64 6964 6174 6573 3a20 0a20 2020  candidates: .   
-00001c50: 2020 2020 2069 6620 616c 6c28 5b62 6561       if all([bea
-00001c60: 745f 7061 7468 735f 7765 6967 6874 735b  t_paths_weights[
-00001c70: 635d 5b63 325d 203e 3d20 6265 6174 5f70  c][c2] >= beat_p
-00001c80: 6174 6873 5f77 6569 6768 7473 5b63 325d  aths_weights[c2]
-00001c90: 5b63 5d20 666f 7220 6332 2069 6e20 6361  [c] for c2 in ca
-00001ca0: 6e64 6964 6174 6573 2020 6966 2063 3220  ndidates  if c2 
-00001cb0: 213d 2063 5d29 3a0a 2020 2020 2020 2020  != c]):.        
-00001cc0: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
-00001cd0: 6e64 2863 290a 2020 2020 7265 7475 726e  nd(c).    return
-00001ce0: 2073 6f72 7465 6428 6c69 7374 2877 696e   sorted(list(win
-00001cf0: 6e65 7273 2929 0a0a 6465 6620 5f62 6561  ners))..def _bea
-00001d00: 745f 7061 7468 5f66 6c6f 7964 5f77 6172  t_path_floyd_war
-00001d10: 7368 616c 6c28 0a20 2020 2020 2020 2065  shall(.        e
-00001d20: 6461 7461 2c20 0a20 2020 2020 2020 2063  data, .        c
-00001d30: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
-00001d40: 2c20 0a20 2020 2020 2020 2073 7472 656e  , .        stren
-00001d50: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-00001d60: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-00001d70: 416e 2069 6d70 6c65 6d65 6e74 6174 696f  An implementatio
-00001d80: 6e20 6f66 2042 6561 7420 5061 7468 2075  n of Beat Path u
-00001d90: 7369 6e67 2061 2076 6172 6961 7469 6f6e  sing a variation
-00001da0: 206f 6620 7468 6520 466c 6f79 642d 5761   of the Floyd-Wa
-00001db0: 7273 6861 6c6c 2041 6c67 6f72 6974 686d  rshall Algorithm
-00001dc0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
-00001dd0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
-00001de0: 672f 7769 6b69 2f53 6368 756c 7a65 5f6d  g/wiki/Schulze_m
-00001df0: 6574 686f 6423 496d 706c 656d 656e 7461  ethod#Implementa
-00001e00: 7469 6f6e 290a 200a 2020 2020 4172 6773  tion). .    Args
-00001e10: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00001e20: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-00001e30: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-00001e40: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-00001e50: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-00001e60: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-00001e70: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-00001e80: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00001e90: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00001ea0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00001eb0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00001ec0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00001ed0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00001ee0: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00001ef0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00001f00: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00001f10: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00001f20: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-00001f30: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-00001f40: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-00001f50: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-00001f60: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-00001f70: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-00001f80: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00001f90: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00001fa0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00001fb0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00001fc0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00001fd0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00001fe0: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
-00001ff0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
-00002000: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
-00002010: 6461 7465 732e 200a 0a20 2020 2022 2222  dates. ..    """
-00002020: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
-00002030: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-00002040: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-00002050: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-00002060: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-00002070: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00002080: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-00002090: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-000020a0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-000020b0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-000020c0: 6e63 7469 6f6e 0a20 2020 2020 2020 200a  nction.        .
-000020d0: 2020 2020 735f 6d61 7472 6978 203d 205b      s_matrix = [
-000020e0: 5b2d 6e70 2e69 6e66 2066 6f72 205f 2069  [-np.inf for _ i
-000020f0: 6e20 6361 6e64 6964 6174 6573 5d20 666f  n candidates] fo
-00002100: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
-00002110: 735d 0a20 2020 2066 6f72 2063 315f 6964  s].    for c1_id
-00002120: 782c 2063 3120 696e 2065 6e75 6d65 7261  x, c1 in enumera
-00002130: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
-00002140: 2020 2020 2020 2020 666f 7220 6332 5f69          for c2_i
-00002150: 6478 2c20 6332 2069 6e20 656e 756d 6572  dx, c2 in enumer
-00002160: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-00002170: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002180: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
-00002190: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
-000021a0: 6f72 2063 3120 3d3d 2063 3229 3a0a 2020  or c1 == c2):.  
-000021b0: 2020 2020 2020 2020 2020 2020 2020 735f                s_
-000021c0: 6d61 7472 6978 5b63 315f 6964 785d 5b63  matrix[c1_idx][c
-000021d0: 325f 6964 785d 203d 2073 7472 656e 6774  2_idx] = strengt
-000021e0: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
-000021f0: 3229 200a 2020 2020 7374 7265 6e67 7468  2) .    strength
-00002200: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
-00002210: 6461 2069 203a 206c 6973 7428 6d61 7028  da i : list(map(
-00002220: 6c61 6d62 6461 206a 203a 206a 202c 2069  lambda j : j , i
-00002230: 2929 202c 2073 5f6d 6174 7269 7829 290a  )) , s_matrix)).
-00002240: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
-00002250: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00002260: 6e64 6964 6174 6573 293a 2020 2020 2020  ndidates):      
-00002270: 2020 200a 2020 2020 2020 2020 666f 7220     .        for 
-00002280: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
-00002290: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-000022a0: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
-000022b0: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
-000022c0: 2020 2020 2020 2020 2020 666f 7220 6b5f            for k_
-000022d0: 6964 782c 206b 2069 6e20 656e 756d 6572  idx, k in enumer
-000022e0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-000022f0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00002300: 2020 2020 2020 6966 2069 213d 206b 2061        if i!= k a
-00002310: 6e64 206a 2021 3d20 6b3a 0a20 2020 2020  nd j != k:.     
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
-00002340: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
-00002350: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
-00002360: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
-00002370: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
-00002380: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
-00002390: 785d 5b6b 5f69 6478 5d29 290a 2020 2020  x][k_idx])).    
-000023a0: 7769 6e6e 6572 7320 3d20 7b69 3a54 7275  winners = {i:Tru
-000023b0: 6520 666f 7220 6920 696e 2063 616e 6469  e for i in candi
-000023c0: 6461 7465 737d 0a20 2020 2066 6f72 2069  dates}.    for i
-000023d0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
-000023e0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-000023f0: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
-00002400: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
-00002410: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00002420: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00002430: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
-00002440: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
-00002450: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
-00002460: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
-00002470: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
-00002480: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00002490: 696e 6e65 7273 5b69 5d20 3d20 4661 6c73  inners[i] = Fals
-000024a0: 650a 2020 2020 7265 7475 726e 2073 6f72  e.    return sor
-000024b0: 7465 6428 5b63 2066 6f72 2063 2069 6e20  ted([c for c in 
-000024c0: 6361 6e64 6964 6174 6573 2069 6620 7769  candidates if wi
-000024d0: 6e6e 6572 735b 635d 5d29 0a0a 6465 6620  nners[c]])..def 
-000024e0: 5f73 6368 7761 7274 7a5f 7365 7175 656e  _schwartz_sequen
-000024f0: 7469 616c 5f64 726f 7070 696e 6728 6564  tial_dropping(ed
-00002500: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-00002510: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
-00002520: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-00002530: 293a 0a0a 2020 2020 2222 2254 6865 2053  ):..    """The S
-00002540: 6368 7761 7274 7a20 5365 7175 656e 7469  chwartz Sequenti
-00002550: 616c 2044 726f 7070 696e 6720 616c 676f  al Dropping algo
-00002560: 7269 7468 6d2e 2053 6565 2068 7474 7073  rithm. See https
-00002570: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
-00002580: 6f72 672f 7769 6b69 2f53 6368 756c 7a65  org/wiki/Schulze
-00002590: 5f6d 6574 686f 6423 5469 6573 5f61 6e64  _method#Ties_and
-000025a0: 5f61 6c74 6572 6e61 7469 7665 5f69 6d70  _alternative_imp
-000025b0: 6c65 6d65 6e74 6174 696f 6e73 2e0a 2020  lementations..  
-000025c0: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
-000025d0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-000025e0: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-000025f0: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00002600: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-00002610: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00002620: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00002630: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00002640: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00002650: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00002660: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00002670: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00002680: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00002690: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-000026a0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-000026b0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-000026c0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-000026d0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-000026e0: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-000026f0: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-00002700: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-00002710: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-00002720: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-00002730: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-00002740: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-00002750: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-00002760: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-00002770: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-00002780: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-00002790: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-000027a0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-000027b0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-000027c0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-000027d0: 2e20 0a20 2020 2022 2222 0a20 2020 2066  . .    """.    f
-000027e0: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
-000027f0: 6331 5f6d 6574 686f 6473 2069 6d70 6f72  c1_methods impor
-00002800: 7420 676f 6368 610a 0a20 2020 2073 7472  t gocha..    str
-00002810: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-00002820: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
-00002830: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00002840: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
-00002850: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00002860: 6e0a 0a20 2020 206d 6720 3d20 6564 6174  n..    mg = edat
-00002870: 6120 6966 2069 7369 6e73 7461 6e63 6528  a if isinstance(
-00002880: 6564 6174 612c 204d 6172 6769 6e47 7261  edata, MarginGra
-00002890: 7068 2920 656c 7365 2065 6461 7461 2e6d  ph) else edata.m
-000028a0: 6172 6769 6e5f 6772 6170 6828 290a 2020  argin_graph().  
-000028b0: 2020 7363 6877 6172 747a 203d 2067 6f63    schwartz = goc
-000028c0: 6861 286d 672c 2063 7572 725f 6361 6e64  ha(mg, curr_cand
-000028d0: 7320 3d20 6375 7272 5f63 616e 6473 290a  s = curr_cands).
-000028e0: 0a20 2020 2069 6620 6c65 6e28 7363 6877  .    if len(schw
-000028f0: 6172 747a 2920 3d3d 2031 3a0a 2020 2020  artz) == 1:.    
-00002900: 2020 2020 7265 7475 726e 2073 6368 7761      return schwa
-00002910: 7274 7a0a 2020 2020 0a20 2020 2070 6f73  rtz.    .    pos
-00002920: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
-00002930: 7468 7320 3d20 5b73 7472 656e 6774 685f  ths = [strength_
-00002940: 6675 6e63 7469 6f6e 2863 2c64 2920 666f  function(c,d) fo
-00002950: 7220 6320 696e 2073 6368 7761 7274 7a20  r c in schwartz 
-00002960: 666f 7220 6420 696e 2073 6368 7761 7274  for d in schwart
-00002970: 7a20 6966 2073 7472 656e 6774 685f 6675  z if strength_fu
-00002980: 6e63 7469 6f6e 2863 2c64 2920 3e20 305d  nction(c,d) > 0]
-00002990: 0a0a 2020 2020 6966 206c 656e 2870 6f73  ..    if len(pos
-000029a0: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
-000029b0: 7468 7329 203d 3d20 303a 0a20 2020 2020  ths) == 0:.     
-000029c0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-000029d0: 2873 6368 7761 7274 7a29 0a0a 2020 2020  (schwartz)..    
-000029e0: 6d61 785f 7363 6877 6172 747a 5f73 7472  max_schwartz_str
-000029f0: 656e 6774 6820 3d20 6d61 7828 706f 735f  ength = max(pos_
-00002a00: 7363 6877 6172 747a 5f73 7472 656e 6774  schwartz_strengt
-00002a10: 6873 290a 2020 2020 6d69 6e5f 7363 6877  hs).    min_schw
-00002a20: 6172 747a 5f73 7472 656e 6774 6820 3d20  artz_strength = 
-00002a30: 6d69 6e28 706f 735f 7363 6877 6172 747a  min(pos_schwartz
-00002a40: 5f73 7472 656e 6774 6873 290a 0a20 2020  _strengths)..   
-00002a50: 2069 6620 6d61 785f 7363 6877 6172 747a   if max_schwartz
-00002a60: 5f73 7472 656e 6774 6820 3d3d 206d 696e  _strength == min
-00002a70: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
-00002a80: 7468 3a0a 2020 2020 2020 2020 7265 7475  th:.        retu
-00002a90: 726e 2073 6f72 7465 6428 7363 6877 6172  rn sorted(schwar
-00002aa0: 747a 290a 2020 2020 0a20 2020 2065 6c73  tz).    .    els
-00002ab0: 653a 0a20 2020 2020 2020 206e 6577 5f6d  e:.        new_m
-00002ac0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
-00002ad0: 7363 6877 6172 747a 2c5b 2863 2c64 2c20  schwartz,[(c,d, 
-00002ae0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00002af0: 6e28 632c 6429 2920 666f 7220 6320 696e  n(c,d)) for c in
-00002b00: 2073 6368 7761 7274 7a20 666f 7220 6420   schwartz for d 
-00002b10: 696e 2073 6368 7761 7274 7a20 6966 2073  in schwartz if s
-00002b20: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00002b30: 2863 2c64 2920 3e20 6d69 6e5f 7363 6877  (c,d) > min_schw
-00002b40: 6172 747a 5f73 7472 656e 6774 685d 290a  artz_strength]).
-00002b50: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00002b60: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
-00002b70: 6961 6c5f 6472 6f70 7069 6e67 286e 6577  ial_dropping(new
-00002b80: 5f6d 672c 2073 6368 7761 7274 7a29 0a0a  _mg, schwartz)..
-00002b90: 6270 5f70 726f 7065 7274 6965 7320 3d20  bp_properties = 
-00002ba0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
-00002bb0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
-00002bc0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
-00002bd0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
-00002be0: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
-00002bf0: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
-00002c00: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
-00002c10: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
-00002c20: 743d 4661 6c73 652c 200a 2020 2020 290a  t=False, .    ).
-00002c30: 0a40 766d 286e 616d 653d 2242 6561 7420  .@vm(name="Beat 
-00002c40: 5061 7468 222c 0a20 2020 2070 726f 7065  Path",.    prope
-00002c50: 7274 6965 733d 6270 5f70 726f 7065 7274  rties=bp_propert
-00002c60: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
-00002c70: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
-00002c80: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
-00002c90: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-00002ca0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
-00002cb0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
-00002cc0: 494e 5f47 5241 5048 5d29 0a64 6566 2062  IN_GRAPH]).def b
-00002cd0: 6561 745f 7061 7468 280a 2020 2020 6564  eat_path(.    ed
-00002ce0: 6174 612c 200a 2020 2020 6375 7272 5f63  ata, .    curr_c
-00002cf0: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
-00002d00: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00002d10: 696f 6e20 3d20 4e6f 6e65 2c20 0a20 2020  ion = None, .   
-00002d20: 2061 6c67 6f72 6974 686d 203d 2027 666c   algorithm = 'fl
-00002d30: 6f79 645f 7761 7273 6861 6c6c 2729 3a20  oyd_warshall'): 
-00002d40: 200a 0a20 2020 2022 2222 466f 7220 6361   ..    """For ca
-00002d50: 6e64 6964 6174 6573 203a 6d61 7468 3a60  ndidates :math:`
-00002d60: 6160 2061 6e64 203a 6d61 7468 3a60 6260  a` and :math:`b`
-00002d70: 2c20 6120 2a2a 7061 7468 2a2a 2066 726f  , a **path** fro
-00002d80: 6d20 3a6d 6174 683a 6061 6020 746f 203a  m :math:`a` to :
-00002d90: 6d61 7468 3a60 6260 2069 7320 6120 7365  math:`b` is a se
-00002da0: 7175 656e 6365 200a 2020 2020 3a6d 6174  quence .    :mat
-00002db0: 683a 6078 5f31 2c20 5c6c 646f 7473 2c20  h:`x_1, \ldots, 
-00002dc0: 785f 6e60 206f 6620 6469 7374 696e 6374  x_n` of distinct
-00002dd0: 2063 616e 6469 6461 7465 7320 2077 6974   candidates  wit
-00002de0: 6820 203a 6d61 7468 3a60 785f 313d 6160  h  :math:`x_1=a`
-00002df0: 2061 6e64 203a 6d61 7468 3a60 785f 6e3d   and :math:`x_n=
-00002e00: 6260 2073 7563 6820 7468 6174 200a 2020  b` such that .  
-00002e10: 2020 666f 7220 3a6d 6174 683a 6031 5c6c    for :math:`1\l
-00002e20: 6571 206b 5c6c 6571 206e 2d31 602c 203a  eq k\leq n-1`, :
-00002e30: 6d61 7468 3a60 785f 6b60 2069 7320 6d61  math:`x_k` is ma
-00002e40: 6a6f 7269 7479 2070 7265 6665 7272 6564  jority preferred
-00002e50: 2074 6f20 3a6d 6174 683a 6078 5f7b 6b2b   to :math:`x_{k+
-00002e60: 317d 602e 2020 5468 6520 2a2a 7374 7265  1}`.  The **stre
-00002e70: 6e67 7468 206f 6620 6120 7061 7468 2a2a  ngth of a path**
-00002e80: 0a20 2020 2069 7320 7468 6520 6d69 6e69  .    is the mini
-00002e90: 6d61 6c20 6d61 7267 696e 2061 6c6f 6e67  mal margin along
-00002ea0: 2074 6861 7420 7061 7468 2e20 2053 6179   that path.  Say
-00002eb0: 2074 6861 7420 3a6d 6174 683a 6061 6020   that :math:`a` 
-00002ec0: 6465 6665 6174 7320 3a6d 6174 683a 6062  defeats :math:`b
-00002ed0: 6020 6163 636f 7264 696e 6720 746f 2042  ` according to B
-00002ee0: 6561 7420 5061 7468 2069 6620 7468 6520  eat Path if the 
-00002ef0: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-00002f00: 7468 6520 7374 726f 6e67 6573 7420 7061  the strongest pa
-00002f10: 7468 2066 726f 6d20 3a6d 6174 683a 6061  th from :math:`a
-00002f20: 6020 746f 203a 6d61 7468 3a60 6260 2069  ` to :math:`b` i
-00002f30: 7320 6772 6561 7465 7220 7468 616e 2074  s greater than t
-00002f40: 6865 2073 7472 656e 6774 6820 6f66 2074  he strength of t
-00002f50: 6865 2073 7472 6f6e 6765 7374 2070 6174  he strongest pat
-00002f60: 6820 6672 6f6d 203a 6d61 7468 3a60 6260  h from :math:`b`
-00002f70: 2074 6f20 3a6d 6174 683a 6061 602e 2054   to :math:`a`. T
-00002f80: 6865 6e20 7468 6520 6361 6e64 6964 6174  hen the candidat
-00002f90: 6573 2074 6861 7420 6172 6520 756e 6465  es that are unde
-00002fa0: 6665 6174 6564 2061 6363 6f72 6469 6e67  feated according
-00002fb0: 2074 6f20 4265 6174 2050 6174 6820 6172   to Beat Path ar
-00002fc0: 6520 7468 6520 7769 6e6e 6572 732e 2020  e the winners.  
-00002fd0: 416c 736f 206b 6e6f 776e 2061 7320 7468  Also known as th
-00002fe0: 6520 5363 6875 6c7a 6520 5275 6c65 2e20  e Schulze Rule. 
-00002ff0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00003000: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
-00003010: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
-00003020: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
-00003030: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
-00003040: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
-00003050: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
-00003060: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-00003070: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-00003080: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-00003090: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-000030a0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-000030b0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-000030c0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-000030d0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-000030e0: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
-000030f0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00003100: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
-00003110: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
-00003120: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
-00003130: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
-00003140: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
-00003150: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
-00003160: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-00003170: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
-00003180: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
-00003190: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
-000031a0: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
-000031b0: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
-000031c0: 6561 7220 6f72 6465 7273 2e20 0a20 2020  ear orders. .   
-000031d0: 2020 2020 2061 6c67 6f72 6974 686d 2028       algorithm (
-000031e0: 7374 7229 3a20 5370 6563 6966 7920 7768  str): Specify wh
-000031f0: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
-00003200: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
-00003210: 7265 2027 666c 6f79 645f 7761 7273 6861  re 'floyd_warsha
-00003220: 6c6c 2720 2874 6865 2064 6566 6175 6c74  ll' (the default
-00003230: 292c 2027 6261 7369 6327 2c20 616e 6420  ), 'basic', and 
-00003240: 2773 6368 7761 7274 7a5f 7365 7175 656e  'schwartz_sequen
-00003250: 7469 616c 5f64 726f 7070 696e 6727 2e0a  tial_dropping'..
-00003260: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-00003270: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
-00003280: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
-00003290: 6573 2e20 0a0a 2020 2020 2e2e 2073 6565  es. ..    .. see
-000032a0: 616c 736f 3a3a 0a0a 2020 2020 2020 2020  also::..        
-000032b0: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-000032c0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-000032d0: 6d65 7468 6f64 732e 6265 6174 5f70 6174  methods.beat_pat
-000032e0: 685f 6465 6665 6174 600a 0a20 2020 203a  h_defeat`..    :
-000032f0: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-00003300: 2e20 706c 6f74 3a3a 2020 6d61 7267 696e  . plot::  margin
-00003310: 5f67 7261 7068 735f 6578 616d 706c 6573  _graphs_examples
-00003320: 2f6d 675f 6578 5f62 705f 7270 2e70 790a  /mg_ex_bp_rp.py.
-00003330: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
-00003340: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
-00003350: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
-00003360: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
-00003370: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00003380: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00003390: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-000033a0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-000033b0: 706f 7274 2062 6561 745f 7061 7468 0a0a  port beat_path..
-000033c0: 2020 2020 2020 2020 6265 6174 5f70 6174          beat_pat
-000033d0: 682e 6469 7370 6c61 7928 6d67 290a 0a0a  h.display(mg)...
-000033e0: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
-000033f0: 3a3a 200a 2020 2020 2020 2020 3a68 6964  :: .        :hid
-00003400: 655f 636f 6465 3a0a 0a20 2020 2020 2020  e_code:..       
-00003410: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00003420: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
-00003430: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
-00003440: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
-00003450: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-00003460: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00003470: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-00003480: 7274 2062 6561 745f 7061 7468 0a20 2020  rt beat_path.   
-00003490: 2020 2020 200a 2020 2020 2020 2020 6d67       .        mg
-000034a0: 203d 204d 6172 6769 6e47 7261 7068 285b   = MarginGraph([
-000034b0: 302c 2031 2c20 322c 2033 5d2c 205b 2830  0, 1, 2, 3], [(0
-000034c0: 2c20 322c 2033 292c 2028 312c 2030 2c20  , 2, 3), (1, 0, 
-000034d0: 3529 2c20 2832 2c20 312c 2035 292c 2028  5), (2, 1, 5), (
-000034e0: 322c 2033 2c20 3129 2c20 2833 2c20 302c  2, 3, 1), (3, 0,
-000034f0: 2033 292c 2028 332c 2031 2c20 3129 5d29   3), (3, 1, 1)])
-00003500: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00003510: 2020 6265 6174 5f70 6174 682e 6469 7370    beat_path.disp
-00003520: 6c61 7928 6d67 290a 2020 2020 2020 2020  lay(mg).        
-00003530: 6265 6174 5f70 6174 682e 6469 7370 6c61  beat_path.displa
-00003540: 7928 6d67 2c20 616c 676f 7269 7468 6d3d  y(mg, algorithm=
-00003550: 2766 6c6f 7964 5f77 6172 7368 616c 6c27  'floyd_warshall'
-00003560: 2920 0a20 2020 2020 2020 2062 6561 745f  ) .        beat_
-00003570: 7061 7468 2e64 6973 706c 6179 286d 672c  path.display(mg,
-00003580: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
-00003590: 6327 290a 2020 2020 2222 220a 0a20 2020  c').    """..   
-000035a0: 2069 6620 616c 676f 7269 7468 6d20 3d3d   if algorithm ==
-000035b0: 2027 666c 6f79 645f 7761 7273 6861 6c6c   'floyd_warshall
-000035c0: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
-000035d0: 6e20 5f62 6561 745f 7061 7468 5f66 6c6f  n _beat_path_flo
-000035e0: 7964 5f77 6172 7368 616c 6c28 6564 6174  yd_warshall(edat
-000035f0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-00003600: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
-00003610: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00003620: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00003630: 6e29 0a20 2020 2065 6c69 6620 616c 676f  n).    elif algo
-00003640: 7269 7468 6d20 3d3d 2027 6261 7369 6327  rithm == 'basic'
-00003650: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00003660: 205f 6265 6174 5f70 6174 685f 6261 7369   _beat_path_basi
-00003670: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
-00003680: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00003690: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-000036a0: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
-000036b0: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
-000036c0: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
-000036d0: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
-000036e0: 6961 6c5f 6472 6f70 7069 6e67 273a 0a20  ial_dropping':. 
-000036f0: 2020 2020 2020 2072 6574 7572 6e20 5f73         return _s
-00003700: 6368 7761 7274 7a5f 7365 7175 656e 7469  chwartz_sequenti
-00003710: 616c 5f64 726f 7070 696e 6728 6564 6174  al_dropping(edat
-00003720: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-00003730: 6375 7272 5f63 616e 6473 2c20 7374 7265  curr_cands, stre
-00003740: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00003750: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00003760: 6e29 0a20 2020 2065 6c73 653a 0a20 2020  n).    else:.   
-00003770: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00003780: 4572 726f 7228 2249 6e76 616c 6964 2061  Error("Invalid a
-00003790: 6c67 6f72 6974 686d 2073 7065 6369 6669  lgorithm specifi
-000037a0: 6564 2e22 290a 0a64 6566 2062 6561 745f  ed.")..def beat_
-000037b0: 7061 7468 5f64 6566 6561 7428 6564 6174  path_defeat(edat
-000037c0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-000037d0: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
-000037e0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-000037f0: 2020 200a 2020 2020 2222 2252 6574 7572     .    """Retur
-00003800: 6e73 2074 6865 2064 6566 6561 7420 7265  ns the defeat re
-00003810: 6c61 7469 6f6e 2066 6f72 2042 6561 7420  lation for Beat 
-00003820: 5061 7468 2e20 0a20 2020 200a 2020 2020  Path. .    .    
-00003830: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00003840: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00003850: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00003860: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00003870: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00003880: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00003890: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-000038a0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-000038b0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-000038c0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-000038d0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-000038e0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-000038f0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-00003900: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-00003910: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-00003920: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-00003930: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-00003940: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-00003950: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-00003960: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-00003970: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00003980: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-00003990: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-000039a0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-000039b0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-000039c0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-000039d0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-000039e0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-000039f0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-00003a00: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-00003a10: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-00003a20: 6e65 7477 6f72 6b78 2044 6947 7261 7068  networkx DiGraph
-00003a30: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
-00003a40: 6520 4265 6174 2050 6174 6820 6465 6665  e Beat Path defe
-00003a50: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
-00003a60: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
-00003a70: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-00003a80: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00003a90: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00003aa0: 2e62 6561 745f 7061 7468 602c 203a 6d65  .beat_path`, :me
-00003ab0: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-00003ac0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00003ad0: 686f 6473 2e62 6561 745f 7061 7468 5f46  hods.beat_path_F
-00003ae0: 6c6f 7964 5f57 6172 7368 616c 6c60 0a0a  loyd_Warshall`..
-00003af0: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
-00003b00: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
-00003b10: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
-00003b20: 6d70 6c65 732f 6d67 5f65 785f 6270 5f64  mples/mg_ex_bp_d
-00003b30: 6566 6561 742e 7079 0a20 2020 2020 2020  efeat.py.       
-00003b40: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
-00003b50: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
-00003b60: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
-00003b70: 0a0a 2020 2020 2222 220a 0a20 2020 2063  ..    """..    c
-00003b80: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
-00003b90: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
-00003ba0: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
-00003bb0: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
-00003bc0: 6473 2020 2020 0a20 2020 2073 7472 656e  ds    .    stren
-00003bd0: 6774 685f 6675 6e63 7469 6f6e 203d 2065  gth_function = e
-00003be0: 6461 7461 2e6d 6172 6769 6e20 6966 2073  data.margin if s
-00003bf0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00003c00: 2069 7320 4e6f 6e65 2065 6c73 6520 7374   is None else st
-00003c10: 7265 6e67 7468 5f66 756e 6374 696f 6e0a  rength_function.
-00003c20: 2020 2020 2020 2020 0a20 2020 2073 5f6d          .    s_m
-00003c30: 6174 7269 7820 3d20 5b5b 2d6e 702e 696e  atrix = [[-np.in
-00003c40: 6620 666f 7220 5f20 696e 2063 616e 6469  f for _ in candi
-00003c50: 6461 7465 735d 2066 6f72 205f 2069 6e20  dates] for _ in 
-00003c60: 6361 6e64 6964 6174 6573 5d0a 2020 2020  candidates].    
-00003c70: 666f 7220 6331 5f69 6478 2c20 6331 2069  for c1_idx, c1 i
-00003c80: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00003c90: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-00003ca0: 2066 6f72 2063 325f 6964 782c 2063 3220   for c2_idx, c2 
-00003cb0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-00003cc0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-00003cd0: 2020 2020 2020 6966 2028 6564 6174 612e        if (edata.
-00003ce0: 6d61 6a6f 7269 7479 5f70 7265 6665 7273  majority_prefers
-00003cf0: 2863 312c 2063 3229 206f 7220 6331 203d  (c1, c2) or c1 =
-00003d00: 3d20 6332 293a 0a20 2020 2020 2020 2020  = c2):.         
-00003d10: 2020 2020 2020 2073 5f6d 6174 7269 785b         s_matrix[
-00003d20: 6331 5f69 6478 5d5b 6332 5f69 6478 5d20  c1_idx][c2_idx] 
-00003d30: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
-00003d40: 696f 6e28 6331 2c20 6332 2920 0a20 2020  ion(c1, c2) .   
-00003d50: 2073 7472 656e 6774 6820 3d20 6c69 7374   strength = list
-00003d60: 286d 6170 286c 616d 6264 6120 6920 3a20  (map(lambda i : 
-00003d70: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
-00003d80: 6a20 3a20 6a20 2c20 6929 2920 2c20 735f  j : j , i)) , s_
-00003d90: 6d61 7472 6978 2929 0a20 2020 2066 6f72  matrix)).    for
-00003da0: 2069 5f69 6478 2c20 6920 696e 2065 6e75   i_idx, i in enu
-00003db0: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00003dc0: 7329 3a20 2020 2020 2020 2020 0a20 2020  s):         .   
-00003dd0: 2020 2020 2066 6f72 206a 5f69 6478 2c20       for j_idx, 
-00003de0: 6a20 696e 2065 6e75 6d65 7261 7465 2863  j in enumerate(c
-00003df0: 616e 6469 6461 7465 7329 3a20 0a20 2020  andidates): .   
-00003e00: 2020 2020 2020 2020 2069 6620 6921 3d20           if i!= 
-00003e10: 6a3a 0a20 2020 2020 2020 2020 2020 2020  j:.             
-00003e20: 2020 2066 6f72 206b 5f69 6478 2c20 6b20     for k_idx, k 
-00003e30: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-00003e40: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
-00003e50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003e60: 6620 6921 3d20 6b20 616e 6420 6a20 213d  f i!= k and j !=
-00003e70: 206b 3a0a 2020 2020 2020 2020 2020 2020   k:.            
-00003e80: 2020 2020 2020 2020 2020 2020 7374 7265              stre
-00003e90: 6e67 7468 5b6a 5f69 6478 5d5b 6b5f 6964  ngth[j_idx][k_id
-00003ea0: 785d 203d 206d 6178 2873 7472 656e 6774  x] = max(strengt
-00003eb0: 685b 6a5f 6964 785d 5b6b 5f69 6478 5d2c  h[j_idx][k_idx],
-00003ec0: 206d 696e 2873 7472 656e 6774 685b 6a5f   min(strength[j_
-00003ed0: 6964 785d 5b69 5f69 6478 5d2c 7374 7265  idx][i_idx],stre
-00003ee0: 6e67 7468 5b69 5f69 6478 5d5b 6b5f 6964  ngth[i_idx][k_id
-00003ef0: 785d 2929 0a0a 2020 2020 6465 6665 6174  x]))..    defeat
-00003f00: 5f67 7261 7068 203d 206e 782e 4469 4772  _graph = nx.DiGr
-00003f10: 6170 6828 290a 2020 2020 6465 6665 6174  aph().    defeat
-00003f20: 5f67 7261 7068 2e61 6464 5f6e 6f64 6573  _graph.add_nodes
-00003f30: 5f66 726f 6d28 6361 6e64 6964 6174 6573  _from(candidates
-00003f40: 290a 2020 2020 0a20 2020 2066 6f72 2069  ).    .    for i
-00003f50: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
-00003f60: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00003f70: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
-00003f80: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
-00003f90: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00003fa0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00003fb0: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
-00003fc0: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
-00003fd0: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
-00003fe0: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
-00003ff0: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
-00004000: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004010: 6566 6561 745f 6772 6170 682e 6164 645f  efeat_graph.add_
-00004020: 7765 6967 6874 6564 5f65 6467 6573 5f66  weighted_edges_f
-00004030: 726f 6d28 5b28 6a2c 692c 735f 6d61 7472  rom([(j,i,s_matr
-00004040: 6978 5b6a 5f69 6478 5d5b 695f 6964 785d  ix[j_idx][i_idx]
-00004050: 295d 290a 0a20 2020 2072 6574 7572 6e20  )])..    return 
-00004060: 6465 6665 6174 5f67 7261 7068 0a0a 0a0a  defeat_graph....
-00004070: 6465 6620 6861 735f 7374 726f 6e67 5f70  def has_strong_p
-00004080: 6174 6828 412c 2073 6f75 7263 652c 2074  ath(A, source, t
-00004090: 6172 6765 742c 206b 293a 0a20 2020 2022  arget, k):.    "
-000040a0: 2222 4769 7665 6e20 6120 7371 7561 7265  ""Given a square
-000040b0: 206d 6174 7269 7820 412c 2072 6574 7572   matrix A, retur
-000040c0: 6e20 5472 7565 2069 6620 7468 6572 6520  n True if there 
-000040d0: 6973 2061 2070 6174 6820 6672 6f6d 2073  is a path from s
-000040e0: 6f75 7263 6520 746f 2074 6172 6765 7420  ource to target 
-000040f0: 696e 2074 6865 2061 7373 6f63 6961 7465  in the associate
-00004100: 6420 6469 7265 6374 6564 2067 7261 7068  d directed graph
-00004110: 2020 2020 2077 6865 7265 2065 6163 6820       where each 
-00004120: 6564 6765 2068 6173 2061 2077 6569 6768  edge has a weigh
-00004130: 7420 6772 6561 7465 7220 7468 616e 206f  t greater than o
-00004140: 7220 6571 7561 6c20 746f 206b 2c20 616e  r equal to k, an
-00004150: 6420 4661 6c73 6520 6f74 6865 7277 6973  d False otherwis
-00004160: 652e 2222 220a 2020 2020 0a20 2020 206e  e.""".    .    n
-00004170: 203d 2041 2e73 6861 7065 5b30 5d20 2320   = A.shape[0] # 
-00004180: 6173 7375 6d65 2041 2069 7320 6120 7371  assume A is a sq
-00004190: 7561 7265 206d 6174 7269 780a 2020 2020  uare matrix.    
-000041a0: 7669 7369 7465 6420 3d20 6e70 2e7a 6572  visited = np.zer
-000041b0: 6f73 286e 2c20 6474 7970 653d 626f 6f6c  os(n, dtype=bool
-000041c0: 290a 0a20 2020 2064 6566 2064 6673 286e  )..    def dfs(n
-000041d0: 6f64 6529 3a0a 2020 2020 2020 2020 6966  ode):.        if
-000041e0: 206e 6f64 6520 3d3d 2074 6172 6765 743a   node == target:
-000041f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00004200: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
-00004210: 2076 6973 6974 6564 5b6e 6f64 655d 203d   visited[node] =
-00004220: 2054 7275 650a 2020 2020 2020 2020 666f   True.        fo
-00004230: 7220 6e65 6967 6862 6f72 2c20 7765 6967  r neighbor, weig
-00004240: 6874 2069 6e20 656e 756d 6572 6174 6528  ht in enumerate(
-00004250: 415b 6e6f 6465 2c20 3a5d 293a 0a20 2020  A[node, :]):.   
-00004260: 2020 2020 2020 2020 2069 6620 415b 6e6f           if A[no
-00004270: 6465 5d5b 6e65 6967 6862 6f72 5d20 3e20  de][neighbor] > 
-00004280: 415b 6e65 6967 6862 6f72 5d5b 6e6f 6465  A[neighbor][node
-00004290: 5d20 616e 6420 7765 6967 6874 203e 3d20  ] and weight >= 
-000042a0: 6b20 616e 6420 6e6f 7420 7669 7369 7465  k and not visite
-000042b0: 645b 6e65 6967 6862 6f72 5d3a 0a20 2020  d[neighbor]:.   
-000042c0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000042d0: 6466 7328 6e65 6967 6862 6f72 293a 0a20  dfs(neighbor):. 
-000042e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000042f0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00004300: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00004310: 6c73 650a 0a20 2020 2072 6574 7572 6e20  lse..    return 
-00004320: 6466 7328 736f 7572 6365 290a 0a64 6566  dfs(source)..def
-00004330: 205f 7370 6c69 745f 6379 636c 655f 6261   _split_cycle_ba
-00004340: 7369 6328 0a20 2020 2020 2020 2065 6461  sic(.        eda
-00004350: 7461 2c20 0a20 2020 2020 2020 2063 7572  ta, .        cur
-00004360: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
-00004370: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-00004380: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-00004390: 6529 3a0a 2020 2020 2222 2241 6e20 696d  e):.    """An im
-000043a0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
-000043b0: 5370 6c69 7420 4379 636c 6520 6261 7365  Split Cycle base
-000043c0: 6420 6f6e 2074 6865 206d 6174 6865 6d61  d on the mathema
-000043d0: 7469 6361 6c20 6465 6669 6e69 7469 6f6e  tical definition
-000043e0: 2e20 2020 0a20 2020 2022 2222 0a20 2020  .   .    """.   
-000043f0: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
-00004400: 2c20 6361 6e64 5f74 6f5f 6369 6e64 6578  , cand_to_cindex
-00004410: 203d 2065 6461 7461 2e73 7472 656e 6774   = edata.strengt
-00004420: 685f 6d61 7472 6978 2863 7572 725f 6361  h_matrix(curr_ca
-00004430: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00004440: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-00004450: 696f 6e3d 7374 7265 6e67 7468 5f66 756e  ion=strength_fun
-00004460: 6374 696f 6e29 0a0a 2020 2020 6361 6e64  ction)..    cand
-00004470: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
-00004480: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-00004490: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-000044a0: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
-000044b0: 200a 0a20 2020 2073 7472 656e 6774 685f   ..    strength_
-000044c0: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
-000044d0: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
-000044e0: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
-000044f0: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
-00004500: 7468 5f66 756e 6374 696f 6e20 0a0a 2020  th_function ..  
-00004510: 2020 706f 7465 6e74 6961 6c5f 7769 6e6e    potential_winn
-00004520: 6572 7320 3d20 7365 7428 6361 6e64 6964  ers = set(candid
-00004530: 6174 6573 290a 0a20 2020 2066 6f72 2061  ates)..    for a
-00004540: 2069 6e20 6361 6e64 6964 6174 6573 3a0a   in candidates:.
-00004550: 2020 2020 2020 2020 666f 7220 6220 696e          for b in
-00004560: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
-00004570: 2020 2020 2020 2020 2069 6620 7374 7265           if stre
-00004580: 6e67 7468 5f66 756e 6374 696f 6e28 622c  ngth_function(b,
-00004590: 2061 2920 3e20 7374 7265 6e67 7468 5f66   a) > strength_f
-000045a0: 756e 6374 696f 6e28 612c 2062 2920 616e  unction(a, b) an
-000045b0: 6420 6e6f 7420 6861 735f 7374 726f 6e67  d not has_strong
-000045c0: 5f70 6174 6828 7374 7265 6e67 7468 5f6d  _path(strength_m
-000045d0: 6174 7269 782c 2063 616e 645f 746f 5f63  atrix, cand_to_c
-000045e0: 696e 6465 7828 6129 2c20 6361 6e64 5f74  index(a), cand_t
-000045f0: 6f5f 6369 6e64 6578 2862 292c 2073 7472  o_cindex(b), str
-00004600: 656e 6774 685f 6675 6e63 7469 6f6e 2862  ength_function(b
-00004610: 2c61 2929 3a0a 2020 2020 2020 2020 2020  ,a)):.          
-00004620: 2020 2020 2020 706f 7465 6e74 6961 6c5f        potential_
-00004630: 7769 6e6e 6572 732e 6469 7363 6172 6428  winners.discard(
-00004640: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
-00004650: 2020 2062 7265 616b 0a0a 2020 2020 7265     break..    re
-00004660: 7475 726e 2073 6f72 7465 6428 706f 7465  turn sorted(pote
-00004670: 6e74 6961 6c5f 7769 6e6e 6572 7329 0a0a  ntial_winners)..
-00004680: 6465 6620 5f69 735f 6361 6e64 5f73 706c  def _is_cand_spl
-00004690: 6974 5f63 7963 6c65 5f64 6566 6561 7465  it_cycle_defeate
-000046a0: 6428 612c 2073 7472 656e 6774 685f 6d61  d(a, strength_ma
-000046b0: 7472 6978 293a 0a0a 2020 2020 666f 7220  trix):..    for 
-000046c0: 6220 696e 2072 616e 6765 2873 7472 656e  b in range(stren
-000046d0: 6774 685f 6d61 7472 6978 2e73 6861 7065  gth_matrix.shape
-000046e0: 5b30 5d29 3a0a 2020 2020 2020 2020 6966  [0]):.        if
-000046f0: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
-00004700: 5b62 5d5b 615d 203e 2073 7472 656e 6774  [b][a] > strengt
-00004710: 685f 6d61 7472 6978 5b61 5d5b 625d 2061  h_matrix[a][b] a
-00004720: 6e64 206e 6f74 2068 6173 5f73 7472 6f6e  nd not has_stron
-00004730: 675f 7061 7468 2873 7472 656e 6774 685f  g_path(strength_
-00004740: 6d61 7472 6978 2c20 612c 2020 622c 2073  matrix, a,  b, s
-00004750: 7472 656e 6774 685f 6d61 7472 6978 5b62  trength_matrix[b
-00004760: 5d5b 615d 293a 0a20 2020 2020 2020 2020  ][a]):.         
-00004770: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00004780: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00004790: 0a0a 6465 6620 6261 7463 6828 6974 6572  ..def batch(iter
-000047a0: 6162 6c65 2c20 6e3d 3129 3a0a 2020 2020  able, n=1):.    
-000047b0: 6c20 3d20 6c65 6e28 6974 6572 6162 6c65  l = len(iterable
-000047c0: 290a 2020 2020 666f 7220 6e64 7820 696e  ).    for ndx in
-000047d0: 2072 616e 6765 2830 2c20 6c2c 206e 293a   range(0, l, n):
-000047e0: 0a20 2020 2020 2020 2079 6965 6c64 2069  .        yield i
-000047f0: 7465 7261 626c 655b 6e64 783a 6d69 6e28  terable[ndx:min(
-00004800: 6e64 7820 2b20 6e2c 206c 295d 0a0a 6465  ndx + n, l)]..de
-00004810: 6620 7072 6f63 6573 735f 6261 7463 685f  f process_batch_
-00004820: 6f66 5f63 616e 6469 6461 7465 7328 6261  of_candidates(ba
-00004830: 7463 682c 2073 7472 656e 6774 685f 6d61  tch, strength_ma
-00004840: 7472 6978 293a 0a20 2020 2072 6573 756c  trix):.    resul
-00004850: 7473 203d 205b 5d0a 2020 2020 666f 7220  ts = [].    for 
-00004860: 6361 6e64 6964 6174 6520 696e 2062 6174  candidate in bat
-00004870: 6368 3a0a 2020 2020 2020 2020 7265 7375  ch:.        resu
-00004880: 6c74 203d 205f 6973 5f63 616e 645f 7370  lt = _is_cand_sp
-00004890: 6c69 745f 6379 636c 655f 6465 6665 6174  lit_cycle_defeat
-000048a0: 6564 2863 616e 6469 6461 7465 2c20 7374  ed(candidate, st
-000048b0: 7265 6e67 7468 5f6d 6174 7269 7829 0a20  rength_matrix). 
-000048c0: 2020 2020 2020 2072 6573 756c 7473 2e61         results.a
-000048d0: 7070 656e 6428 7265 7375 6c74 290a 2020  ppend(result).  
-000048e0: 2020 7265 7475 726e 2072 6573 756c 7473    return results
-000048f0: 0a0a 6465 6620 5f73 706c 6974 5f63 7963  ..def _split_cyc
-00004900: 6c65 5f62 6173 6963 5f70 6172 616c 6c65  le_basic_paralle
-00004910: 6c28 7374 7265 6e67 7468 5f6d 6174 7269  l(strength_matri
-00004920: 782c 206e 756d 5f63 7075 733d 3429 3a0a  x, num_cpus=4):.
-00004930: 0a20 2020 206e 756d 5f63 616e 6473 203d  .    num_cands =
-00004940: 2073 7472 656e 6774 685f 6d61 7472 6978   strength_matrix
-00004950: 2e73 6861 7065 5b30 5d0a 2020 2020 6361  .shape[0].    ca
-00004960: 6e64 7320 3d20 6c69 7374 2872 616e 6765  nds = list(range
-00004970: 286e 756d 5f63 616e 6473 2929 0a20 2020  (num_cands)).   
-00004980: 2062 6174 6368 5f73 697a 6520 3d20 6e75   batch_size = nu
-00004990: 6d5f 6361 6e64 7320 2f2f 206e 756d 5f63  m_cands // num_c
-000049a0: 7075 7320 2b20 286e 756d 5f63 616e 6473  pus + (num_cands
-000049b0: 2025 206e 756d 5f63 7075 7320 3e20 3029   % num_cpus > 0)
-000049c0: 0a20 2020 2063 616e 6469 6461 7465 5f62  .    candidate_b
-000049d0: 6174 6368 6573 203d 206c 6973 7428 6261  atches = list(ba
-000049e0: 7463 6828 6361 6e64 732c 2062 6174 6368  tch(cands, batch
-000049f0: 5f73 697a 6529 290a 2020 2020 7769 7468  _size)).    with
-00004a00: 2050 6f6f 6c28 6e75 6d5f 6370 7573 2920   Pool(num_cpus) 
-00004a10: 6173 2070 6f6f 6c3a 0a20 2020 2020 2020  as pool:.       
-00004a20: 2062 6174 6368 5f61 7267 7320 3d20 5b28   batch_args = [(
-00004a30: 6261 7463 682c 2073 7472 656e 6774 685f  batch, strength_
-00004a40: 6d61 7472 6978 2920 0a20 2020 2020 2020  matrix) .       
-00004a50: 2066 6f72 2062 6174 6368 2069 6e20 6361   for batch in ca
-00004a60: 6e64 6964 6174 655f 6261 7463 6865 735d  ndidate_batches]
-00004a70: 0a20 2020 2020 2020 2072 6573 756c 7473  .        results
-00004a80: 203d 2070 6f6f 6c2e 7374 6172 6d61 7028   = pool.starmap(
-00004a90: 7072 6f63 6573 735f 6261 7463 685f 6f66  process_batch_of
-00004aa0: 5f63 616e 6469 6461 7465 732c 2062 6174  _candidates, bat
-00004ab0: 6368 5f61 7267 7329 0a20 2020 2023 2046  ch_args).    # F
-00004ac0: 6c61 7474 656e 2074 6865 206c 6973 7420  latten the list 
-00004ad0: 6f66 2072 6573 756c 7473 0a20 2020 2073  of results.    s
-00004ae0: 635f 6465 6665 6174 5f64 6174 6120 3d20  c_defeat_data = 
-00004af0: 5b69 7465 6d20 666f 7220 7375 626c 6973  [item for sublis
-00004b00: 7420 696e 2072 6573 756c 7473 2066 6f72  t in results for
-00004b10: 2069 7465 6d20 696e 2073 7562 6c69 7374   item in sublist
-00004b20: 5d0a 0a20 2020 2072 6574 7572 6e20 736f  ]..    return so
-00004b30: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
-00004b40: 2063 616e 6473 2069 6620 6e6f 7420 7363   cands if not sc
-00004b50: 5f64 6566 6561 745f 6461 7461 5b63 5d5d  _defeat_data[c]]
-00004b60: 290a 0a64 6566 205f 7370 6c69 745f 6379  )..def _split_cy
-00004b70: 636c 655f 666c 6f79 645f 7761 7273 6861  cle_floyd_warsha
-00004b80: 6c6c 280a 2020 2020 2020 2020 6564 6174  ll(.        edat
-00004b90: 612c 200a 2020 2020 2020 2020 6375 7272  a, .        curr
-00004ba0: 5f63 616e 6473 203d 204e 6f6e 652c 200a  _cands = None, .
-00004bb0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00004bc0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-00004bd0: 293a 2020 200a 2020 2020 2222 2241 6e20  ):   .    """An 
-00004be0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00004bf0: 6620 5370 6c69 7420 4379 636c 6520 6261  f Split Cycle ba
-00004c00: 7365 6420 6f6e 2074 6865 2046 6c6f 7964  sed on the Floyd
-00004c10: 2d57 6172 7368 616c 6c20 416c 676f 7269  -Warshall Algori
-00004c20: 7468 6d2e 200a 0a20 2020 2053 6565 2068  thm. ..    See h
-00004c30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00004c40: 6d2f 6570 6163 7569 742f 7370 6c69 7463  m/epacuit/splitc
-00004c50: 7963 6c65 2061 6e64 2074 6865 2070 6170  ycle and the pap
-00004c60: 6572 2068 7474 7073 3a2f 2f61 7278 6976  er https://arxiv
-00004c70: 2e6f 7267 2f61 6273 2f32 3030 342e 3032  .org/abs/2004.02
-00004c80: 3335 3020 666f 7220 6d6f 7265 2069 6e66  350 for more inf
-00004c90: 6f72 6d61 7469 6f6e 2e20 0a0a 2020 2020  ormation. ..    
-00004ca0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
-00004cb0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-00004cc0: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-00004cd0: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-00004ce0: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
-00004cf0: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-00004d00: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
-00004d10: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
-00004d20: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
-00004d30: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
-00004d40: 5f66 756e 6374 696f 6e20 0a20 0a20 2020  _function . .   
-00004d50: 2077 6561 6b5f 636f 6e64 6f72 6365 745f   weak_condorcet_
-00004d60: 7769 6e6e 6572 7320 3d20 7b63 3a54 7275  winners = {c:Tru
-00004d70: 6520 666f 7220 6320 696e 2063 616e 6469  e for c in candi
-00004d80: 6461 7465 737d 0a20 2020 2073 5f6d 6174  dates}.    s_mat
-00004d90: 7269 7820 3d20 5b5b 2d6e 702e 696e 6620  rix = [[-np.inf 
-00004da0: 666f 7220 5f20 696e 2063 616e 6469 6461  for _ in candida
-00004db0: 7465 735d 2066 6f72 205f 2069 6e20 6361  tes] for _ in ca
-00004dc0: 6e64 6964 6174 6573 5d0a 2020 2020 0a20  ndidates].    . 
-00004dd0: 2020 2023 2069 6e69 7469 616c 697a 6520     # initialize 
-00004de0: 7468 6520 735f 6d61 7472 6978 0a20 2020  the s_matrix.   
-00004df0: 2066 6f72 2063 315f 6964 782c 2063 3120   for c1_idx, c1 
-00004e00: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
-00004e10: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
-00004e20: 2020 666f 7220 6332 5f69 6478 2c20 6332    for c2_idx, c2
-00004e30: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
-00004e40: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
-00004e50: 2020 2020 2020 2069 6620 2865 6461 7461         if (edata
-00004e60: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
-00004e70: 7328 6331 2c20 6332 2920 6f72 2063 3120  s(c1, c2) or c1 
-00004e80: 3d3d 2063 3229 3a0a 2020 2020 2020 2020  == c2):.        
-00004e90: 2020 2020 2020 2020 735f 6d61 7472 6978          s_matrix
-00004ea0: 5b63 315f 6964 785d 5b63 325f 6964 785d  [c1_idx][c2_idx]
-00004eb0: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
-00004ec0: 7469 6f6e 2863 312c 2063 3229 200a 2020  tion(c1, c2) .  
-00004ed0: 2020 2020 2020 2020 2020 2020 2020 7765                we
-00004ee0: 616b 5f63 6f6e 646f 7263 6574 5f77 696e  ak_condorcet_win
-00004ef0: 6e65 7273 5b63 325d 203d 2077 6561 6b5f  ners[c2] = weak_
-00004f00: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-00004f10: 735b 6332 5d20 616e 6420 2863 3120 3d3d  s[c2] and (c1 ==
-00004f20: 2063 3229 2023 2057 6561 6b20 436f 6e64   c2) # Weak Cond
-00004f30: 6f72 6365 7420 7769 6e6e 6572 7320 6172  orcet winners ar
-00004f40: 6520 5370 6c69 7420 4379 636c 6520 7769  e Split Cycle wi
-00004f50: 6e6e 6572 730a 2020 2020 0a20 2020 2073  nners.    .    s
-00004f60: 7472 656e 6774 6820 3d20 6c69 7374 286d  trength = list(m
-00004f70: 6170 286c 616d 6264 6120 6920 3a20 6c69  ap(lambda i : li
-00004f80: 7374 286d 6170 286c 616d 6264 6120 6a20  st(map(lambda j 
-00004f90: 3a20 6a20 2c20 6929 2920 2c20 735f 6d61  : j , i)) , s_ma
-00004fa0: 7472 6978 2929 0a20 2020 2066 6f72 2069  trix)).    for i
-00004fb0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
-00004fc0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00004fd0: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
-00004fe0: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
-00004ff0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00005000: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005010: 2069 213d 206a 3a0a 2020 2020 2020 2020   i!= j:.        
-00005020: 2020 2020 2020 2020 6966 206e 6f74 2077          if not w
-00005030: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00005040: 6e6e 6572 735b 6a5d 3a20 2320 7765 616b  nners[j]: # weak
-00005050: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
-00005060: 7273 2061 7265 2053 706c 6974 2043 7963  rs are Split Cyc
-00005070: 6c65 2077 696e 6e65 7273 0a20 2020 2020  le winners.     
-00005080: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00005090: 6f72 206b 5f69 6478 2c20 6b20 696e 2065  or k_idx, k in e
-000050a0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
-000050b0: 7465 7329 3a20 0a20 2020 2020 2020 2020  tes): .         
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000050d0: 6620 6920 213d 206b 2061 6e64 206a 2021  f i != k and j !
-000050e0: 3d20 6b3a 0a20 2020 2020 2020 2020 2020  = k:.           
-000050f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005100: 2073 7472 656e 6774 685b 6a5f 6964 785d   strength[j_idx]
-00005110: 5b6b 5f69 6478 5d20 3d20 6d61 7828 7374  [k_idx] = max(st
-00005120: 7265 6e67 7468 5b6a 5f69 6478 5d5b 6b5f  rength[j_idx][k_
-00005130: 6964 785d 2c20 6d69 6e28 7374 7265 6e67  idx], min(streng
-00005140: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
-00005150: 2c73 7472 656e 6774 685b 695f 6964 785d  ,strength[i_idx]
-00005160: 5b6b 5f69 6478 5d29 290a 2020 2020 7769  [k_idx])).    wi
-00005170: 6e6e 6572 7320 3d20 7b69 3a54 7275 6520  nners = {i:True 
-00005180: 666f 7220 6920 696e 2063 616e 6469 6461  for i in candida
-00005190: 7465 737d 0a20 2020 2066 6f72 2069 5f69  tes}.    for i_i
-000051a0: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
-000051b0: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
-000051c0: 2020 2020 2020 2020 666f 7220 6a5f 6964          for j_id
-000051d0: 782c 206a 2069 6e20 656e 756d 6572 6174  x, j in enumerat
-000051e0: 6528 6361 6e64 6964 6174 6573 293a 0a20  e(candidates):. 
-000051f0: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-00005200: 213d 206a 3a0a 2020 2020 2020 2020 2020  != j:.          
-00005210: 2020 2020 2020 6966 2073 5f6d 6174 7269        if s_matri
-00005220: 785b 6a5f 6964 785d 5b69 5f69 6478 5d20  x[j_idx][i_idx] 
-00005230: 3e20 7374 7265 6e67 7468 5b69 5f69 6478  > strength[i_idx
-00005240: 5d5b 6a5f 6964 785d 3a20 2320 7468 6520  ][j_idx]: # the 
-00005250: 6d61 696e 2064 6966 6665 7265 6e63 6520  main difference 
-00005260: 7769 7468 2042 6561 7420 5061 7468 0a20  with Beat Path. 
-00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005280: 2020 2077 696e 6e65 7273 5b69 5d20 3d20     winners[i] = 
-00005290: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
-000052a0: 2073 6f72 7465 6428 5b63 2066 6f72 2063   sorted([c for c
-000052b0: 2069 6e20 6361 6e64 6964 6174 6573 2069   in candidates i
-000052c0: 6620 7769 6e6e 6572 735b 635d 5d29 0a0a  f winners[c]])..
-000052d0: 7363 5f70 726f 7065 7274 6965 7320 3d20  sc_properties = 
-000052e0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
-000052f0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
-00005300: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
-00005310: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
-00005320: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
-00005330: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
-00005340: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
-00005350: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
-00005360: 743d 5472 7565 2c20 0a20 2020 2029 0a40  t=True, .    ).@
-00005370: 766d 286e 616d 653d 2253 706c 6974 2043  vm(name="Split C
-00005380: 7963 6c65 222c 0a20 2020 2070 726f 7065  ycle",.    prope
-00005390: 7274 6965 733d 7363 5f70 726f 7065 7274  rties=sc_propert
-000053a0: 6965 732c 0a20 2020 2069 6e70 7574 5f74  ies,.    input_t
-000053b0: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
-000053c0: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
-000053d0: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-000053e0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
-000053f0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
-00005400: 494e 5f47 5241 5048 5d29 0a64 6566 2073  IN_GRAPH]).def s
-00005410: 706c 6974 5f63 7963 6c65 280a 2020 2020  plit_cycle(.    
-00005420: 6564 6174 612c 200a 2020 2020 6375 7272  edata, .    curr
-00005430: 5f63 616e 6473 3d4e 6f6e 652c 200a 2020  _cands=None, .  
-00005440: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00005450: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 616c  ion=None,.    al
-00005460: 676f 7269 7468 6d3d 2762 6173 6963 272c  gorithm='basic',
-00005470: 0a20 2020 206e 756d 5f63 7075 733d 3429  .    num_cpus=4)
-00005480: 3a0a 0a20 2020 2022 2222 4120 2a2a 6d61  :..    """A **ma
-00005490: 6a6f 7269 7479 2063 7963 6c65 2a2a 2069  jority cycle** i
-000054a0: 7320 6120 7365 7175 656e 6365 203a 6d61  s a sequence :ma
-000054b0: 7468 3a60 785f 312c 205c 6c64 6f74 7320  th:`x_1, \ldots 
-000054c0: 2c78 5f6e 6020 6f66 2064 6973 7469 6e63  ,x_n` of distinc
-000054d0: 7420 6361 6e64 6964 6174 6573 2077 6974  t candidates wit
-000054e0: 6820 3a6d 6174 683a 6078 5f31 3d78 5f6e  h :math:`x_1=x_n
-000054f0: 6020 7375 6368 2074 6861 7420 666f 7220  ` such that for 
-00005500: 3a6d 6174 683a 6031 205c 6c65 7120 6b20  :math:`1 \leq k 
-00005510: 5c6c 6571 206e 2d31 602c 2020 3a6d 6174  \leq n-1`,  :mat
-00005520: 683a 6078 5f6b 6020 6973 206d 616a 6f72  h:`x_k` is major
-00005530: 6974 7920 7072 6566 6572 7265 6420 746f  ity preferred to
-00005540: 203a 6d61 7468 3a60 785f 7b6b 2b31 7d60   :math:`x_{k+1}`
-00005550: 2e20 2054 6865 2053 706c 6974 2043 7963  .  The Split Cyc
-00005560: 6c65 2077 696e 6e65 7273 2061 7265 2064  le winners are d
-00005570: 6574 6572 6d69 6e65 6420 6173 2066 6f6c  etermined as fol
-00005580: 6c6f 7773 3a20 200a 2020 2020 0a20 2020  lows:  .    .   
-00005590: 2049 6620 6361 6e64 6964 6174 6520 7820   If candidate x 
-000055a0: 6861 7320 6120 706f 7369 7469 7665 206d  has a positive m
-000055b0: 6172 6769 6e20 6f76 6572 2079 2061 6e64  argin over y and
-000055c0: 2028 782c 7929 2069 7320 6e6f 7420 7468   (x,y) is not th
-000055d0: 6520 7765 616b 6573 7420 6564 6765 2069  e weakest edge i
-000055e0: 6e20 6120 6379 636c 652c 2074 6865 6e20  n a cycle, then 
-000055f0: 7820 6465 6665 6174 7320 792e 2045 7175  x defeats y. Equ
-00005600: 6976 616c 656e 746c 792c 2069 6620 7820  ivalently, if x 
-00005610: 6861 7320 6120 706f 7369 7469 7665 206d  has a positive m
-00005620: 6172 6769 6e20 6f76 6572 2079 2061 6e64  argin over y and
-00005630: 2074 6865 7265 2069 7320 6e6f 2070 6174   there is no pat
-00005640: 6820 6672 6f6d 2079 2062 6163 6b20 746f  h from y back to
-00005650: 2078 206f 6620 7374 7265 6e67 7468 2061   x of strength a
-00005660: 7420 6c65 6173 7420 7468 6520 6d61 7267  t least the marg
-00005670: 696e 206f 6620 7820 6f76 6572 2079 2c20  in of x over y, 
-00005680: 7468 656e 2078 2064 6566 6561 7473 2079  then x defeats y
-00005690: 2e20 0a20 2020 200a 2020 2020 5468 6520  . .    .    The 
-000056a0: 6361 6e64 6964 6174 6573 2074 6861 7420  candidates that 
-000056b0: 6172 6520 756e 6465 6665 6174 6564 2061  are undefeated a
-000056c0: 7265 2074 6865 2053 706c 6974 2043 7963  re the Split Cyc
-000056d0: 6c65 2077 696e 6e65 7273 2e0a 0a20 2020  le winners...   
-000056e0: 2053 6565 2068 7474 7073 3a2f 2f67 6974   See https://git
-000056f0: 6875 622e 636f 6d2f 6570 6163 7569 742f  hub.com/epacuit/
-00005700: 7370 6c69 7463 7963 6c65 2061 6e64 2074  splitcycle and t
-00005710: 6865 2070 6170 6572 2068 7474 7073 3a2f  he paper https:/
-00005720: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
-00005730: 3030 342e 3032 3335 3020 666f 7220 6d6f  004.02350 for mo
-00005740: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e20  re information. 
-00005750: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00005760: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
-00005770: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
-00005780: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
-00005790: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
-000057a0: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
-000057b0: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
-000057c0: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-000057d0: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-000057e0: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-000057f0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-00005800: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-00005810: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-00005820: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-00005830: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-00005840: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
-00005850: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00005860: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
-00005870: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
-00005880: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
-00005890: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
-000058a0: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
-000058b0: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
-000058c0: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-000058d0: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
-000058e0: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
-000058f0: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
-00005900: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
-00005910: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
-00005920: 6561 7220 6f72 6465 7273 2e20 0a20 2020  ear orders. .   
-00005930: 2020 2020 2061 6c67 6f72 6974 686d 2028       algorithm (
-00005940: 7374 7229 3a20 5370 6563 6966 7920 7768  str): Specify wh
-00005950: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
-00005960: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
-00005970: 7265 2027 6261 7369 6327 2028 7468 6520  re 'basic' (the 
-00005980: 6465 6661 756c 7429 2061 6e64 2027 666c  default) and 'fl
-00005990: 6f79 645f 7761 7273 6861 6c6c 272e 0a0a  oyd_warshall'...
-000059a0: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
-000059b0: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
-000059c0: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
-000059d0: 732e 200a 0a20 2020 202e 2e20 7365 6561  s. ..    .. seea
-000059e0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
-000059f0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-00005a00: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-00005a10: 6574 686f 6473 2e73 706c 6974 5f63 7963  ethods.split_cyc
-00005a20: 6c65 5f64 6566 6561 7460 0a0a 2020 2020  le_defeat`..    
-00005a30: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
-00005a40: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
-00005a50: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
-00005a60: 732f 6d67 5f65 785f 6270 5f72 702e 7079  s/mg_ex_bp_rp.py
-00005a70: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
-00005a80: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
-00005a90: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
-00005aa0: 6365 3a20 5472 7565 0a0a 2020 2020 2e2e  ce: True..    ..
-00005ab0: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
-00005ac0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00005ad0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
-00005ae0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
-00005af0: 706f 7274 2073 706c 6974 5f63 7963 6c65  port split_cycle
-00005b00: 0a0a 2020 2020 2020 2020 7370 6c69 745f  ..        split_
-00005b10: 6379 636c 652e 6469 7370 6c61 7928 6d67  cycle.display(mg
-00005b20: 290a 0a0a 2020 2020 2e2e 2065 7865 635f  )...    .. exec_
-00005b30: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
-00005b40: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
-00005b50: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00005b60: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
-00005b70: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
-00005b80: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
-00005b90: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
-00005ba0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00005bb0: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
-00005bc0: 696d 706f 7274 2073 706c 6974 5f63 7963  import split_cyc
-00005bd0: 6c65 0a20 2020 2020 2020 200a 2020 2020  le.        .    
-00005be0: 2020 2020 6d67 203d 204d 6172 6769 6e47      mg = MarginG
-00005bf0: 7261 7068 285b 302c 2031 2c20 322c 2033  raph([0, 1, 2, 3
-00005c00: 5d2c 205b 2830 2c20 322c 2033 292c 2028  ], [(0, 2, 3), (
-00005c10: 312c 2030 2c20 3529 2c20 2832 2c20 312c  1, 0, 5), (2, 1,
-00005c20: 2035 292c 2028 322c 2033 2c20 3129 2c20   5), (2, 3, 1), 
-00005c30: 2833 2c20 302c 2033 292c 2028 332c 2031  (3, 0, 3), (3, 1
-00005c40: 2c20 3129 5d29 0a20 2020 2020 2020 200a  , 1)]).        .
-00005c50: 2020 2020 2020 2020 7370 6c69 745f 6379          split_cy
-00005c60: 636c 652e 6469 7370 6c61 7928 6d67 290a  cle.display(mg).
-00005c70: 2020 2020 2020 2020 7370 6c69 745f 6379          split_cy
-00005c80: 636c 652e 6469 7370 6c61 7928 6d67 2c20  cle.display(mg, 
-00005c90: 616c 676f 7269 7468 6d3d 2762 6173 6963  algorithm='basic
-00005ca0: 2729 0a20 2020 2020 2020 2073 706c 6974  ').        split
-00005cb0: 5f63 7963 6c65 2e64 6973 706c 6179 286d  _cycle.display(m
-00005cc0: 672c 2061 6c67 6f72 6974 686d 3d27 666c  g, algorithm='fl
-00005cd0: 6f79 645f 7761 7273 6861 6c6c 2729 0a20  oyd_warshall'). 
-00005ce0: 2020 2022 2222 0a20 2020 200a 2020 2020     """.    .    
-00005cf0: 6966 2061 6c67 6f72 6974 686d 203d 3d20  if algorithm == 
-00005d00: 2762 6173 6963 273a 0a20 2020 2020 2020  'basic':.       
-00005d10: 2072 6574 7572 6e20 5f73 706c 6974 5f63   return _split_c
-00005d20: 7963 6c65 5f62 6173 6963 2865 6461 7461  ycle_basic(edata
-00005d30: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
-00005d40: 7572 725f 6361 6e64 732c 2073 7472 656e  urr_cands, stren
-00005d50: 6774 685f 6675 6e63 7469 6f6e 203d 2073  gth_function = s
-00005d60: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-00005d70: 290a 2020 2020 656c 6966 2061 6c67 6f72  ).    elif algor
-00005d80: 6974 686d 203d 3d20 2766 6c6f 7964 5f77  ithm == 'floyd_w
-00005d90: 6172 7368 616c 6c27 3a0a 2020 2020 2020  arshall':.      
-00005da0: 2020 7265 7475 726e 205f 7370 6c69 745f    return _split_
-00005db0: 6379 636c 655f 666c 6f79 645f 7761 7273  cycle_floyd_wars
-00005dc0: 6861 6c6c 2865 6461 7461 2c20 6375 7272  hall(edata, curr
-00005dd0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
-00005de0: 6e64 732c 2073 7472 656e 6774 685f 6675  nds, strength_fu
-00005df0: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
-00005e00: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
-00005e10: 656c 6966 2061 6c67 6f72 6974 686d 203d  elif algorithm =
-00005e20: 3d20 2762 6173 6963 5f70 6172 616c 6c65  = 'basic_paralle
-00005e30: 6c27 3a0a 2020 2020 2020 2020 6375 7272  l':.        curr
-00005e40: 5f63 616e 6473 203d 2065 6461 7461 2e63  _cands = edata.c
-00005e50: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
-00005e60: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
-00005e70: 656c 7365 2063 7572 725f 6361 6e64 730a  else curr_cands.
-00005e80: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00005e90: 5f6d 6174 7269 782c 2063 616e 645f 746f  _matrix, cand_to
-00005ea0: 5f63 696e 6465 7820 3d20 6564 6174 612e  _cindex = edata.
-00005eb0: 7374 7265 6e67 7468 5f6d 6174 7269 7828  strength_matrix(
-00005ec0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-00005ed0: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
-00005ee0: 685f 6675 6e63 7469 6f6e 3d73 7472 656e  h_function=stren
-00005ef0: 6774 685f 6675 6e63 7469 6f6e 290a 2020  gth_function).  
-00005f00: 2020 2020 2020 6369 6e64 785f 746f 5f63        cindx_to_c
-00005f10: 616e 6420 3d20 7b63 616e 645f 746f 5f63  and = {cand_to_c
-00005f20: 696e 6465 7828 6329 3a63 2066 6f72 2063  index(c):c for c
-00005f30: 2069 6e20 6375 7272 5f63 616e 6473 7d0a   in curr_cands}.
-00005f40: 2020 2020 2020 2020 7363 5f77 7320 3d20          sc_ws = 
-00005f50: 5f73 706c 6974 5f63 7963 6c65 5f62 6173  _split_cycle_bas
-00005f60: 6963 5f70 6172 616c 6c65 6c28 7374 7265  ic_parallel(stre
-00005f70: 6e67 7468 5f6d 6174 7269 782c 6e75 6d5f  ngth_matrix,num_
-00005f80: 6370 7573 3d6e 756d 5f63 7075 7329 0a20  cpus=num_cpus). 
-00005f90: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
-00005fa0: 7274 6564 285b 6369 6e64 785f 746f 5f63  rted([cindx_to_c
-00005fb0: 616e 645b 635d 2066 6f72 2063 2069 6e20  and[c] for c in 
-00005fc0: 7363 5f77 735d 290a 2020 2020 656c 7365  sc_ws]).    else
-00005fd0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-00005fe0: 5661 6c75 6545 7272 6f72 2822 496e 7661  ValueError("Inva
-00005ff0: 6c69 6420 616c 676f 7269 7468 6d20 7370  lid algorithm sp
-00006000: 6563 6966 6965 642e 2229 0a0a 0a64 6566  ecified.")...def
-00006010: 2073 706c 6974 5f63 7963 6c65 5f64 6566   split_cycle_def
-00006020: 6561 7428 6564 6174 612c 2063 7572 725f  eat(edata, curr_
-00006030: 6361 6e64 7320 3d20 4e6f 6e65 2c20 7374  cands = None, st
-00006040: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00006050: 3d20 4e6f 6e65 293a 2020 200a 2020 2020  = None):   .    
-00006060: 2222 220a 2020 2020 5265 7475 726e 7320  """.    Returns 
-00006070: 7468 6520 5370 6c69 7420 4379 636c 6520  the Split Cycle 
-00006080: 6465 6665 6174 2072 656c 6174 696f 6e2e  defeat relation.
-00006090: 200a 0a20 2020 2053 6565 2068 7474 7073   ..    See https
-000060a0: 3a2f 2f61 7278 6976 2e6f 7267 2f61 6273  ://arxiv.org/abs
-000060b0: 2f32 3030 382e 3038 3435 3120 666f 7220  /2008.08451 for 
-000060c0: 616e 2065 7874 656e 6465 6420 6469 7363  an extended disc
-000060d0: 7573 7369 6f6e 206f 6620 7468 6973 206e  ussion of this n
-000060e0: 6f74 696f 6e20 6f66 2064 6566 6561 7420  otion of defeat 
-000060f0: 696e 2061 6e20 656c 6563 7469 6f6e 2e20  in an election. 
-00006100: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
-00006110: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
-00006120: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
-00006130: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
-00006140: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
-00006150: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
-00006160: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
-00006170: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-00006180: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-00006190: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-000061a0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-000061b0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-000061c0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-000061d0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-000061e0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-000061f0: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
-00006200: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-00006210: 4120 6e65 7477 6f72 6b78 2044 6947 7261  A networkx DiGra
-00006220: 7068 2072 6570 7265 7365 6e74 696e 6720  ph representing 
-00006230: 7468 6520 5370 6c69 7420 4379 636c 6520  the Split Cycle 
-00006240: 6465 6665 6174 2072 656c 6174 696f 6e2e  defeat relation.
-00006250: 200a 0a20 2020 202e 2e20 7365 6561 6c73   ..    .. seeals
-00006260: 6f3a 3a0a 0a20 2020 2020 2020 203a 6d65  o::..        :me
-00006270: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-00006280: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00006290: 686f 6473 2e73 706c 6974 5f63 7963 6c65  hods.split_cycle
-000062a0: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
-000062b0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
-000062c0: 6564 5f6d 6574 686f 6473 2e73 706c 6974  ed_methods.split
-000062d0: 5f63 7963 6c65 5f46 6c6f 7964 5f57 6172  _cycle_Floyd_War
-000062e0: 7368 616c 6c60 0a0a 2020 2020 3a45 7861  shall`..    :Exa
-000062f0: 6d70 6c65 3a20 0a0a 2020 2020 2e2e 2070  mple: ..    .. p
-00006300: 6c6f 743a 3a20 206d 6172 6769 6e5f 6772  lot::  margin_gr
-00006310: 6170 6873 5f65 7861 6d70 6c65 732f 6d67  aphs_examples/mg
-00006320: 5f65 785f 7363 5f64 6566 6561 742e 7079  _ex_sc_defeat.py
-00006330: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
-00006340: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
-00006350: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
-00006360: 6365 3a20 5472 7565 0a0a 2020 2020 2222  ce: True..    ""
-00006370: 220a 0a20 2020 2063 616e 6469 6461 7465  "..    candidate
-00006380: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00006390: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-000063a0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-000063b0: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
-000063c0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-000063d0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-000063e0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-000063f0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-00006400: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-00006410: 756e 6374 696f 6e20 0a20 0a20 2020 2077  unction . .    w
-00006420: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00006430: 6e6e 6572 7320 3d20 7b63 3a54 7275 6520  nners = {c:True 
-00006440: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
-00006450: 7465 737d 0a20 2020 2073 5f6d 6174 7269  tes}.    s_matri
-00006460: 7820 3d20 5b5b 2d6e 702e 696e 6620 666f  x = [[-np.inf fo
-00006470: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
-00006480: 735d 2066 6f72 205f 2069 6e20 6361 6e64  s] for _ in cand
-00006490: 6964 6174 6573 5d0a 2020 2020 0a20 2020  idates].    .   
-000064a0: 2023 2069 6e69 7469 616c 697a 6520 7468   # initialize th
-000064b0: 6520 735f 6d61 7472 6978 0a20 2020 2066  e s_matrix.    f
-000064c0: 6f72 2063 315f 6964 782c 2063 3120 696e  or c1_idx, c1 in
-000064d0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-000064e0: 6461 7465 7329 3a0a 2020 2020 2020 2020  dates):.        
-000064f0: 666f 7220 6332 5f69 6478 2c20 6332 2069  for c2_idx, c2 i
-00006500: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
-00006510: 6964 6174 6573 293a 0a20 2020 2020 2020  idates):.       
-00006520: 2020 2020 2069 6620 2865 6461 7461 2e6d       if (edata.m
-00006530: 616a 6f72 6974 795f 7072 6566 6572 7328  ajority_prefers(
-00006540: 6331 2c20 6332 2920 6f72 2063 3120 3d3d  c1, c2) or c1 ==
-00006550: 2063 3229 3a0a 2020 2020 2020 2020 2020   c2):.          
-00006560: 2020 2020 2020 735f 6d61 7472 6978 5b63        s_matrix[c
-00006570: 315f 6964 785d 5b63 325f 6964 785d 203d  1_idx][c2_idx] =
-00006580: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-00006590: 6f6e 2863 312c 2063 3229 200a 2020 2020  on(c1, c2) .    
-000065a0: 2020 2020 2020 2020 2020 2020 7765 616b              weak
-000065b0: 5f63 6f6e 646f 7263 6574 5f77 696e 6e65  _condorcet_winne
-000065c0: 7273 5b63 325d 203d 2077 6561 6b5f 636f  rs[c2] = weak_co
-000065d0: 6e64 6f72 6365 745f 7769 6e6e 6572 735b  ndorcet_winners[
-000065e0: 6332 5d20 616e 6420 2863 3120 3d3d 2063  c2] and (c1 == c
-000065f0: 3229 2023 2077 6561 6b20 436f 6e64 6f72  2) # weak Condor
-00006600: 6365 7420 7769 6e6e 6572 7320 6172 6520  cet winners are 
-00006610: 5370 6c69 7420 4379 636c 6520 7769 6e6e  Split Cycle winn
-00006620: 6572 730a 2020 2020 0a20 2020 2073 7472  ers.    .    str
-00006630: 656e 6774 6820 3d20 6c69 7374 286d 6170  ength = list(map
-00006640: 286c 616d 6264 6120 6920 3a20 6c69 7374  (lambda i : list
-00006650: 286d 6170 286c 616d 6264 6120 6a20 3a20  (map(lambda j : 
-00006660: 6a20 2c20 6929 2920 2c20 735f 6d61 7472  j , i)) , s_matr
-00006670: 6978 2929 0a20 2020 2066 6f72 2069 5f69  ix)).    for i_i
-00006680: 6478 2c20 6920 696e 2065 6e75 6d65 7261  dx, i in enumera
-00006690: 7465 2863 616e 6469 6461 7465 7329 3a20  te(candidates): 
-000066a0: 0a20 2020 2020 2020 2066 6f72 206a 5f69  .        for j_i
-000066b0: 6478 2c20 6a20 696e 2065 6e75 6d65 7261  dx, j in enumera
-000066c0: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
-000066d0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-000066e0: 213d 206a 3a0a 2020 2020 2020 2020 2020  != j:.          
-000066f0: 2020 2020 2020 6966 206e 6f74 2077 6561        if not wea
-00006700: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
-00006710: 6572 735b 6a5d 3a20 2320 7765 616b 2043  ers[j]: # weak C
-00006720: 6f6e 646f 7263 6574 2077 696e 6e65 7273  ondorcet winners
-00006730: 2061 7265 2053 706c 6974 2043 7963 6c65   are Split Cycle
-00006740: 2077 696e 6e65 7273 0a20 2020 2020 2020   winners.       
-00006750: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-00006760: 206b 5f69 6478 2c20 6b20 696e 2065 6e75   k_idx, k in enu
-00006770: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-00006780: 7329 3a20 0a20 2020 2020 2020 2020 2020  s): .           
-00006790: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000067a0: 6920 213d 206b 2061 6e64 206a 2021 3d20  i != k and j != 
-000067b0: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
-000067c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000067d0: 7472 656e 6774 685b 6a5f 6964 785d 5b6b  trength[j_idx][k
-000067e0: 5f69 6478 5d20 3d20 6d61 7828 7374 7265  _idx] = max(stre
-000067f0: 6e67 7468 5b6a 5f69 6478 5d5b 6b5f 6964  ngth[j_idx][k_id
-00006800: 785d 2c20 6d69 6e28 7374 7265 6e67 7468  x], min(strength
-00006810: 5b6a 5f69 6478 5d5b 695f 6964 785d 2c73  [j_idx][i_idx],s
-00006820: 7472 656e 6774 685b 695f 6964 785d 5b6b  trength[i_idx][k
-00006830: 5f69 6478 5d29 290a 200a 2020 2020 6465  _idx])). .    de
-00006840: 6665 6174 5f67 7261 7068 203d 206e 782e  feat_graph = nx.
-00006850: 4469 4772 6170 6828 290a 2020 2020 6465  DiGraph().    de
-00006860: 6665 6174 5f67 7261 7068 2e61 6464 5f6e  feat_graph.add_n
-00006870: 6f64 6573 5f66 726f 6d28 6361 6e64 6964  odes_from(candid
-00006880: 6174 6573 290a 0a20 2020 2066 6f72 2069  ates)..    for i
-00006890: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
-000068a0: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-000068b0: 3a0a 2020 2020 2020 2020 666f 7220 6a5f  :.        for j_
-000068c0: 6964 782c 206a 2069 6e20 656e 756d 6572  idx, j in enumer
-000068d0: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
-000068e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000068f0: 6920 213d 206a 3a0a 2020 2020 2020 2020  i != j:.        
-00006900: 2020 2020 2020 2020 6966 2073 5f6d 6174          if s_mat
-00006910: 7269 785b 6a5f 6964 785d 5b69 5f69 6478  rix[j_idx][i_idx
-00006920: 5d20 3e20 7374 7265 6e67 7468 5b69 5f69  ] > strength[i_i
-00006930: 6478 5d5b 6a5f 6964 785d 3a20 2320 7468  dx][j_idx]: # th
-00006940: 6520 6d61 696e 2064 6966 6665 7265 6e63  e main differenc
-00006950: 6520 7769 7468 2042 6561 7420 5061 7468  e with Beat Path
-00006960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006970: 2020 2020 2064 6566 6561 745f 6772 6170       defeat_grap
-00006980: 682e 6164 645f 7765 6967 6874 6564 5f65  h.add_weighted_e
-00006990: 6467 6573 5f66 726f 6d28 5b28 6a2c 692c  dges_from([(j,i,
-000069a0: 735f 6d61 7472 6978 5b6a 5f69 6478 5d5b  s_matrix[j_idx][
-000069b0: 695f 6964 785d 295d 290a 2020 2020 2020  i_idx])]).      
-000069c0: 2020 2020 2020 2020 2020 0a20 2020 2072            .    r
-000069d0: 6574 7572 6e20 6465 6665 6174 5f67 7261  eturn defeat_gra
-000069e0: 7068 0a0a 0a23 2066 6c61 7474 656e 2061  ph...# flatten a
-000069f0: 2032 6420 6c69 7374 202d 2074 7572 6e20   2d list - turn 
-00006a00: 6120 3264 206c 6973 7420 696e 746f 2061  a 2d list into a
-00006a10: 2073 696e 676c 6520 6c69 7374 206f 6620   single list of 
-00006a20: 6974 656d 730a 666c 6174 7465 6e20 3d20  items.flatten = 
-00006a30: 6c61 6d62 6461 206c 3a20 5b69 7465 6d20  lambda l: [item 
-00006a40: 666f 7220 7375 626c 6973 7420 696e 206c  for sublist in l
-00006a50: 2066 6f72 2069 7465 6d20 696e 2073 7562   for item in sub
-00006a60: 6c69 7374 5d0a 0a64 6566 2064 6f65 735f  list]..def does_
-00006a70: 6372 6561 7465 5f63 7963 6c65 2867 2c20  create_cycle(g, 
-00006a80: 6564 6765 293a 0a20 2020 2027 2727 7265  edge):.    '''re
-00006a90: 7475 726e 2054 7275 6520 6966 2061 6464  turn True if add
-00006aa0: 696e 6720 7468 6520 6564 6765 2074 6f20  ing the edge to 
-00006ab0: 6720 6372 6561 7465 2061 2063 7963 6c65  g create a cycle
-00006ac0: 2e0a 2020 2020 6974 2069 7320 6173 7375  ..    it is assu
-00006ad0: 6d65 6420 7468 6174 2065 6467 6520 6973  med that edge is
-00006ae0: 2061 6c72 6561 6479 2069 6e20 6727 2727   already in g'''
-00006af0: 0a20 2020 2073 6f75 7263 6520 3d20 6564  .    source = ed
-00006b00: 6765 5b30 5d0a 2020 2020 7461 7267 6574  ge[0].    target
-00006b10: 203d 2065 6467 655b 315d 0a20 2020 2066   = edge[1].    f
-00006b20: 6f72 206e 2069 6e20 672e 7072 6564 6563  or n in g.predec
-00006b30: 6573 736f 7273 2873 6f75 7263 6529 3a0a  essors(source):.
-00006b40: 2020 2020 2020 2020 6966 206e 782e 6861          if nx.ha
-00006b50: 735f 7061 7468 2867 2c20 7461 7267 6574  s_path(g, target
-00006b60: 2c20 6e29 3a20 0a20 2020 2020 2020 2020  , n): .         
-00006b70: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00006b80: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00006b90: 0a0a 0a64 6566 2070 6f77 6572 7365 7428  ...def powerset(
-00006ba0: 6974 6572 6162 6c65 293a 0a20 2020 2022  iterable):.    "
-00006bb0: 2222 0a20 2020 2052 6574 7572 6e20 7468  "".    Return th
-00006bc0: 6520 706f 7765 7273 6574 206f 6620 6060  e powerset of ``
-00006bd0: 6974 6572 6162 6c65 6060 0a0a 2020 2020  iterable``..    
-00006be0: 706f 7765 7273 6574 285b 312c 322c 335d  powerset([1,2,3]
-00006bf0: 2920 2d2d 3e20 2829 2028 312c 2920 2832  ) --> () (1,) (2
-00006c00: 2c29 2028 332c 2920 2831 2c32 2920 2831  ,) (3,) (1,2) (1
-00006c10: 2c33 2920 2832 2c33 2920 2831 2c32 2c33  ,3) (2,3) (1,2,3
-00006c20: 290a 2020 2020 2222 220a 2020 2020 7320  ).    """.    s 
-00006c30: 3d20 6c69 7374 2869 7465 7261 626c 6529  = list(iterable)
-00006c40: 0a20 2020 2072 6574 7572 6e20 6368 6169  .    return chai
-00006c50: 6e2e 6672 6f6d 5f69 7465 7261 626c 6528  n.from_iterable(
-00006c60: 636f 6d62 696e 6174 696f 6e73 2873 2c20  combinations(s, 
-00006c70: 7229 2066 6f72 2072 2069 6e20 7261 6e67  r) for r in rang
-00006c80: 6528 6c65 6e28 7329 2b31 2929 0a0a 0a64  e(len(s)+1))...d
-00006c90: 6566 2069 735f 7374 6163 6b28 6564 6174  ef is_stack(edat
-00006ca0: 612c 2063 616e 645f 6c69 7374 2c20 6375  a, cand_list, cu
-00006cb0: 7272 5f63 616e 6473 3d4e 6f6e 6529 3a20  rr_cands=None): 
-00006cc0: 0a20 2020 2022 2222 0a20 2020 2041 202a  .    """.    A *
-00006cd0: 2a73 7461 636b 2a2a 2069 7320 6120 6c69  *stack** is a li
-00006ce0: 6e65 6172 206f 7264 6572 203a 6d61 7468  near order :math
-00006cf0: 3a60 4c60 206f 6e20 7468 6520 6361 6e64  :`L` on the cand
-00006d00: 6964 6174 6520 7375 6368 2074 6861 7420  idate such that 
-00006d10: 666f 7220 616c 6c20 6361 6e64 6964 6174  for all candidat
-00006d20: 6573 203a 6d61 7468 3a60 6160 2061 6e64  es :math:`a` and
-00006d30: 203a 6d61 7468 3a60 6260 2c20 6966 203a   :math:`b`, if :
-00006d40: 6d61 7468 3a60 614c 6260 2c20 7468 656e  math:`aLb`, then
-00006d50: 2074 6865 7265 2061 7265 2064 6973 7469   there are disti
-00006d60: 6e63 7420 6361 6e64 6964 6174 6573 203a  nct candidates :
-00006d70: 6d61 7468 3a60 785f 312c 5c64 6f74 732c  math:`x_1,\dots,
-00006d80: 785f 6e60 2077 6974 6820 3a6d 6174 683a  x_n` with :math:
-00006d90: 6078 5f31 3d61 6020 616e 6420 3a6d 6174  `x_1=a` and :mat
-00006da0: 683a 6078 5f6e 3d62 6020 7375 6368 2074  h:`x_n=b` such t
-00006db0: 6861 7420 3a6d 6174 683a 6078 5f69 204c  hat :math:`x_i L
-00006dc0: 2078 5f7b 692b 317d 6020 616e 6420 666f   x_{i+1}` and fo
-00006dd0: 7220 616c 6c20 3a6d 6174 683a 6069 5c69  r all :math:`i\i
-00006de0: 6e20 5c7b 312c 5c64 6f74 732c 206e 2d31  n \{1,\dots, n-1
-00006df0: 5c7d 602c 2074 6865 206d 6172 6769 6e20  \}`, the margin 
-00006e00: 6f66 203a 6d61 7468 3a60 785f 3160 206f  of :math:`x_1` o
-00006e10: 7665 7220 3a6d 6174 683a 6078 5f7b 692b  ver :math:`x_{i+
-00006e20: 317d 6020 6973 2067 7265 6174 6572 2074  1}` is greater t
-00006e30: 6861 6e20 6f72 2065 7175 616c 2074 6f20  han or equal to 
-00006e40: 7468 6520 6d61 7267 696e 206f 6620 3a6d  the margin of :m
-00006e50: 6174 683a 6062 6020 6f76 6572 203a 6d61  ath:`b` over :ma
-00006e60: 7468 3a60 6160 2e0a 0a20 2020 2054 6869  th:`a`...    Thi
-00006e70: 7320 6465 6669 6e69 7469 6f6e 2069 7320  s definition is 
-00006e80: 6475 6520 746f 205a 6176 6973 7420 616e  due to Zavist an
-00006e90: 6420 5469 6465 6d61 6e20 3139 3839 2c20  d Tideman 1989, 
-00006ea0: 616e 6420 6973 2075 7365 6420 6173 2061  and is used as a
-00006eb0: 6e20 616c 7465 726e 6174 6976 6520 6368  n alternative ch
-00006ec0: 6172 6163 7465 7269 7a61 7469 6f6e 206f  aracterization o
-00006ed0: 6620 5261 6e6b 6564 2050 6169 7273 3a20  f Ranked Pairs: 
-00006ee0: 3a6d 6174 683a 6061 6020 6973 2061 2052  :math:`a` is a R
-00006ef0: 616e 6b65 6420 5061 6972 7320 7769 6e6e  anked Pairs winn
-00006f00: 6572 2069 6620 616e 6420 6f6e 6c79 2069  er if and only i
-00006f10: 6620 3a6d 6174 683a 6061 6020 6973 2074  f :math:`a` is t
-00006f20: 6865 206d 6178 696d 756d 2065 6c65 6d65  he maximum eleme
-00006f30: 6e74 206f 6620 736f 6d65 2073 7461 636b  nt of some stack
-00006f40: 2e20 0a0a 2020 2020 4172 6773 3a0a 2020  . ..    Args:.  
-00006f50: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
-00006f60: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
-00006f70: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
-00006f80: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
-00006f90: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
-00006fa0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
-00006fb0: 642e 200a 2020 2020 2020 2020 6361 6e64  d. .        cand
-00006fc0: 5f6c 6973 7420 286c 6973 7429 3a20 5468  _list (list): Th
-00006fd0: 6520 6c69 7374 206f 6620 6361 6e64 6964  e list of candid
-00006fe0: 6174 6573 2074 6861 7420 6d61 7920 6265  ates that may be
-00006ff0: 2061 2073 7461 636b 0a20 2020 2020 2020   a stack.       
-00007000: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00007010: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00007020: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00007030: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00007040: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00007050: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00007060: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00007070: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00007080: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
-00007090: 2020 2020 2020 2054 7275 6520 6966 2060         True if `
-000070a0: 6063 616e 645f 6c69 7374 6060 2069 7320  `cand_list`` is 
-000070b0: 6120 7374 6163 6b20 616e 6420 4661 6c73  a stack and Fals
-000070c0: 6520 6f74 6865 7277 6973 650a 0a20 2020  e otherwise..   
-000070d0: 203a 4578 616d 706c 653a 200a 2020 2020   :Example: .    
-000070e0: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-000070f0: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00007100: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
-00007110: 7374 6163 6b73 2e70 790a 2020 2020 2020  stacks.py.      
-00007120: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
-00007130: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
-00007140: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
-00007150: 650a 0a0a 2020 2020 2e2e 2065 7865 635f  e...    .. exec_
-00007160: 636f 6465 3a3a 0a20 2020 2020 2020 200a  code::.        .
-00007170: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00007180: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-00007190: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-000071a0: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-000071b0: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-000071c0: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-000071d0: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-000071e0: 6473 2069 6d70 6f72 7420 6973 5f73 7461  ds import is_sta
-000071f0: 636b 0a20 2020 2020 2020 2066 726f 6d20  ck.        from 
-00007200: 6974 6572 746f 6f6c 7320 696d 706f 7274  itertools import
-00007210: 2070 6572 6d75 7461 7469 6f6e 730a 2020   permutations.  
-00007220: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
-00007230: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
-00007240: 5b30 2c20 312c 2032 5d2c 205b 2830 2c20  [0, 1, 2], [(0, 
-00007250: 312c 2032 292c 2028 312c 2032 2c20 3429  1, 2), (1, 2, 4)
-00007260: 2c20 2832 2c20 302c 2032 295d 290a 2020  , (2, 0, 2)]).  
-00007270: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
-00007280: 6f72 2063 6c69 7374 2069 6e20 7065 726d  or clist in perm
-00007290: 7574 6174 696f 6e73 286d 672e 6361 6e64  utations(mg.cand
-000072a0: 6964 6174 6573 293a 200a 2020 2020 2020  idates): .      
-000072b0: 2020 2020 2020 7072 696e 7428 6622 7b63        print(f"{c
-000072c0: 6c69 7374 7d20 7b27 6973 2720 6966 2069  list} {'is' if i
-000072d0: 735f 7374 6163 6b28 6d67 2c20 636c 6973  s_stack(mg, clis
-000072e0: 7429 2065 6c73 6520 2769 7320 6e6f 7427  t) else 'is not'
-000072f0: 7d20 6120 7374 6163 6b22 290a 2020 2020  } a stack").    
-00007300: 2020 2020 2020 2020 0a20 2020 2022 2222          .    """
-00007310: 0a20 2020 200a 2020 2020 6361 6e64 6964  .    .    candid
-00007320: 6174 6573 203d 2063 7572 725f 6361 6e64  ates = curr_cand
-00007330: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-00007340: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00007350: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-00007360: 730a 2020 2020 6361 6e64 5f70 6169 7273  s.    cand_pairs
-00007370: 203d 205b 2861 2c20 6229 2069 6620 6361   = [(a, b) if ca
-00007380: 6e64 5f6c 6973 742e 696e 6465 7828 6129  nd_list.index(a)
-00007390: 203c 2063 616e 645f 6c69 7374 2e69 6e64   < cand_list.ind
-000073a0: 6578 2862 2920 656c 7365 2028 622c 2061  ex(b) else (b, a
-000073b0: 2920 666f 7220 612c 2062 2069 6e20 636f  ) for a, b in co
-000073c0: 6d62 696e 6174 696f 6e73 2863 616e 6469  mbinations(candi
-000073d0: 6461 7465 732c 2032 295d 0a20 2020 2020  dates, 2)].     
-000073e0: 2020 200a 2020 2020 666f 7220 612c 2062     .    for a, b
-000073f0: 2069 6e20 6361 6e64 5f70 6169 7273 3a0a   in cand_pairs:.
-00007400: 2020 2020 2020 2020 6f74 6865 725f 6361          other_ca
-00007410: 6e64 7320 3d20 5b63 2066 6f72 2063 2069  nds = [c for c i
-00007420: 6e20 6361 6e64 6964 6174 6573 2069 6620  n candidates if 
-00007430: 6320 213d 2061 2061 6e64 2063 2021 3d20  c != a and c != 
-00007440: 625d 0a20 2020 2020 2020 2066 6f75 6e64  b].        found
-00007450: 5f70 6174 6820 3d20 4661 6c73 650a 2020  _path = False.  
-00007460: 2020 2020 2020 0a20 2020 2020 2020 2073        .        s
-00007470: 7562 6c69 7374 203d 2063 616e 645f 6c69  ublist = cand_li
-00007480: 7374 5b63 616e 645f 6c69 7374 2e69 6e64  st[cand_list.ind
-00007490: 6578 2861 2920 2b20 313a 6361 6e64 5f6c  ex(a) + 1:cand_l
-000074a0: 6973 742e 696e 6465 7828 6229 5d0a 2020  ist.index(b)].  
-000074b0: 2020 2020 2020 0a20 2020 2020 2020 2066        .        f
-000074c0: 6f72 2069 6e64 6963 6573 2069 6e20 706f  or indices in po
-000074d0: 7765 7273 6574 2872 616e 6765 286c 656e  werset(range(len
-000074e0: 2873 7562 6c69 7374 2929 293a 200a 2020  (sublist))): .  
-000074f0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00007500: 2020 2020 2020 2070 6174 6820 3d20 5b61         path = [a
-00007510: 5d20 2b20 5b73 7562 6c69 7374 5b69 5d20  ] + [sublist[i] 
-00007520: 666f 7220 6920 696e 2073 6f72 7465 6428  for i in sorted(
-00007530: 696e 6469 6365 7329 5d20 2b20 5b62 5d0a  indices)] + [b].
-00007540: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
-00007550: 696e 7320 3d20 5b65 6461 7461 2e6d 6172  ins = [edata.mar
-00007560: 6769 6e28 7869 2c20 7061 7468 5b69 202b  gin(xi, path[i +
-00007570: 2031 5d29 2066 6f72 2069 2c20 7869 2069   1]) for i, xi i
-00007580: 6e20 656e 756d 6572 6174 6528 7061 7468  n enumerate(path
-00007590: 5b30 3a2d 315d 295d 0a20 2020 2020 2020  [0:-1])].       
-000075a0: 2020 2020 2069 6620 616c 6c28 5b63 616e       if all([can
-000075b0: 645f 6c69 7374 2e69 6e64 6578 2878 6929  d_list.index(xi)
-000075c0: 203c 2063 616e 645f 6c69 7374 2e69 6e64   < cand_list.ind
-000075d0: 6578 2870 6174 685b 692b 315d 2920 666f  ex(path[i+1]) fo
-000075e0: 7220 692c 2078 6920 696e 2065 6e75 6d65  r i, xi in enume
-000075f0: 7261 7465 2870 6174 685b 303a 2d31 5d29  rate(path[0:-1])
-00007600: 5d29 2061 6e64 2061 6c6c 285b 6d20 3e3d  ]) and all([m >=
-00007610: 2065 6461 7461 2e6d 6172 6769 6e28 622c   edata.margin(b,
-00007620: 2061 2920 666f 7220 6d20 696e 206d 6172   a) for m in mar
-00007630: 6769 6e73 5d29 3a20 0a20 2020 2020 2020  gins]): .       
-00007640: 2020 2020 2020 2020 2066 6f75 6e64 5f70           found_p
-00007650: 6174 6820 3d20 5472 7565 0a20 2020 2020  ath = True.     
-00007660: 2020 2020 2020 2020 2020 2062 7265 616b             break
-00007670: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00007680: 666f 756e 645f 7061 7468 3a20 0a20 2020  found_path: .   
-00007690: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-000076a0: 4661 6c73 650a 2020 2020 7265 7475 726e  False.    return
-000076b0: 2054 7275 650a 0a64 6566 205f 7261 6e6b   True..def _rank
-000076c0: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
-000076d0: 6163 6b73 2865 6461 7461 2c20 6375 7272  acks(edata, curr
-000076e0: 5f63 616e 6473 203d 204e 6f6e 6529 3a20  _cands = None): 
-000076f0: 0a20 2020 2022 2222 4669 6e64 2074 6865  .    """Find the
-00007700: 2052 616e 6b65 6420 5061 6972 7320 7769   Ranked Pairs wi
-00007710: 6e6e 6572 7320 6279 2069 7465 7261 7469  nners by iterati
-00007720: 6e67 206f 7665 7220 616c 6c20 7065 726d  ng over all perm
-00007730: 7574 6174 696f 6e73 206f 6620 6361 6e64  utations of cand
-00007740: 6964 6174 6573 2028 7265 7374 7269 6374  idates (restrict
-00007750: 6564 2074 6f20 6060 6375 7272 5f63 616e  ed to ``curr_can
-00007760: 6473 6060 2069 6620 6e6f 7420 4e6f 6e65  ds`` if not None
-00007770: 292c 2061 6e64 2063 6865 636b 696e 6720  ), and checking 
-00007780: 6966 2074 6865 206c 6973 7420 6973 2061  if the list is a
-00007790: 2073 7461 636b 2e20 0a0a 2020 2020 4172   stack. ..    Ar
-000077a0: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-000077b0: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-000077c0: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-000077d0: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-000077e0: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-000077f0: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-00007800: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-00007810: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-00007820: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-00007830: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-00007840: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-00007850: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-00007860: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-00007870: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-00007880: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-00007890: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-000078a0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-000078b0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-000078c0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-000078d0: 6561 6c73 6f3a 3a0a 2020 2020 2020 2020  ealso::.        
-000078e0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-000078f0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00007900: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00007910: 2e69 735f 7374 6163 6b60 0a0a 0a20 2020  .is_stack`...   
-00007920: 2022 2222 2020 2020 0a0a 2020 2020 6361   """    ..    ca
-00007930: 6e64 6964 6174 6573 203d 2063 7572 725f  ndidates = curr_
-00007940: 6361 6e64 7320 6966 2063 7572 725f 6361  cands if curr_ca
-00007950: 6e64 7320 6973 206e 6f74 204e 6f6e 6520  nds is not None 
-00007960: 656c 7365 2065 6461 7461 2e63 616e 6469  else edata.candi
-00007970: 6461 7465 730a 2020 2020 7769 6e6e 6572  dates.    winner
-00007980: 7320 3d20 6c69 7374 2829 0a20 2020 2066  s = list().    f
-00007990: 6f72 2063 6c69 7374 2069 6e20 7065 726d  or clist in perm
-000079a0: 7574 6174 696f 6e73 2863 616e 6469 6461  utations(candida
-000079b0: 7465 7329 3a20 0a20 2020 2020 2020 2069  tes): .        i
-000079c0: 7373 7461 636b 203d 2069 735f 7374 6163  sstack = is_stac
-000079d0: 6b28 6564 6174 612c 2063 6c69 7374 2c20  k(edata, clist, 
-000079e0: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-000079f0: 725f 6361 6e64 7329 0a20 2020 2020 2020  r_cands).       
-00007a00: 2069 6620 6973 7374 6163 6b3a 200a 2020   if isstack: .  
-00007a10: 2020 2020 2020 2020 2020 7769 6e6e 6572            winner
-00007a20: 732e 6170 7065 6e64 2863 6c69 7374 5b30  s.append(clist[0
-00007a30: 5d29 0a20 2020 2020 2020 2020 2020 200a  ]).            .
-00007a40: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
-00007a50: 6428 6c69 7374 2873 6574 2877 696e 6e65  d(list(set(winne
-00007a60: 7273 2929 290a 0a64 6566 205f 7261 6e6b  rs)))..def _rank
-00007a70: 6564 5f70 6169 7273 5f62 6173 6963 280a  ed_pairs_basic(.
-00007a80: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
-00007a90: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
-00007aa0: 652c 200a 2020 2020 7374 7265 6e67 7468  e, .    strength
-00007ab0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-00007ac0: 293a 2020 200a 2020 2020 2222 2241 6e20  ):   .    """An 
-00007ad0: 696d 706c 656d 656e 7461 7469 6f6e 206f  implementation o
-00007ae0: 6620 5261 6e6b 6564 2050 6169 7273 2074  f Ranked Pairs t
-00007af0: 6861 7420 7573 6573 2061 2062 6173 6963  hat uses a basic
-00007b00: 2061 6c67 6f72 6974 686d 2e20 0a0a 2020   algorithm. ..  
-00007b10: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00007b20: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
-00007b30: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
-00007b40: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
-00007b50: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
-00007b60: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
-00007b70: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
-00007b80: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-00007b90: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
-00007ba0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
-00007bb0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
-00007bc0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
-00007bd0: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
-00007be0: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
-00007bf0: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
-00007c00: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
-00007c10: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-00007c20: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-00007c30: 6469 6461 7465 732e 200a 0a20 2020 2022  didates. ..    "
-00007c40: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-00007c50: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00007c60: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00007c70: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00007c80: 6375 7272 5f63 616e 6473 200a 2020 2020  curr_cands .    
-00007c90: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
-00007ca0: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
-00007cb0: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-00007cc0: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-00007cd0: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
-00007ce0: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
-00007cf0: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
-00007d00: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-00007d10: 7d20 200a 2020 2020 7374 7265 6e67 7468  }  .    strength
-00007d20: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
-00007d30: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
-00007d40: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
-00007d50: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
-00007d60: 6774 685f 6675 6e63 7469 6f6e 2020 2020  gth_function    
-00007d70: 0a0a 2020 2020 6377 203d 2065 6461 7461  ..    cw = edata
-00007d80: 2e63 6f6e 646f 7263 6574 5f77 696e 6e65  .condorcet_winne
-00007d90: 7228 6375 7272 5f63 616e 6473 3d63 7572  r(curr_cands=cur
-00007da0: 725f 6361 6e64 7329 0a20 2020 2023 2052  r_cands).    # R
-00007db0: 616e 6b65 6420 5061 6972 7320 6973 2043  anked Pairs is C
-00007dc0: 6f6e 646f 7263 6574 2063 6f6e 7369 7374  ondorcet consist
-00007dd0: 656e 742c 2073 6f20 7369 6d70 6c79 2072  ent, so simply r
-00007de0: 6574 7572 6e20 7468 6520 436f 6e64 6f72  eturn the Condor
-00007df0: 6365 7420 7769 6e6e 6572 2069 6620 6578  cet winner if ex
-00007e00: 6973 7473 0a20 2020 2069 6620 6377 2069  ists.    if cw i
-00007e10: 7320 6e6f 7420 4e6f 6e65 3a20 0a20 2020  s not None: .   
-00007e20: 2020 2020 2077 696e 6e65 7273 203d 205b       winners = [
-00007e30: 6377 5d0a 2020 2020 656c 7365 3a0a 2020  cw].    else:.  
-00007e40: 2020 2020 2020 775f 6564 6765 7320 3d20        w_edges = 
-00007e50: 5b28 6331 2c20 6332 2c20 7374 7265 6e67  [(c1, c2, streng
-00007e60: 7468 5f66 756e 6374 696f 6e28 6331 2c20  th_function(c1, 
-00007e70: 6332 2929 2066 6f72 2063 3120 696e 2063  c2)) for c1 in c
-00007e80: 616e 6469 6461 7465 7320 666f 7220 6332  andidates for c2
-00007e90: 2069 6e20 6361 6e64 6964 6174 6573 200a   in candidates .
-00007ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007eb0: 2020 2069 6620 6331 2021 3d20 6332 2061     if c1 != c2 a
-00007ec0: 6e64 2028 6564 6174 612e 6d61 6a6f 7269  nd (edata.majori
-00007ed0: 7479 5f70 7265 6665 7273 2863 312c 2063  ty_prefers(c1, c
-00007ee0: 3229 206f 7220 6564 6174 612e 6973 5f74  2) or edata.is_t
-00007ef0: 6965 6428 6331 2c20 6332 2929 5d0a 2020  ied(c1, c2))].  
-00007f00: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
-00007f10: 6c69 7374 2829 2020 200a 2020 2020 2020  list()   .      
-00007f20: 2020 6966 206c 656e 2877 5f65 6467 6573    if len(w_edges
-00007f30: 2920 3e20 303a 2020 2020 2020 2020 2020  ) > 0:          
-00007f40: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00007f50: 656e 6774 6873 203d 2073 6f72 7465 6428  engths = sorted(
-00007f60: 6c69 7374 2873 6574 285b 655b 325d 2066  list(set([e[2] f
-00007f70: 6f72 2065 2069 6e20 775f 6564 6765 735d  or e in w_edges]
-00007f80: 2929 2c20 7265 7665 7273 653d 5472 7565  )), reverse=True
-00007f90: 290a 2020 2020 2020 2020 2020 2020 736f  ).            so
-00007fa0: 7274 6564 5f65 6467 6573 203d 205b 5b65  rted_edges = [[e
-00007fb0: 2066 6f72 2065 2069 6e20 775f 6564 6765   for e in w_edge
-00007fc0: 7320 6966 2065 5b32 5d20 3d3d 2073 5d20  s if e[2] == s] 
-00007fd0: 666f 7220 7320 696e 2073 7472 656e 6774  for s in strengt
-00007fe0: 6873 5d0a 2020 2020 2020 2020 2020 2020  hs].            
-00007ff0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
-00008000: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
-00008010: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
-00008020: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
-00008030: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008040: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
-00008050: 2020 2020 2020 2020 2020 2065 6467 6573             edges
-00008060: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
-00008070: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00008080: 705f 6465 6665 6174 203d 2053 504f 286c  p_defeat = SPO(l
-00008090: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
-000080a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000080b0: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
-000080c0: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
-000080d0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000080e0: 7420 7270 5f64 6566 6561 742e 505b 6361  t rp_defeat.P[ca
-000080f0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
-00008100: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
-00008110: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-00008120: 2020 2020 2020 2020 2020 2072 705f 6465             rp_de
-00008130: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-00008140: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-00008150: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-00008160: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
-00008170: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
-00008180: 746f 5f63 616e 645b 7270 5f64 6566 6561  to_cand[rp_defea
-00008190: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
-000081a0: 7473 2829 5b30 5d5d 290a 2020 2020 2020  ts()[0]]).      
-000081b0: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
-000081c0: 2020 2020 2077 696e 6e65 7273 203d 2063       winners = c
-000081d0: 616e 6469 6461 7465 730a 2020 2020 7265  andidates.    re
-000081e0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
-000081f0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
-00008200: 0a0a 7270 5f70 726f 7065 7274 6965 7320  ..rp_properties 
-00008210: 3d20 566f 7469 6e67 4d65 7468 6f64 5072  = VotingMethodPr
-00008220: 6f70 6572 7469 6573 280a 2020 2020 636f  operties(.    co
-00008230: 6e64 6f72 6365 745f 7769 6e6e 6572 3d54  ndorcet_winner=T
-00008240: 7275 652c 200a 2020 2020 636f 6e64 6f72  rue, .    condor
-00008250: 6365 745f 6c6f 7365 723d 5472 7565 2c0a  cet_loser=True,.
-00008260: 2020 2020 7061 7265 746f 5f64 6f6d 696e      pareto_domin
-00008270: 616e 6365 3d54 7275 652c 0a20 2020 2070  ance=True,.    p
-00008280: 6f73 6974 6976 655f 696e 766f 6c76 656d  ositive_involvem
-00008290: 656e 743d 4661 6c73 652c 200a 2020 2020  ent=False, .    
-000082a0: 290a 4076 6d28 6e61 6d65 3d22 5261 6e6b  ).@vm(name="Rank
-000082b0: 6564 2050 6169 7273 222c 0a20 2020 2070  ed Pairs",.    p
-000082c0: 726f 7065 7274 6965 733d 7270 5f70 726f  roperties=rp_pro
-000082d0: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
-000082e0: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
-000082f0: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
-00008300: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
-00008310: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
-00008320: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
-00008330: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
-00008340: 6566 2072 616e 6b65 645f 7061 6972 7328  ef ranked_pairs(
-00008350: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-00008360: 2063 7572 725f 6361 6e64 733d 4e6f 6e65   curr_cands=None
-00008370: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
-00008380: 6675 6e63 7469 6f6e 3d4e 6f6e 652c 200a  function=None, .
-00008390: 2020 2020 616c 676f 7269 7468 6d3d 2762      algorithm='b
-000083a0: 6173 6963 2729 3a20 2020 0a20 2020 2022  asic'):   .    "
-000083b0: 2222 0a20 2020 204f 7264 6572 2074 6865  "".    Order the
-000083c0: 2065 6467 6573 2069 6e20 7468 6520 6d61   edges in the ma
-000083d0: 7267 696e 2067 7261 7068 2066 726f 6d20  rgin graph from 
-000083e0: 6c61 7267 6573 7420 746f 2073 6d61 6c6c  largest to small
-000083f0: 6573 7420 616e 6420 6c6f 636b 2074 6865  est and lock the
-00008400: 6d20 696e 2069 6e20 7468 6174 206f 7264  m in in that ord
-00008410: 6572 2c20 736b 6970 7069 6e67 2065 6467  er, skipping edg
-00008420: 6573 2074 6861 7420 6372 6561 7465 2061  es that create a
-00008430: 2063 7963 6c65 2e20 2049 6620 7468 6572   cycle.  If ther
-00008440: 6520 6172 6520 7469 6573 2069 6e20 7468  e are ties in th
-00008450: 6520 6d61 7267 696e 732c 2062 7265 616b  e margins, break
-00008460: 2074 6865 2074 6965 7320 7573 696e 6720   the ties using 
-00008470: 6120 7469 652d 6272 6561 6b69 6e67 2072  a tie-breaking r
-00008480: 756c 653a 2061 206c 696e 6561 7220 6f72  ule: a linear or
-00008490: 6465 7269 6e67 206f 7665 7220 7468 6520  dering over the 
-000084a0: 6564 6765 732e 2020 2041 2063 616e 6469  edges.   A candi
-000084b0: 6461 7465 2069 7320 6120 5261 6e6b 6564  date is a Ranked
-000084c0: 2050 6169 7273 2077 696e 6e65 7220 6966   Pairs winner if
-000084d0: 2069 7420 7769 6e73 2061 6363 6f72 6469   it wins accordi
-000084e0: 6e67 2074 6f20 736f 6d65 2074 6965 2d62  ng to some tie-b
-000084f0: 7265 616b 696e 6720 7275 6c65 2e20 416c  reaking rule. Al
-00008500: 736f 206b 6e6f 776e 2061 7320 5469 6465  so known as Tide
-00008510: 6d61 6e27 7320 5275 6c65 2e0a 0a20 2020  man's Rule...   
-00008520: 202e 2e20 7761 726e 696e 673a 3a20 0a20   .. warning:: . 
-00008530: 2020 2020 2020 2054 6869 7320 6d65 7468         This meth
-00008540: 6f64 2063 616e 2074 616b 6520 6120 7665  od can take a ve
-00008550: 7279 206c 6f6e 6720 7469 6d65 2074 6f20  ry long time to 
-00008560: 6669 6e64 2077 696e 6e65 7273 2e20 0a20  find winners. . 
-00008570: 2020 2020 2020 200a 2020 2020 4172 6773         .    Args
-00008580: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
-00008590: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
-000085a0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
-000085b0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
-000085c0: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
-000085d0: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
-000085e0: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
-000085f0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
-00008600: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-00008610: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
-00008620: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
-00008630: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
-00008640: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
-00008650: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
-00008660: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
-00008670: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
-00008680: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
-00008690: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
-000086a0: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
-000086b0: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
-000086c0: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
-000086d0: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
-000086e0: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
-000086f0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
-00008700: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
-00008710: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
-00008720: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
-00008730: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
-00008740: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
-00008750: 2e20 0a20 2020 2020 2020 2061 6c67 6f72  . .        algor
-00008760: 6974 686d 2028 7374 722c 206f 7074 696f  ithm (str, optio
-00008770: 6e61 6c29 3a20 5370 6563 6966 7920 7768  nal): Specify wh
-00008780: 6963 6820 616c 676f 7269 7468 6d20 746f  ich algorithm to
-00008790: 2075 7365 2e20 204f 7074 696f 6e73 2061   use.  Options a
-000087a0: 7265 2027 6261 7369 6327 2028 7468 6520  re 'basic' (the 
-000087b0: 6465 6661 756c 7429 2061 6e64 2027 6672  default) and 'fr
-000087c0: 6f6d 5f73 7461 636b 7327 2e0a 0a20 2020  om_stacks'...   
-000087d0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-000087e0: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-000087f0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-00008800: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-00008810: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-00008820: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-00008830: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-00008840: 6f64 732e 7261 6e6b 6564 5f70 6169 7273  ods.ranked_pairs
-00008850: 5f77 6974 685f 7465 7374 602c 203a 6d65  _with_test`, :me
-00008860: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
-00008870: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
-00008880: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
-00008890: 735f 7a74 602c 203a 6d65 7468 3a60 7072  s_zt`, :meth:`pr
-000088a0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-000088b0: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-000088c0: 616e 6b65 645f 7061 6972 735f 6465 6665  anked_pairs_defe
-000088d0: 6174 7360 0a0a 2020 2020 3a45 7861 6d70  ats`..    :Examp
-000088e0: 6c65 3a20 0a0a 2020 2020 2e2e 2070 6c6f  le: ..    .. plo
-000088f0: 743a 3a20 206d 6172 6769 6e5f 6772 6170  t::  margin_grap
-00008900: 6873 5f65 7861 6d70 6c65 732f 6d67 5f65  hs_examples/mg_e
-00008910: 785f 6270 5f72 702e 7079 0a20 2020 2020  x_bp_rp.py.     
-00008920: 2020 203a 636f 6e74 6578 743a 2072 6573     :context: res
-00008930: 6574 2020 0a20 2020 2020 2020 203a 696e  et  .        :in
-00008940: 636c 7564 652d 736f 7572 6365 3a20 5472  clude-source: Tr
-00008950: 7565 0a0a 0a20 2020 202e 2e20 636f 6465  ue...    .. code
-00008960: 2d62 6c6f 636b 3a3a 200a 0a20 2020 2020  -block:: ..     
-00008970: 2020 2066 726f 6d20 7072 6566 5f76 6f74     from pref_vot
-00008980: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-00008990: 5f6d 6574 686f 6473 2069 6d70 6f72 7420  _methods import 
-000089a0: 7261 6e6b 6564 5f70 6169 7273 0a0a 2020  ranked_pairs..  
-000089b0: 2020 2020 2020 7261 6e6b 6564 5f70 6169        ranked_pai
-000089c0: 7273 2e64 6973 706c 6179 286d 6729 0a20  rs.display(mg). 
-000089d0: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
-000089e0: 6972 732e 6469 7370 6c61 7928 6d67 2c20  irs.display(mg, 
-000089f0: 616c 676f 7269 7468 6d3d 2762 6173 6963  algorithm='basic
-00008a00: 2729 200a 2020 2020 2020 2020 7261 6e6b  ') .        rank
-00008a10: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
-00008a20: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-00008a30: 6672 6f6d 5f73 7461 636b 7327 2920 2020  from_stacks')   
-00008a40: 200a 0a0a 2020 2020 2e2e 2065 7865 635f   ...    .. exec_
-00008a50: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
-00008a60: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
-00008a70: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00008a80: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
-00008a90: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
-00008aa0: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
-00008ab0: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
-00008ac0: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00008ad0: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
-00008ae0: 696d 706f 7274 2072 616e 6b65 645f 7061  import ranked_pa
-00008af0: 6972 730a 2020 2020 2020 2020 0a20 2020  irs.        .   
-00008b00: 2020 2020 206d 6720 3d20 4d61 7267 696e       mg = Margin
-00008b10: 4772 6170 6828 5b30 2c20 312c 2032 2c20  Graph([0, 1, 2, 
-00008b20: 335d 2c20 5b28 302c 2032 2c20 3329 2c20  3], [(0, 2, 3), 
-00008b30: 2831 2c20 302c 2035 292c 2028 322c 2031  (1, 0, 5), (2, 1
-00008b40: 2c20 3529 2c20 2832 2c20 332c 2031 292c  , 5), (2, 3, 1),
-00008b50: 2028 332c 2030 2c20 3329 2c20 2833 2c20   (3, 0, 3), (3, 
-00008b60: 312c 2031 295d 290a 2020 2020 2020 2020  1, 1)]).        
-00008b70: 0a20 2020 2020 2020 2072 616e 6b65 645f  .        ranked_
-00008b80: 7061 6972 732e 6469 7370 6c61 7928 6d67  pairs.display(mg
-00008b90: 290a 2020 2020 2020 2020 7261 6e6b 6564  ).        ranked
-00008ba0: 5f70 6169 7273 2e64 6973 706c 6179 286d  _pairs.display(m
-00008bb0: 672c 2061 6c67 6f72 6974 686d 3d27 6261  g, algorithm='ba
-00008bc0: 7369 6327 290a 2020 2020 2020 2020 7261  sic').        ra
-00008bd0: 6e6b 6564 5f70 6169 7273 2e64 6973 706c  nked_pairs.displ
-00008be0: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
-00008bf0: 3d27 6672 6f6d 5f73 7461 636b 7327 290a  ='from_stacks').
-00008c00: 0a20 2020 2022 2222 0a0a 2020 2020 6966  .    """..    if
-00008c10: 2061 6c67 6f72 6974 686d 203d 3d20 2762   algorithm == 'b
-00008c20: 6173 6963 273a 0a20 2020 2020 2020 2072  asic':.        r
-00008c30: 6574 7572 6e20 5f72 616e 6b65 645f 7061  eturn _ranked_pa
-00008c40: 6972 735f 6261 7369 6328 6564 6174 612c  irs_basic(edata,
-00008c50: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00008c60: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-00008c70: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-00008c80: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-00008c90: 0a20 2020 2065 6c69 6620 616c 676f 7269  .    elif algori
-00008ca0: 7468 6d20 3d3d 2027 6672 6f6d 5f73 7461  thm == 'from_sta
-00008cb0: 636b 7327 3a0a 2020 2020 2020 2020 7265  cks':.        re
-00008cc0: 7475 726e 205f 7261 6e6b 6564 5f70 6169  turn _ranked_pai
-00008cd0: 7273 5f66 726f 6d5f 7374 6163 6b73 2865  rs_from_stacks(e
-00008ce0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00008cf0: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
-00008d00: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-00008d10: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-00008d20: 7228 2249 6e76 616c 6964 2061 6c67 6f72  r("Invalid algor
-00008d30: 6974 686d 2073 7065 6369 6669 6564 2e22  ithm specified."
-00008d40: 290a 0a40 766d 286e 616d 653d 2252 616e  )..@vm(name="Ran
-00008d50: 6b65 6420 5061 6972 7322 2c0a 2020 2020  ked Pairs",.    
-00008d60: 736b 6970 5f72 6567 6973 7472 6174 696f  skip_registratio
-00008d70: 6e3d 5472 7565 290a 6465 6620 7261 6e6b  n=True).def rank
-00008d80: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
-00008d90: 7374 280a 2020 2020 6564 6174 612c 200a  st(.    edata, .
-00008da0: 2020 2020 6375 7272 5f63 616e 6473 3d4e      curr_cands=N
-00008db0: 6f6e 652c 200a 2020 2020 7374 7265 6e67  one, .    streng
-00008dc0: 7468 5f66 756e 6374 696f 6e3d 4e6f 6e65  th_function=None
-00008dd0: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
-00008de0: 6420 7468 6520 5261 6e6b 6564 2050 6169  d the Ranked Pai
-00008df0: 7273 2077 696e 6e65 7273 2c20 6275 7420  rs winners, but 
-00008e00: 696e 636c 7564 6520 6120 7465 7374 2074  include a test t
-00008e10: 6f20 6465 7465 726d 696e 6564 2069 6620  o determined if 
-00008e20: 6974 2077 696c 6c20 7461 6b65 2074 6f6f  it will take too
-00008e30: 206c 6f6e 6720 746f 2063 6f6d 7075 7465   long to compute
-00008e40: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
-00008e50: 7320 7769 6e6e 6572 732e 2049 6620 7468  s winners. If th
-00008e60: 6520 6361 6c63 756c 6174 696f 6e20 6f66  e calculation of
-00008e70: 2074 6865 2077 696e 6e65 7273 2077 696c   the winners wil
-00008e80: 6c20 7461 6b65 2074 6f6f 206c 6f6e 672c  l take too long,
-00008e90: 2072 6574 7572 6e20 4e6f 6e65 2e0a 0a20   return None... 
-00008ea0: 2020 202e 2e20 696d 706f 7274 616e 743a     .. important:
-00008eb0: 3a0a 2020 2020 2020 2020 5468 6973 2076  :.        This v
-00008ec0: 6f74 696e 6720 6d65 7468 6f64 2074 6861  oting method tha
-00008ed0: 7420 6d69 6768 7420 7265 7475 726e 204e  t might return N
-00008ee0: 6f6e 6520 7261 7468 6572 2074 6861 6e20  one rather than 
-00008ef0: 6120 6c69 7374 206f 6620 6361 6e64 6964  a list of candid
-00008f00: 6174 6573 2e20 200a 0a20 2020 2041 7267  ates.  ..    Arg
-00008f10: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00008f20: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00008f30: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00008f40: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00008f50: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00008f60: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00008f70: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-00008f80: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00008f90: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00008fa0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00008fb0: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00008fc0: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00008fd0: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00008fe0: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00008ff0: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00009000: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00009010: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-00009020: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-00009030: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-00009040: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-00009050: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00009060: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-00009070: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-00009080: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-00009090: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-000090a0: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-000090b0: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-000090c0: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-000090d0: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-000090e0: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-000090f0: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00009100: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00009110: 6964 6174 6573 2e20 0a0a 2020 2020 2e2e  idates. ..    ..
-00009120: 2073 6565 616c 736f 3a3a 0a0a 2020 2020   seealso::..    
-00009130: 2020 2020 3a6d 6574 683a 6070 7265 665f      :meth:`pref_
-00009140: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00009150: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
-00009160: 6564 5f70 6169 7273 5f77 6974 685f 7465  ed_pairs_with_te
-00009170: 7374 602c 203a 6d65 7468 3a60 7072 6566  st`, :meth:`pref
-00009180: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
-00009190: 6173 6564 5f6d 6574 686f 6473 2e72 616e  ased_methods.ran
-000091a0: 6b65 645f 7061 6972 735f 7a74 602c 203a  ked_pairs_zt`, :
-000091b0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-000091c0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-000091d0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-000091e0: 6972 735f 6465 6665 6174 7360 0a0a 2020  irs_defeats`..  
-000091f0: 2020 3a45 7861 6d70 6c65 3a20 0a0a 2020    :Example: ..  
-00009200: 2020 2e2e 2070 6c6f 743a 3a20 206d 6172    .. plot::  mar
-00009210: 6769 6e5f 6772 6170 6873 5f65 7861 6d70  gin_graphs_examp
-00009220: 6c65 732f 6d67 5f65 785f 7270 5f77 6974  les/mg_ex_rp_wit
-00009230: 685f 7465 7374 2e70 790a 2020 2020 2020  h_test.py.      
-00009240: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
-00009250: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
-00009260: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
-00009270: 650a 0a0a 2020 2020 2e2e 2063 6f64 652d  e...    .. code-
-00009280: 626c 6f63 6b3a 3a20 0a0a 2020 2020 2020  block:: ..      
-00009290: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
-000092a0: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-000092b0: 6d65 7468 6f64 7320 696d 706f 7274 2072  methods import r
-000092c0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-000092d0: 5f74 6573 740a 0a20 2020 2020 2020 2072  _test..        r
-000092e0: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-000092f0: 5f74 6573 742e 6469 7370 6c61 7928 6d67  _test.display(mg
-00009300: 290a 0a0a 2020 2020 2e2e 2065 7865 635f  )...    .. exec_
-00009310: 636f 6465 3a3a 200a 2020 2020 2020 2020  code:: .        
-00009320: 3a68 6964 655f 636f 6465 3a0a 0a20 2020  :hide_code:..   
-00009330: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-00009340: 6f74 696e 672e 7765 6967 6874 6564 5f6d  oting.weighted_m
-00009350: 616a 6f72 6974 795f 6772 6170 6873 2069  ajority_graphs i
-00009360: 6d70 6f72 7420 4d61 7267 696e 4772 6170  mport MarginGrap
-00009370: 680a 2020 2020 2020 2020 6672 6f6d 2070  h.        from p
-00009380: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-00009390: 6e5f 6261 7365 645f 6d65 7468 6f64 7320  n_based_methods 
-000093a0: 696d 706f 7274 2072 616e 6b65 645f 7061  import ranked_pa
-000093b0: 6972 735f 7769 7468 5f74 6573 740a 2020  irs_with_test.  
-000093c0: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
-000093d0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
-000093e0: 5b30 2c20 312c 2032 2c20 335d 2c20 5b28  [0, 1, 2, 3], [(
-000093f0: 312c 2032 2c20 3229 2c20 2831 2c20 332c  1, 2, 2), (1, 3,
-00009400: 2032 292c 2028 322c 2030 2c20 3229 5d29   2), (2, 0, 2)])
-00009410: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00009420: 2020 7261 6e6b 6564 5f70 6169 7273 5f77    ranked_pairs_w
-00009430: 6974 685f 7465 7374 2e64 6973 706c 6179  ith_test.display
-00009440: 286d 6729 0a0a 0a20 2020 2022 2222 2020  (mg)...    """  
-00009450: 2020 0a20 2020 2063 616e 6469 6461 7465    .    candidate
-00009460: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00009470: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00009480: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00009490: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
-000094a0: 2020 2063 6964 785f 746f 5f63 616e 6420     cidx_to_cand 
-000094b0: 3d20 7b63 6964 783a 2063 2066 6f72 2063  = {cidx: c for c
-000094c0: 6964 782c 2063 2069 6e20 656e 756d 6572  idx, c in enumer
-000094d0: 6174 6528 6361 6e64 6964 6174 6573 297d  ate(candidates)}
-000094e0: 2020 0a20 2020 2063 616e 645f 746f 5f63    .    cand_to_c
-000094f0: 6964 7820 3d20 7b63 3a20 6369 6478 2066  idx = {c: cidx f
-00009500: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
-00009510: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
-00009520: 6573 297d 2020 0a20 2020 200a 2020 2020  es)}  .    .    
-00009530: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-00009540: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
-00009550: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
-00009560: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
-00009570: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
-00009580: 7469 6f6e 2020 200a 0a20 2020 2063 7720  tion   ..    cw 
-00009590: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
-000095a0: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
-000095b0: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-000095c0: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
-000095d0: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
-000095e0: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
-000095f0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
-00009600: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
-00009610: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
-00009620: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
-00009630: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
-00009640: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
-00009650: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
-00009660: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
-00009670: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
-00009680: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
-00009690: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
-000096a0: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
-000096b0: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
-000096c0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000096d0: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
-000096e0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-000096f0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
-00009700: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
-00009710: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
-00009720: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
-00009730: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00009740: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
-00009750: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
-00009760: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
-00009770: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
-00009780: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
-00009790: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
-000097a0: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
-000097b0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
-000097c0: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
-000097d0: 6e67 7468 735d 0a20 2020 2020 2020 2069  ngths].        i
-000097e0: 6620 6e70 2e70 726f 6428 5b6d 6174 682e  f np.prod([math.
-000097f0: 6661 6374 6f72 6961 6c28 6c65 6e28 6573  factorial(len(es
-00009800: 2929 2066 6f72 2065 7320 696e 2073 6f72  )) for es in sor
-00009810: 7465 645f 6564 6765 735d 2920 3e20 3330  ted_edges]) > 30
-00009820: 3030 3a20 0a20 2020 2020 2020 2020 2020  00: .           
-00009830: 2072 6574 7572 6e20 4e6f 6e65 0a20 2020   return None.   
-00009840: 2020 2020 2065 6c73 653a 200a 2020 2020       else: .    
-00009850: 2020 2020 2020 2020 7462 7320 3d20 7072          tbs = pr
-00009860: 6f64 7563 7428 2a5b 7065 726d 7574 6174  oduct(*[permutat
-00009870: 696f 6e73 2865 6467 6573 2920 666f 7220  ions(edges) for 
-00009880: 6564 6765 7320 696e 2073 6f72 7465 645f  edges in sorted_
-00009890: 6564 6765 735d 290a 2020 2020 2020 2020  edges]).        
-000098a0: 2020 2020 666f 7220 7462 2069 6e20 7462      for tb in tb
-000098b0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000098c0: 2020 2065 6467 6573 203d 2066 6c61 7474     edges = flatt
-000098d0: 656e 2874 6229 0a20 2020 2020 2020 2020  en(tb).         
-000098e0: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-000098f0: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
-00009900: 6461 7465 7329 290a 2020 2020 2020 2020  dates)).        
-00009910: 2020 2020 2020 2020 666f 7220 6530 2c65          for e0,e
-00009920: 312c 7320 696e 2065 6467 6573 3a20 0a20  1,s in edges: . 
-00009930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009940: 2020 2069 6620 6e6f 7420 7270 5f64 6566     if not rp_def
-00009950: 6561 742e 505b 6361 6e64 5f74 6f5f 6369  eat.P[cand_to_ci
-00009960: 6478 5b65 315d 5d5b 6361 6e64 5f74 6f5f  dx[e1]][cand_to_
-00009970: 6369 6478 5b65 305d 5d3a 0a20 2020 2020  cidx[e0]]:.     
-00009980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009990: 2020 2072 705f 6465 6665 6174 2e61 6464     rp_defeat.add
-000099a0: 2863 616e 645f 746f 5f63 6964 785b 6530  (cand_to_cidx[e0
-000099b0: 5d2c 6361 6e64 5f74 6f5f 6369 6478 5b65  ],cand_to_cidx[e
-000099c0: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-000099d0: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
-000099e0: 6e64 2863 6964 785f 746f 5f63 616e 645b  nd(cidx_to_cand[
-000099f0: 7270 5f64 6566 6561 742e 696e 6974 6961  rp_defeat.initia
-00009a00: 6c5f 656c 656d 656e 7473 2829 5b30 5d5d  l_elements()[0]]
-00009a10: 290a 2020 2020 7265 7475 726e 2073 6f72  ).    return sor
-00009a20: 7465 6428 6c69 7374 2873 6574 2877 696e  ted(list(set(win
-00009a30: 6e65 7273 2929 290a 0a64 6566 2072 616e  ners)))..def ran
-00009a40: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
-00009a50: 7328 6564 6174 612c 2063 7572 725f 6361  s(edata, curr_ca
-00009a60: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
-00009a70: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-00009a80: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
-00009a90: 220a 2020 2020 5265 7475 726e 7320 7468  ".    Returns th
-00009aa0: 6520 5261 6e6b 6564 2050 6169 7273 2064  e Ranked Pairs d
-00009ab0: 6566 6561 7420 7265 6c61 7469 6f6e 7320  efeat relations 
-00009ac0: 7072 6f64 7563 6564 2062 7920 7468 6520  produced by the 
-00009ad0: 5261 6e6b 6564 2050 6169 7273 2061 6c67  Ranked Pairs alg
-00009ae0: 6f72 6974 686d 2e20 0a0a 2020 2020 2e2e  orithm. ..    ..
-00009af0: 2069 6d70 6f72 7461 6e74 3a3a 0a20 2020   important::.   
-00009b00: 2020 2020 2055 6e6c 696b 6520 7468 6520       Unlike the 
-00009b10: 6f74 6865 7220 6675 6e63 7469 6f6e 7320  other functions 
-00009b20: 7468 6174 2072 6574 7572 6e20 6120 7369  that return a si
-00009b30: 6e67 6c65 2064 6566 6561 7420 7265 6c61  ngle defeat rela
-00009b40: 7469 6f6e 2c20 7468 6973 2072 6574 7572  tion, this retur
-00009b50: 6e73 2061 206c 6973 7420 6f66 2064 6566  ns a list of def
-00009b60: 6561 7420 7265 6c61 7469 6f6e 732e 200a  eat relations. .
-00009b70: 2020 2020 2020 2020 0a20 2020 2041 7267          .    Arg
-00009b80: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-00009b90: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-00009ba0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-00009bb0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-00009bc0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-00009bd0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-00009be0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-00009bf0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-00009c00: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-00009c10: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-00009c20: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-00009c30: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-00009c40: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-00009c50: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-00009c60: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-00009c70: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-00009c80: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-00009c90: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-00009ca0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-00009cb0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-00009cc0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-00009cd0: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-00009ce0: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-00009cf0: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-00009d00: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-00009d10: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-00009d20: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-00009d30: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-00009d40: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-00009d50: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-00009d60: 3a20 0a20 2020 2020 2020 2041 206e 6574  : .        A net
-00009d70: 776f 726b 7820 4469 4772 6170 6820 7265  workx DiGraph re
-00009d80: 7072 6573 656e 7469 6e67 2074 6865 2052  presenting the R
-00009d90: 616e 6b65 6420 5061 6972 7320 6465 6665  anked Pairs defe
-00009da0: 6174 2072 656c 6174 696f 6e2e 200a 0a20  at relation. .. 
-00009db0: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
-00009dc0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-00009dd0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-00009de0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-00009df0: 2e72 616e 6b65 645f 7061 6972 7360 2c20  .ranked_pairs`, 
-00009e00: 3a6d 6574 683a 6070 7265 665f 766f 7469  :meth:`pref_voti
-00009e10: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-00009e20: 6d65 7468 6f64 732e 7261 6e6b 6564 5f70  methods.ranked_p
-00009e30: 6169 7273 5f77 6974 685f 7465 7374 600a  airs_with_test`.
-00009e40: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-00009e50: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
-00009e60: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
-00009e70: 616d 706c 6573 2f6d 675f 6578 5f72 705f  amples/mg_ex_rp_
-00009e80: 6465 6665 6174 732e 7079 0a20 2020 2020  defeats.py.     
-00009e90: 2020 203a 636f 6e74 6578 743a 2072 6573     :context: res
-00009ea0: 6574 2020 0a20 2020 2020 2020 203a 696e  et  .        :in
-00009eb0: 636c 7564 652d 736f 7572 6365 3a20 5472  clude-source: Tr
-00009ec0: 7565 0a0a 2020 2020 2e2e 2065 7865 635f  ue..    .. exec_
-00009ed0: 636f 6465 3a3a 0a0a 0a20 2020 2020 2020  code::...       
-00009ee0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
-00009ef0: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
-00009f00: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
-00009f10: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
-00009f20: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-00009f30: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-00009f40: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-00009f50: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
-00009f60: 6465 6665 6174 730a 0a20 2020 2020 2020  defeats..       
-00009f70: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
-00009f80: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
-00009f90: 5b28 302c 2031 2c20 3130 292c 2028 302c  [(0, 1, 10), (0,
-00009fa0: 2032 2c20 3229 2c20 2831 2c20 332c 2034   2, 2), (1, 3, 4
-00009fb0: 292c 2028 322c 2031 2c20 3629 2c20 2832  ), (2, 1, 6), (2
-00009fc0: 2c20 332c 2038 292c 2028 332c 2030 2c20  , 3, 8), (3, 0, 
-00009fd0: 3429 5d29 0a20 2020 2020 2020 2072 705f  4)]).        rp_
-00009fe0: 6465 6665 6174 7320 3d20 7261 6e6b 6564  defeats = ranked
-00009ff0: 5f70 6169 7273 5f64 6566 6561 7473 286d  _pairs_defeats(m
-0000a000: 6729 0a0a 2020 2020 2020 2020 666f 7220  g)..        for 
-0000a010: 7270 6420 696e 2072 705f 6465 6665 6174  rpd in rp_defeat
-0000a020: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
-0000a030: 7072 696e 7428 7270 642e 6564 6765 7329  print(rpd.edges)
-0000a040: 0a0a 2020 2020 2222 220a 2020 2020 0a20  ..    """.    . 
-0000a050: 2020 2063 616e 6469 6461 7465 7320 3d20     candidates = 
-0000a060: 6564 6174 612e 6361 6e64 6964 6174 6573  edata.candidates
-0000a070: 2069 6620 6375 7272 5f63 616e 6473 2069   if curr_cands i
-0000a080: 7320 4e6f 6e65 2065 6c73 6520 6375 7272  s None else curr
-0000a090: 5f63 616e 6473 2020 2020 0a20 2020 2073  _cands    .    s
-0000a0a0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000a0b0: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
-0000a0c0: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
-0000a0d0: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
-0000a0e0: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
-0000a0f0: 696f 6e20 2020 200a 0a20 2020 2077 5f65  ion    ..    w_e
-0000a100: 6467 6573 203d 205b 2863 312c 2063 322c  dges = [(c1, c2,
-0000a110: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000a120: 6f6e 2863 312c 2063 3229 2920 666f 7220  on(c1, c2)) for 
-0000a130: 6331 2069 6e20 6361 6e64 6964 6174 6573  c1 in candidates
-0000a140: 2066 6f72 2063 3220 696e 2063 616e 6469   for c2 in candi
-0000a150: 6461 7465 7320 6966 2063 3120 213d 2063  dates if c1 != c
-0000a160: 3220 616e 6420 2865 6461 7461 2e6d 616a  2 and (edata.maj
-0000a170: 6f72 6974 795f 7072 6566 6572 7328 6331  ority_prefers(c1
-0000a180: 2c20 6332 2920 6f72 2065 6461 7461 2e69  , c2) or edata.i
-0000a190: 735f 7469 6564 2863 312c 2063 3229 295d  s_tied(c1, c2))]
-0000a1a0: 0a20 2020 2077 696e 6e65 7273 203d 206c  .    winners = l
-0000a1b0: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
-0000a1c0: 200a 2020 2020 7374 7265 6e67 7468 7320   .    strengths 
-0000a1d0: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
-0000a1e0: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
-0000a1f0: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
-0000a200: 6572 7365 3d54 7275 6529 0a20 2020 2073  erse=True).    s
-0000a210: 6f72 7465 645f 6564 6765 7320 3d20 5b5b  orted_edges = [[
-0000a220: 6520 666f 7220 6520 696e 2077 5f65 6467  e for e in w_edg
-0000a230: 6573 2069 6620 655b 325d 203d 3d20 735d  es if e[2] == s]
-0000a240: 2066 6f72 2073 2069 6e20 7374 7265 6e67   for s in streng
-0000a250: 7468 735d 0a20 2020 2074 6273 203d 2070  ths].    tbs = p
-0000a260: 726f 6475 6374 282a 5b70 6572 6d75 7461  roduct(*[permuta
-0000a270: 7469 6f6e 7328 6564 6765 7329 2066 6f72  tions(edges) for
-0000a280: 2065 6467 6573 2069 6e20 736f 7274 6564   edges in sorted
-0000a290: 5f65 6467 6573 5d29 0a20 2020 2072 705f  _edges]).    rp_
-0000a2a0: 6465 6665 6174 7320 3d20 6c69 7374 2829  defeats = list()
-0000a2b0: 0a20 2020 2066 6f72 2074 6220 696e 2074  .    for tb in t
-0000a2c0: 6273 3a0a 2020 2020 2020 2020 6564 6765  bs:.        edge
-0000a2d0: 7320 3d20 666c 6174 7465 6e28 7462 290a  s = flatten(tb).
-0000a2e0: 2020 2020 2020 2020 7270 5f64 6566 6561          rp_defea
-0000a2f0: 7420 3d20 6e78 2e44 6947 7261 7068 2829  t = nx.DiGraph()
-0000a300: 200a 2020 2020 2020 2020 666f 7220 6520   .        for e 
-0000a310: 696e 2065 6467 6573 3a20 0a20 2020 2020  in edges: .     
-0000a320: 2020 2020 2020 2072 705f 6465 6665 6174         rp_defeat
-0000a330: 2e61 6464 5f65 6467 6528 655b 305d 2c20  .add_edge(e[0], 
-0000a340: 655b 315d 2c20 7765 6967 6874 3d65 5b32  e[1], weight=e[2
-0000a350: 5d29 0a20 2020 2020 2020 2020 2020 2069  ]).            i
-0000a360: 6620 646f 6573 5f63 7265 6174 655f 6379  f does_create_cy
-0000a370: 636c 6528 7270 5f64 6566 6561 742c 2065  cle(rp_defeat, e
-0000a380: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000a390: 2020 2072 705f 6465 6665 6174 2e72 656d     rp_defeat.rem
-0000a3a0: 6f76 655f 6564 6765 2865 5b30 5d2c 2065  ove_edge(e[0], e
-0000a3b0: 5b31 5d29 0a20 2020 2020 2020 2072 705f  [1]).        rp_
-0000a3c0: 6465 6665 6174 732e 6170 7065 6e64 2872  defeats.append(r
-0000a3d0: 705f 6465 6665 6174 290a 2020 2020 2020  p_defeat).      
-0000a3e0: 2020 7769 6e6e 6572 732e 6170 7065 6e64    winners.append
-0000a3f0: 286d 6178 696d 616c 5f65 6c65 6d65 6e74  (maximal_element
-0000a400: 7328 7270 5f64 6566 6561 7429 5b30 5d29  s(rp_defeat)[0])
-0000a410: 0a20 2020 2072 6574 7572 6e20 7270 5f64  .    return rp_d
-0000a420: 6566 6561 7473 0a0a 7270 5f74 625f 7072  efeats..rp_tb_pr
-0000a430: 6f70 6572 7469 6573 203d 2056 6f74 696e  operties = Votin
-0000a440: 674d 6574 686f 6450 726f 7065 7274 6965  gMethodPropertie
-0000a450: 7328 0a20 2020 2063 6f6e 646f 7263 6574  s(.    condorcet
-0000a460: 5f77 696e 6e65 723d 5472 7565 2c20 0a20  _winner=True, . 
-0000a470: 2020 2063 6f6e 646f 7263 6574 5f6c 6f73     condorcet_los
-0000a480: 6572 3d54 7275 652c 0a20 2020 2070 6172  er=True,.    par
-0000a490: 6574 6f5f 646f 6d69 6e61 6e63 653d 5472  eto_dominance=Tr
-0000a4a0: 7565 2c0a 2020 2020 706f 7369 7469 7665  ue,.    positive
-0000a4b0: 5f69 6e76 6f6c 7665 6d65 6e74 3d46 616c  _involvement=Fal
-0000a4c0: 7365 2c20 0a20 2020 2029 0a40 766d 286e  se, .    ).@vm(n
-0000a4d0: 616d 653d 2252 616e 6b65 6420 5061 6972  ame="Ranked Pair
-0000a4e0: 7320 5442 222c 0a20 2020 2070 726f 7065  s TB",.    prope
-0000a4f0: 7274 6965 733d 7270 5f74 625f 7072 6f70  rties=rp_tb_prop
-0000a500: 6572 7469 6573 2c0a 2020 2020 696e 7075  erties,.    inpu
-0000a510: 745f 7479 7065 733d 5b45 6c65 6374 696f  t_types=[Electio
-0000a520: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
-0000a530: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-0000a540: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
-0000a550: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
-0000a560: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
-0000a570: 6620 7261 6e6b 6564 5f70 6169 7273 5f74  f ranked_pairs_t
-0000a580: 6228 0a20 2020 2065 6461 7461 2c20 0a20  b(.    edata, . 
-0000a590: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-0000a5a0: 4e6f 6e65 2c20 0a20 2020 2074 6965 5f62  None, .    tie_b
-0000a5b0: 7265 616b 6572 203d 204e 6f6e 652c 200a  reaker = None, .
-0000a5c0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-0000a5d0: 6374 696f 6e20 3d20 4e6f 6e65 293a 2020  ction = None):  
-0000a5e0: 200a 2020 2020 2222 220a 2020 2020 5261   .    """.    Ra
-0000a5f0: 6e6b 6564 2050 6169 7273 2077 6974 6820  nked Pairs with 
-0000a600: 6120 6669 7865 6420 6c69 6e65 6172 206f  a fixed linear o
-0000a610: 7264 6572 206f 6e20 7468 6520 6361 6e64  rder on the cand
-0000a620: 6964 6174 6573 2074 6f20 6272 6561 6b20  idates to break 
-0000a630: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
-0000a640: 6d61 7267 696e 732e 2020 200a 2020 2020  margins.   .    
-0000a650: 5369 6e63 6520 7468 6520 7469 655f 6272  Since the tie_br
-0000a660: 6561 6b65 7220 6973 2061 206c 696e 6561  eaker is a linea
-0000a670: 7220 6f72 6465 722c 2074 6869 7320 6d65  r order, this me
-0000a680: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
-0000a690: 2e20 2020 0a0a 2020 2020 4172 6773 3a0a  .   ..    Args:.
-0000a6a0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-0000a6b0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-0000a6c0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-0000a6d0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-0000a6e0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-0000a6f0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-0000a700: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-0000a710: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-0000a720: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-0000a730: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-0000a740: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-0000a750: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-0000a760: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-0000a770: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-0000a780: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-0000a790: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-0000a7a0: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-0000a7b0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-0000a7c0: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-0000a7d0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-0000a7e0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-0000a7f0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-0000a800: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-0000a810: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-0000a820: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-0000a830: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-0000a840: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-0000a850: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-0000a860: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-0000a870: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-0000a880: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-0000a890: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-0000a8a0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
-0000a8b0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
-0000a8c0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
-0000a8d0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
-0000a8e0: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
-0000a8f0: 7061 6972 7360 2c20 3a6d 6574 683a 6070  pairs`, :meth:`p
-0000a900: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000a910: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000a920: 7261 6e6b 6564 5f70 6169 7273 5f77 6974  ranked_pairs_wit
-0000a930: 685f 7465 7374 600a 0a20 2020 202e 2e20  h_test`..    .. 
-0000a940: 6578 6563 5f63 6f64 653a 3a0a 0a20 2020  exec_code::..   
-0000a950: 2020 2020 2066 726f 6d20 7072 6566 5f76       from pref_v
-0000a960: 6f74 696e 672e 7072 6f66 696c 6573 2069  oting.profiles i
-0000a970: 6d70 6f72 7420 5072 6f66 696c 650a 2020  mport Profile.  
-0000a980: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
-0000a990: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
-0000a9a0: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
-0000a9b0: 7274 2072 616e 6b65 645f 7061 6972 735f  rt ranked_pairs_
-0000a9c0: 7462 2c20 7261 6e6b 6564 5f70 6169 7273  tb, ranked_pairs
-0000a9d0: 5f7a 740a 0a20 2020 2020 2020 2070 726f  _zt..        pro
-0000a9e0: 6620 3d20 5072 6f66 696c 6528 5b5b 322c  f = Profile([[2,
-0000a9f0: 2033 2c20 312c 2030 5d2c 205b 302c 2033   3, 1, 0], [0, 3
-0000aa00: 2c20 312c 2032 5d2c 205b 312c 2033 2c20  , 1, 2], [1, 3, 
-0000aa10: 322c 2030 5d2c 205b 322c 2031 2c20 332c  2, 0], [2, 1, 3,
-0000aa20: 2030 5d5d 2c20 5b31 2c20 312c 2031 2c20   0]], [1, 1, 1, 
-0000aa30: 315d 290a 0a20 2020 2020 2020 2070 726f  1])..        pro
-0000aa40: 662e 6469 7370 6c61 7928 290a 0a20 2020  f.display()..   
-0000aa50: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
-0000aa60: 735f 7462 2e64 6973 706c 6179 2870 726f  s_tb.display(pro
-0000aa70: 6629 0a20 2020 2020 2020 2072 616e 6b65  f).        ranke
-0000aa80: 645f 7061 6972 735f 7462 2e64 6973 706c  d_pairs_tb.displ
-0000aa90: 6179 2870 726f 662c 2074 6965 5f62 7265  ay(prof, tie_bre
-0000aaa0: 616b 6572 203d 205b 332c 2032 2c20 312c  aker = [3, 2, 1,
-0000aab0: 2030 5d29 0a20 2020 2020 2020 2072 616e   0]).        ran
-0000aac0: 6b65 645f 7061 6972 735f 7a74 2e64 6973  ked_pairs_zt.dis
-0000aad0: 706c 6179 2870 726f 6629 0a0a 2020 2020  play(prof)..    
-0000aae0: 2222 220a 0a20 2020 2063 616e 6469 6461  """..    candida
-0000aaf0: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
-0000ab00: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
-0000ab10: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
-0000ab20: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
-0000ab30: 0a20 2020 2063 6964 785f 746f 5f63 616e  .    cidx_to_can
-0000ab40: 6420 3d20 7b63 6964 783a 2063 2066 6f72  d = {cidx: c for
-0000ab50: 2063 6964 782c 2063 2069 6e20 656e 756d   cidx, c in enum
-0000ab60: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
-0000ab70: 297d 2020 0a20 2020 2063 616e 645f 746f  )}  .    cand_to
-0000ab80: 5f63 6964 7820 3d20 7b63 3a20 6369 6478  _cidx = {c: cidx
-0000ab90: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
-0000aba0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
-0000abb0: 6174 6573 297d 2020 0a0a 2020 2020 7374  ates)}  ..    st
-0000abc0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000abd0: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
-0000abe0: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
-0000abf0: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
-0000ac00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000ac10: 6f6e 0a20 2020 200a 2020 2020 7462 5f72  on.    .    tb_r
-0000ac20: 616e 6b69 6e67 203d 2074 6965 5f62 7265  anking = tie_bre
-0000ac30: 616b 6572 2069 6620 7469 655f 6272 6561  aker if tie_brea
-0000ac40: 6b65 7220 6973 206e 6f74 204e 6f6e 6520  ker is not None 
-0000ac50: 656c 7365 2073 6f72 7465 6428 6c69 7374  else sorted(list
-0000ac60: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
-0000ac70: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
-0000ac80: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
-0000ac90: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
-0000aca0: 616e 6473 290a 2020 2020 2320 5261 6e6b  ands).    # Rank
-0000acb0: 6564 2050 6169 7273 2069 7320 436f 6e64  ed Pairs is Cond
-0000acc0: 6f72 6365 7420 636f 6e73 6973 7465 6e74  orcet consistent
-0000acd0: 2c20 736f 2073 696d 706c 7920 7265 7475  , so simply retu
-0000ace0: 726e 2074 6865 2043 6f6e 646f 7263 6574  rn the Condorcet
-0000acf0: 2077 696e 6e65 7220 6966 2065 7869 7374   winner if exist
-0000ad00: 730a 2020 2020 6966 2063 7720 6973 206e  s.    if cw is n
-0000ad10: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
-0000ad20: 2020 7769 6e6e 6572 7320 3d20 5b63 775d    winners = [cw]
-0000ad30: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-0000ad40: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
-0000ad50: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
-0000ad60: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
-0000ad70: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
-0000ad80: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
-0000ad90: 2063 616e 6469 6461 7465 7320 0a20 2020   candidates .   
-0000ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000adb0: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
-0000adc0: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
-0000add0: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
-0000ade0: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
-0000adf0: 2863 312c 2063 3229 295d 0a20 2020 2020  (c1, c2))].     
-0000ae00: 2020 2077 696e 6e65 7273 203d 206c 6973     winners = lis
-0000ae10: 7428 2920 2020 2020 2020 2020 2020 200a  t()            .
-0000ae20: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000ae30: 7320 3d20 736f 7274 6564 286c 6973 7428  s = sorted(list(
-0000ae40: 7365 7428 5b65 5b32 5d20 666f 7220 6520  set([e[2] for e 
-0000ae50: 696e 2077 5f65 6467 6573 5d29 292c 2072  in w_edges])), r
-0000ae60: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
-0000ae70: 2020 2020 200a 2020 2020 2020 2020 7270       .        rp
-0000ae80: 5f64 6566 6561 7420 3d20 5350 4f28 6c65  _defeat = SPO(le
-0000ae90: 6e28 6361 6e64 6964 6174 6573 2929 0a0a  n(candidates))..
-0000aea0: 2020 2020 2020 2020 666f 7220 7320 696e          for s in
-0000aeb0: 2073 7472 656e 6774 6873 3a20 0a20 2020   strengths: .   
-0000aec0: 2020 2020 2020 2020 2065 6467 6573 203d           edges =
-0000aed0: 205b 6520 666f 7220 6520 696e 2077 5f65   [e for e in w_e
-0000aee0: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
-0000aef0: 735d 0a20 2020 2020 2020 2020 2020 200a  s].            .
-0000af00: 2020 2020 2020 2020 2020 2020 2320 6272              # br
-0000af10: 6561 6b20 7469 6573 2075 7369 6e67 2074  eak ties using t
-0000af20: 6865 206c 6578 6963 6f67 7261 7068 6963  he lexicographic
-0000af30: 206f 7264 6572 696e 6720 6f6e 2074 7570   ordering on tup
-0000af40: 6c65 7320 6769 7665 6e20 7462 5f72 616e  les given tb_ran
-0000af50: 6b69 6e67 0a20 2020 2020 2020 2020 2020  king.           
-0000af60: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
-0000af70: 736f 7274 6564 2865 6467 6573 2c20 6b65  sorted(edges, ke
-0000af80: 7920 3d20 6c61 6d62 6461 2065 3a20 2874  y = lambda e: (t
-0000af90: 625f 7261 6e6b 696e 672e 696e 6465 7828  b_ranking.index(
-0000afa0: 655b 305d 292c 2074 625f 7261 6e6b 696e  e[0]), tb_rankin
-0000afb0: 672e 696e 6465 7828 655b 315d 2929 2c20  g.index(e[1])), 
-0000afc0: 7265 7665 7273 653d 4661 6c73 6529 0a20  reverse=False). 
-0000afd0: 2020 2020 2020 2020 2020 2066 6f72 2065             for e
-0000afe0: 302c 6531 2c73 2069 6e20 6564 6765 733a  0,e1,s in edges:
-0000aff0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000b000: 2020 6966 206e 6f74 2072 705f 6465 6665    if not rp_defe
-0000b010: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
-0000b020: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
-0000b030: 6964 785b 6530 5d5d 3a0a 2020 2020 2020  idx[e0]]:.      
-0000b040: 2020 2020 2020 2020 2020 2020 2020 7270                rp
-0000b050: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
-0000b060: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
-0000b070: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
-0000b080: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
-0000b090: 7273 2e61 7070 656e 6428 6369 6478 5f74  rs.append(cidx_t
-0000b0a0: 6f5f 6361 6e64 5b72 705f 6465 6665 6174  o_cand[rp_defeat
-0000b0b0: 2e69 6e69 7469 616c 5f65 6c65 6d65 6e74  .initial_element
-0000b0c0: 7328 295b 305d 5d29 0a0a 2020 2020 7265  s()[0]])..    re
-0000b0d0: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
-0000b0e0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
-0000b0f0: 0a72 705f 7a74 5f70 726f 7065 7274 6965  .rp_zt_propertie
-0000b100: 7320 3d20 566f 7469 6e67 4d65 7468 6f64  s = VotingMethod
-0000b110: 5072 6f70 6572 7469 6573 280a 2020 2020  Properties(.    
-0000b120: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-0000b130: 3d54 7275 652c 200a 2020 2020 636f 6e64  =True, .    cond
-0000b140: 6f72 6365 745f 6c6f 7365 723d 5472 7565  orcet_loser=True
-0000b150: 2c0a 2020 2020 7061 7265 746f 5f64 6f6d  ,.    pareto_dom
-0000b160: 696e 616e 6365 3d54 7275 652c 200a 2020  inance=True, .  
-0000b170: 2020 706f 7369 7469 7665 5f69 6e76 6f6c    positive_invol
-0000b180: 7665 6d65 6e74 3d46 616c 7365 2c0a 2020  vement=False,.  
-0000b190: 2020 290a 4076 6d28 6e61 6d65 3d22 5261    ).@vm(name="Ra
-0000b1a0: 6e6b 6564 2050 6169 7273 205a 5422 2c0a  nked Pairs ZT",.
-0000b1b0: 2020 2020 7072 6f70 6572 7469 6573 3d72      properties=r
-0000b1c0: 705f 7a74 5f70 726f 7065 7274 6965 732c  p_zt_properties,
-0000b1d0: 0a20 2020 2069 6e70 7574 5f74 7970 6573  .    input_types
-0000b1e0: 3d5b 456c 6563 7469 6f6e 5479 7065 732e  =[ElectionTypes.
-0000b1f0: 5052 4f46 494c 455d 290a 6465 6620 7261  PROFILE]).def ra
-0000b200: 6e6b 6564 5f70 6169 7273 5f7a 7428 0a20  nked_pairs_zt(. 
-0000b210: 2020 2070 726f 6669 6c65 2c20 0a20 2020     profile, .   
-0000b220: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
-0000b230: 6e65 2c20 0a20 2020 2073 7472 656e 6774  ne, .    strengt
-0000b240: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-0000b250: 6529 3a20 2020 0a20 2020 2022 2222 5261  e):   .    """Ra
-0000b260: 6e6b 6564 2070 6169 7273 2077 6865 7265  nked pairs where
-0000b270: 2061 2066 6978 6564 2076 6f74 6572 2062   a fixed voter b
-0000b280: 7265 616b 7320 616e 7920 7469 6573 2069  reaks any ties i
-0000b290: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
-0000b2a0: 4974 2069 7320 616c 7761 7973 2074 6865  It is always the
-0000b2b0: 2076 6f74 6572 2069 6e20 706f 7369 7469   voter in positi
-0000b2c0: 6f6e 2030 2074 6861 7420 6272 6561 6b73  on 0 that breaks
-0000b2d0: 2074 6865 2074 6965 732e 2020 5369 6e63   the ties.  Sinc
-0000b2e0: 6520 766f 7465 7273 2068 6176 6520 7374  e voters have st
-0000b2f0: 7269 6374 2070 7265 6665 7265 6e63 6573  rict preferences
-0000b300: 2c20 7468 6973 206d 6574 686f 6420 6973  , this method is
-0000b310: 2072 6573 6f6c 7574 652e 2020 5468 6973   resolute.  This
-0000b320: 2069 7320 6b6e 6f77 6e20 6173 2052 616e   is known as Ran
-0000b330: 6b65 6420 5061 6972 7320 5a54 2c20 666f  ked Pairs ZT, fo
-0000b340: 7220 5a61 7669 7374 2054 6964 656d 616e  r Zavist Tideman
-0000b350: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
-0000b360: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-0000b370: 696c 6529 3a20 4120 7072 6f66 696c 6520  ile): A profile 
-0000b380: 6f66 206c 696e 6561 7220 6f72 6465 7273  of linear orders
-0000b390: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-0000b3a0: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-0000b3b0: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-0000b3c0: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-0000b3d0: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-0000b3e0: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-0000b3f0: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-0000b400: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-0000b410: 6361 6e64 7360 600a 0a20 2020 2052 6574  cands``..    Ret
-0000b420: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000b430: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000b440: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000b450: 2020 2e2e 2073 6565 616c 736f 3a3a 0a0a    .. seealso::..
-0000b460: 2020 2020 2020 2020 3a6d 6574 683a 6070          :meth:`p
-0000b470: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000b480: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000b490: 7261 6e6b 6564 5f70 6169 7273 602c 203a  ranked_pairs`, :
-0000b4a0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
-0000b4b0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
-0000b4c0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
-0000b4d0: 6972 735f 7769 7468 5f74 6573 7460 0a0a  irs_with_test`..
-0000b4e0: 2020 2020 2e2e 2065 7865 635f 636f 6465      .. exec_code
-0000b4f0: 3a3a 0a0a 2020 2020 2020 2020 6672 6f6d  ::..        from
-0000b500: 2070 7265 665f 766f 7469 6e67 2e70 726f   pref_voting.pro
-0000b510: 6669 6c65 7320 696d 706f 7274 2050 726f  files import Pro
-0000b520: 6669 6c65 0a20 2020 2020 2020 2066 726f  file.        fro
-0000b530: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-0000b540: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000b550: 6473 2069 6d70 6f72 7420 7261 6e6b 6564  ds import ranked
-0000b560: 5f70 6169 7273 5f74 622c 2072 616e 6b65  _pairs_tb, ranke
-0000b570: 645f 7061 6972 735f 7a74 0a0a 2020 2020  d_pairs_zt..    
-0000b580: 2020 2020 7072 6f66 203d 2050 726f 6669      prof = Profi
-0000b590: 6c65 285b 5b32 2c20 332c 2031 2c20 305d  le([[2, 3, 1, 0]
-0000b5a0: 2c20 5b30 2c20 332c 2031 2c20 325d 2c20  , [0, 3, 1, 2], 
-0000b5b0: 5b31 2c20 332c 2032 2c20 305d 2c20 5b32  [1, 3, 2, 0], [2
-0000b5c0: 2c20 312c 2033 2c20 305d 5d2c 205b 312c  , 1, 3, 0]], [1,
-0000b5d0: 2031 2c20 312c 2031 5d29 0a0a 2020 2020   1, 1, 1])..    
-0000b5e0: 2020 2020 7072 6f66 2e64 6973 706c 6179      prof.display
-0000b5f0: 2829 0a0a 2020 2020 2020 2020 7261 6e6b  ()..        rank
-0000b600: 6564 5f70 6169 7273 5f74 622e 6469 7370  ed_pairs_tb.disp
-0000b610: 6c61 7928 7072 6f66 290a 2020 2020 2020  lay(prof).      
-0000b620: 2020 7261 6e6b 6564 5f70 6169 7273 5f74    ranked_pairs_t
-0000b630: 622e 6469 7370 6c61 7928 7072 6f66 2c20  b.display(prof, 
-0000b640: 7469 655f 6272 6561 6b65 7220 3d20 5b33  tie_breaker = [3
-0000b650: 2c20 322c 2031 2c20 305d 290a 2020 2020  , 2, 1, 0]).    
-0000b660: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
-0000b670: 5f7a 742e 6469 7370 6c61 7928 7072 6f66  _zt.display(prof
-0000b680: 290a 0a20 2020 200a 2020 2020 2222 220a  )..    .    """.
-0000b690: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-0000b6a0: 2070 726f 6669 6c65 2e63 616e 6469 6461   profile.candida
-0000b6b0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-0000b6c0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-0000b6d0: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
-0000b6e0: 2020 0a20 2020 2023 2074 6865 2074 6965    .    # the tie
-0000b6f0: 2d62 7265 616b 6572 2069 7320 616c 7761  -breaker is alwa
-0000b700: 7973 2074 6865 2066 6972 7374 2076 6f74  ys the first vot
-0000b710: 6572 2e20 0a20 2020 2074 625f 7261 6e6b  er. .    tb_rank
-0000b720: 696e 6720 3d20 7475 706c 6528 5b63 2066  ing = tuple([c f
-0000b730: 6f72 2063 2069 6e20 6c69 7374 2870 726f  or c in list(pro
-0000b740: 6669 6c65 2e5f 7261 6e6b 696e 6773 5b30  file._rankings[0
-0000b750: 5d29 2069 6620 6320 696e 2063 616e 6469  ]) if c in candi
-0000b760: 6461 7465 735d 290a 2020 2020 0a20 2020  dates]).    .   
-0000b770: 2072 6574 7572 6e20 7261 6e6b 6564 5f70   return ranked_p
-0000b780: 6169 7273 5f74 6228 7072 6f66 696c 652c  airs_tb(profile,
-0000b790: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-0000b7a0: 7272 5f63 616e 6473 2c20 7469 655f 6272  rr_cands, tie_br
-0000b7b0: 6561 6b65 7220 3d20 7462 5f72 616e 6b69  eaker = tb_ranki
-0000b7c0: 6e67 2c20 7374 7265 6e67 7468 5f66 756e  ng, strength_fun
-0000b7d0: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
-0000b7e0: 5f66 756e 6374 696f 6e29 0a0a 7269 7665  _function)..rive
-0000b7f0: 725f 7072 6f70 6572 7469 6573 203d 2056  r_properties = V
-0000b800: 6f74 696e 674d 6574 686f 6450 726f 7065  otingMethodPrope
-0000b810: 7274 6965 7328 0a20 2020 2063 6f6e 646f  rties(.    condo
-0000b820: 7263 6574 5f77 696e 6e65 723d 5472 7565  rcet_winner=True
-0000b830: 2c20 0a20 2020 2063 6f6e 646f 7263 6574  , .    condorcet
-0000b840: 5f6c 6f73 6572 3d54 7275 652c 0a20 2020  _loser=True,.   
-0000b850: 2070 6172 6574 6f5f 646f 6d69 6e61 6e63   pareto_dominanc
-0000b860: 653d 5472 7565 2c0a 2020 2020 706f 7369  e=True,.    posi
-0000b870: 7469 7665 5f69 6e76 6f6c 7665 6d65 6e74  tive_involvement
-0000b880: 3d46 616c 7365 2c20 0a20 2020 2029 0a40  =False, .    ).@
-0000b890: 766d 286e 616d 653d 2252 6976 6572 222c  vm(name="River",
-0000b8a0: 0a20 2020 2070 726f 7065 7274 6965 733d  .    properties=
-0000b8b0: 7269 7665 725f 7072 6f70 6572 7469 6573  river_properties
-0000b8c0: 2c0a 2020 2020 696e 7075 745f 7479 7065  ,.    input_type
-0000b8d0: 733d 5b45 6c65 6374 696f 6e54 7970 6573  s=[ElectionTypes
-0000b8e0: 2e50 524f 4649 4c45 2c20 456c 6563 7469  .PROFILE, Electi
-0000b8f0: 6f6e 5479 7065 732e 5052 4f46 494c 455f  onTypes.PROFILE_
-0000b900: 5749 5448 5f54 4945 532c 2045 6c65 6374  WITH_TIES, Elect
-0000b910: 696f 6e54 7970 6573 2e4d 4152 4749 4e5f  ionTypes.MARGIN_
-0000b920: 4752 4150 485d 290a 6465 6620 7269 7665  GRAPH]).def rive
-0000b930: 7228 6564 6174 612c 2063 7572 725f 6361  r(edata, curr_ca
-0000b940: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
-0000b950: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
-0000b960: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
-0000b970: 220a 2020 2020 4f72 6465 7220 7468 6520  ".    Order the 
-0000b980: 6564 6765 7320 696e 2074 6865 2077 6561  edges in the wea
-0000b990: 6b20 6d61 7267 696e 2067 7261 7068 2066  k margin graph f
-0000b9a0: 726f 6d20 6c61 7267 6573 7420 746f 2073  rom largest to s
-0000b9b0: 6d61 6c6c 6573 7420 616e 6420 6c6f 636b  mallest and lock
-0000b9c0: 2074 6865 6d20 696e 2069 6e20 7468 6174   them in in that
-0000b9d0: 206f 7264 6572 2c20 736b 6970 7069 6e67   order, skipping
-0000b9e0: 2065 6467 6573 2074 6861 7420 6372 6561   edges that crea
-0000b9f0: 7465 2061 2063 7963 6c65 202a 616e 6420  te a cycle *and 
-0000ba00: 6564 6765 7320 696e 2077 6869 6368 2074  edges in which t
-0000ba10: 6865 7265 2069 7320 616c 7265 6164 7920  here is already 
-0000ba20: 616e 2065 6467 6520 706f 696e 7469 6e67  an edge pointing
-0000ba30: 2074 6f20 7468 6520 7461 7267 6574 2a2e   to the target*.
-0000ba40: 2020 4272 6561 6b20 7469 6573 2075 7369    Break ties usi
-0000ba50: 6e67 2061 2074 6965 2d62 7265 616b 696e  ng a tie-breakin
-0000ba60: 6720 206c 696e 6561 7220 6f72 6465 7269  g  linear orderi
-0000ba70: 6e67 206f 7665 7220 7468 6520 6564 6765  ng over the edge
-0000ba80: 732e 2020 4120 6361 6e64 6964 6174 6520  s.  A candidate 
-0000ba90: 6973 2061 2052 6976 6572 2077 696e 6e65  is a River winne
-0000baa0: 7220 6966 2069 7420 7769 6e73 2061 6363  r if it wins acc
-0000bab0: 6f72 6469 6e67 2074 6f20 736f 6d65 2074  ording to some t
-0000bac0: 6965 2d62 7265 616b 696e 6720 7275 6c65  ie-breaking rule
-0000bad0: 2e20 5365 6520 6874 7470 733a 2f2f 656c  . See https://el
-0000bae0: 6563 746f 7769 6b69 2e6f 7267 2f77 696b  ectowiki.org/wik
-0000baf0: 692f 5269 7665 722e 0a0a 2020 2020 4172  i/River...    Ar
-0000bb00: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
-0000bb10: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
-0000bb20: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
-0000bb30: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
-0000bb40: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
-0000bb50: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
-0000bb60: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
-0000bb70: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
-0000bb80: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
-0000bb90: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
-0000bba0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
-0000bbb0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
-0000bbc0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
-0000bbd0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
-0000bbe0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
-0000bbf0: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
-0000bc00: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
-0000bc10: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
-0000bc20: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
-0000bc30: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
-0000bc40: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
-0000bc50: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
-0000bc60: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
-0000bc70: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
-0000bc80: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
-0000bc90: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
-0000bca0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
-0000bcb0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
-0000bcc0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
-0000bcd0: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
-0000bce0: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
-0000bcf0: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
-0000bd00: 6469 6461 7465 732e 200a 0a20 2020 203a  didates. ..    :
-0000bd10: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
-0000bd20: 2e20 6578 6563 5f63 6f64 653a 3a20 0a0a  . exec_code:: ..
-0000bd30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-0000bd40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-0000bd50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-0000bd60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-0000bd70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-0000bd80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-0000bd90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-0000bda0: 6473 2069 6d70 6f72 7420 7269 7665 722c  ds import river,
-0000bdb0: 2072 616e 6b65 645f 7061 6972 730a 2020   ranked_pairs.  
-0000bdc0: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
-0000bdd0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
-0000bde0: 5b30 2c20 312c 2032 2c20 335d 2c20 5b28  [0, 1, 2, 3], [(
-0000bdf0: 302c 2032 2c20 3229 2c20 2830 2c20 332c  0, 2, 2), (0, 3,
-0000be00: 2038 292c 2028 312c 2030 2c20 3132 292c   8), (1, 0, 12),
-0000be10: 2028 322c 2033 2c20 3132 292c 2028 332c   (2, 3, 12), (3,
-0000be20: 2031 2c20 3629 5d29 0a0a 2020 2020 2020   1, 6)])..      
-0000be30: 2020 7261 6e6b 6564 5f70 6169 7273 2e64    ranked_pairs.d
-0000be40: 6973 706c 6179 286d 6729 0a20 2020 2020  isplay(mg).     
-0000be50: 2020 2072 6976 6572 2e64 6973 706c 6179     river.display
-0000be60: 286d 6729 0a0a 2020 2020 2222 220a 2020  (mg)..    """.  
-0000be70: 2020 6361 6e64 6964 6174 6573 203d 2065    candidates = e
-0000be80: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
-0000be90: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
-0000bea0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
-0000beb0: 6361 6e64 7320 2020 200a 2020 2020 6369  cands    .    ci
-0000bec0: 6478 5f74 6f5f 6361 6e64 203d 207b 6369  dx_to_cand = {ci
-0000bed0: 6478 3a20 6320 666f 7220 6369 6478 2c20  dx: c for cidx, 
-0000bee0: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
-0000bef0: 616e 6469 6461 7465 7329 7d20 200a 2020  andidates)}  .  
-0000bf00: 2020 6361 6e64 5f74 6f5f 6369 6478 203d    cand_to_cidx =
-0000bf10: 207b 633a 2063 6964 7820 666f 7220 6369   {c: cidx for ci
-0000bf20: 6478 2c20 6320 696e 2065 6e75 6d65 7261  dx, c in enumera
-0000bf30: 7465 2863 616e 6469 6461 7465 7329 7d20  te(candidates)} 
-0000bf40: 200a 0a20 2020 2073 7472 656e 6774 685f   ..    strength_
-0000bf50: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
-0000bf60: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
-0000bf70: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
-0000bf80: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
-0000bf90: 7468 5f66 756e 6374 696f 6e20 2020 200a  th_function    .
-0000bfa0: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
-0000bfb0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-0000bfc0: 2863 7572 725f 6361 6e64 733d 6375 7272  (curr_cands=curr
-0000bfd0: 5f63 616e 6473 290a 2020 2020 2320 5261  _cands).    # Ra
-0000bfe0: 6e6b 6564 2050 6169 7273 2069 7320 436f  nked Pairs is Co
-0000bff0: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
-0000c000: 6e74 2c20 736f 2073 696d 706c 7920 7265  nt, so simply re
-0000c010: 7475 726e 2074 6865 2043 6f6e 646f 7263  turn the Condorc
-0000c020: 6574 2077 696e 6e65 7220 6966 2065 7869  et winner if exi
-0000c030: 7374 730a 2020 2020 6966 2063 7720 6973  sts.    if cw is
-0000c040: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
-0000c050: 2020 2020 7769 6e6e 6572 7320 3d20 5b63      winners = [c
-0000c060: 775d 0a20 2020 2065 6c73 653a 0a20 2020  w].    else:.   
-0000c070: 2020 2020 2077 5f65 6467 6573 203d 205b       w_edges = [
-0000c080: 2863 312c 2063 322c 2073 7472 656e 6774  (c1, c2, strengt
-0000c090: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
-0000c0a0: 3229 2920 666f 7220 6331 2069 6e20 6361  2)) for c1 in ca
-0000c0b0: 6e64 6964 6174 6573 2066 6f72 2063 3220  ndidates for c2 
-0000c0c0: 696e 2063 616e 6469 6461 7465 7320 0a20  in candidates . 
-0000c0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0e0: 2020 6966 2063 3120 213d 2063 3220 616e    if c1 != c2 an
-0000c0f0: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
-0000c100: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
-0000c110: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
-0000c120: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
-0000c130: 2020 2020 2077 696e 6e65 7273 203d 206c       winners = l
-0000c140: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
-0000c150: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
-0000c160: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
-0000c170: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
-0000c180: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
-0000c190: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
-0000c1a0: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
-0000c1b0: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
-0000c1c0: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
-0000c1d0: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
-0000c1e0: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
-0000c1f0: 2020 2020 2074 6273 203d 2070 726f 6475       tbs = produ
-0000c200: 6374 282a 5b70 6572 6d75 7461 7469 6f6e  ct(*[permutation
-0000c210: 7328 6564 6765 7329 2066 6f72 2065 6467  s(edges) for edg
-0000c220: 6573 2069 6e20 736f 7274 6564 5f65 6467  es in sorted_edg
-0000c230: 6573 5d29 0a20 2020 2020 2020 2066 6f72  es]).        for
-0000c240: 2074 6220 696e 2074 6273 3a0a 2020 2020   tb in tbs:.    
-0000c250: 2020 2020 2020 2020 6564 6765 7320 3d20          edges = 
-0000c260: 666c 6174 7465 6e28 7462 290a 2020 2020  flatten(tb).    
-0000c270: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
-0000c280: 7420 3d20 5350 4f28 6c65 6e28 6361 6e64  t = SPO(len(cand
-0000c290: 6964 6174 6573 2929 0a20 2020 2020 2020  idates)).       
-0000c2a0: 2020 2020 2066 6f72 2065 302c 6531 2c73       for e0,e1,s
-0000c2b0: 2069 6e20 6564 6765 733a 200a 2020 2020   in edges: .    
-0000c2c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000c2d0: 6f74 2072 765f 6465 6665 6174 2e50 5b63  ot rv_defeat.P[c
-0000c2e0: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
-0000c2f0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
-0000c300: 5d5d 2061 6e64 206c 656e 2872 765f 6465  ]] and len(rv_de
-0000c310: 6665 6174 2e70 7265 6473 5b63 616e 645f  feat.preds[cand_
-0000c320: 746f 5f63 6964 785b 6531 5d5d 2920 3d3d  to_cidx[e1]]) ==
-0000c330: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0000c340: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
-0000c350: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
-0000c360: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
-0000c370: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
-0000c380: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-0000c390: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
-0000c3a0: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
-0000c3b0: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
-0000c3c0: 5d29 0a0a 2020 2020 7265 7475 726e 2073  ])..    return s
-0000c3d0: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
-0000c3e0: 696e 6e65 7273 2929 290a 0a64 6566 2072  inners)))..def r
-0000c3f0: 6976 6572 5f64 6566 6561 7473 2865 6461  iver_defeats(eda
-0000c400: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000c410: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
-0000c420: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
-0000c430: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-0000c440: 7475 726e 7320 7468 6520 5269 7665 7220  turns the River 
-0000c450: 6465 6665 6174 2072 656c 6174 696f 6e73  defeat relations
-0000c460: 2070 726f 6475 6365 6420 6279 2074 6865   produced by the
-0000c470: 2052 6976 6572 2061 6c67 6f72 6974 686d   River algorithm
-0000c480: 2e0a 0a20 2020 202e 2e20 696d 706f 7274  ...    .. import
-0000c490: 616e 743a 3a0a 2020 2020 2020 2020 556e  ant::.        Un
-0000c4a0: 6c69 6b65 2074 6865 206f 7468 6572 2066  like the other f
-0000c4b0: 756e 6374 696f 6e73 2074 6861 7420 7265  unctions that re
-0000c4c0: 7475 726e 2061 2073 696e 676c 6520 6465  turn a single de
-0000c4d0: 6665 6174 2072 656c 6174 696f 6e2c 2074  feat relation, t
-0000c4e0: 6869 7320 7265 7475 726e 7320 6120 6c69  his returns a li
-0000c4f0: 7374 206f 6620 6465 6665 6174 2072 656c  st of defeat rel
-0000c500: 6174 696f 6e73 2e20 0a20 2020 2020 2020  ations. .       
-0000c510: 200a 2020 2020 4172 6773 3a0a 2020 2020   .    Args:.    
-0000c520: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
-0000c530: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
-0000c540: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
-0000c550: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
-0000c560: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
-0000c570: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
-0000c580: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-0000c590: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
-0000c5a0: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
-0000c5b0: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
-0000c5c0: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
-0000c5d0: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
-0000c5e0: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
-0000c5f0: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
-0000c600: 5f63 616e 6473 6060 0a20 2020 2020 2020  _cands``.       
-0000c610: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000c620: 6f6e 2028 6675 6e63 7469 6f6e 2c20 6f70  on (function, op
-0000c630: 7469 6f6e 616c 293a 2054 6865 2073 7472  tional): The str
-0000c640: 656e 6774 6820 6675 6e63 7469 6f6e 2074  ength function t
-0000c650: 6f20 6265 2075 7365 6420 746f 2063 616c  o be used to cal
-0000c660: 6375 6c61 7465 2074 6865 2073 7472 656e  culate the stren
-0000c670: 6774 6820 6f66 2061 2070 6174 682e 2020  gth of a path.  
-0000c680: 2054 6865 2064 6566 6175 6c74 2069 7320   The default is 
-0000c690: 7468 6520 6d61 7267 696e 206d 6574 686f  the margin metho
-0000c6a0: 6420 6f66 2060 6065 6461 7461 6060 2e20  d of ``edata``. 
-0000c6b0: 2020 5468 6973 206f 6e6c 7920 6d61 7474    This only matt
-0000c6c0: 6572 7320 7768 656e 2074 6865 2062 616c  ers when the bal
-0000c6d0: 6c6f 7473 2061 7265 206e 6f74 206c 696e  lots are not lin
-0000c6e0: 6561 7220 6f72 6465 7273 2e20 0a0a 2020  ear orders. ..  
-0000c6f0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
-0000c700: 2020 2020 4120 6e65 7477 6f72 6b78 2044      A networkx D
-0000c710: 6947 7261 7068 2072 6570 7265 7365 6e74  iGraph represent
-0000c720: 696e 6720 7468 6520 5269 7665 7220 6465  ing the River de
-0000c730: 6665 6174 2072 656c 6174 696f 6e2e 200a  feat relation. .
-0000c740: 2020 2020 2222 220a 0a20 2020 2063 616e      """..    can
-0000c750: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
-0000c760: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
-0000c770: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
-0000c780: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
-0000c790: 2020 2020 0a20 2020 2073 7472 656e 6774      .    strengt
-0000c7a0: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-0000c7b0: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-0000c7c0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-0000c7d0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-0000c7e0: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
-0000c7f0: 200a 0a20 2020 2077 5f65 6467 6573 203d   ..    w_edges =
-0000c800: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
-0000c810: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
-0000c820: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
-0000c830: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
-0000c840: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
-0000c850: 6966 2063 3120 213d 2063 3220 616e 6420  if c1 != c2 and 
-0000c860: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
-0000c870: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
-0000c880: 6f72 2065 6461 7461 2e69 735f 7469 6564  or edata.is_tied
-0000c890: 2863 312c 2063 3229 295d 0a0a 2020 2020  (c1, c2))]..    
-0000c8a0: 7374 7265 6e67 7468 7320 3d20 736f 7274  strengths = sort
-0000c8b0: 6564 286c 6973 7428 7365 7428 5b65 5b32  ed(list(set([e[2
-0000c8c0: 5d20 666f 7220 6520 696e 2077 5f65 6467  ] for e in w_edg
-0000c8d0: 6573 5d29 292c 2072 6576 6572 7365 3d54  es])), reverse=T
-0000c8e0: 7275 6529 0a20 2020 2073 6f72 7465 645f  rue).    sorted_
-0000c8f0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
-0000c900: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
-0000c910: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
-0000c920: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
-0000c930: 2020 2074 6273 203d 2070 726f 6475 6374     tbs = product
-0000c940: 282a 5b70 6572 6d75 7461 7469 6f6e 7328  (*[permutations(
-0000c950: 6564 6765 7329 2066 6f72 2065 6467 6573  edges) for edges
-0000c960: 2069 6e20 736f 7274 6564 5f65 6467 6573   in sorted_edges
-0000c970: 5d29 0a0a 2020 2020 7269 7665 725f 6465  ])..    river_de
-0000c980: 6665 6174 7320 3d20 6c69 7374 2829 0a20  feats = list(). 
-0000c990: 2020 2066 6f72 2074 6220 696e 2074 6273     for tb in tbs
-0000c9a0: 3a0a 2020 2020 2020 2020 6564 6765 7320  :.        edges 
-0000c9b0: 3d20 666c 6174 7465 6e28 7462 290a 2020  = flatten(tb).  
-0000c9c0: 2020 2020 2020 7269 7665 725f 6465 6665        river_defe
-0000c9d0: 6174 203d 206e 782e 4469 4772 6170 6828  at = nx.DiGraph(
-0000c9e0: 2920 0a20 2020 2020 2020 2066 6f72 2065  ) .        for e
-0000c9f0: 2069 6e20 6564 6765 733a 200a 2020 2020   in edges: .    
-0000ca00: 2020 2020 2020 2020 6966 2065 5b31 5d20          if e[1] 
-0000ca10: 6e6f 7420 696e 2072 6976 6572 5f64 6566  not in river_def
-0000ca20: 6561 742e 6e6f 6465 7320 6f72 206c 656e  eat.nodes or len
-0000ca30: 286c 6973 7428 7269 7665 725f 6465 6665  (list(river_defe
-0000ca40: 6174 2e69 6e5f 6564 6765 7328 655b 315d  at.in_edges(e[1]
-0000ca50: 2929 2920 3d3d 2030 3a0a 2020 2020 2020  ))) == 0:.      
-0000ca60: 2020 2020 2020 2020 2020 7269 7665 725f            river_
-0000ca70: 6465 6665 6174 2e61 6464 5f65 6467 6528  defeat.add_edge(
-0000ca80: 655b 305d 2c20 655b 315d 2c20 7765 6967  e[0], e[1], weig
-0000ca90: 6874 3d65 5b32 5d29 0a20 2020 2020 2020  ht=e[2]).       
-0000caa0: 2020 2020 2020 2020 2069 6620 646f 6573           if does
-0000cab0: 5f63 7265 6174 655f 6379 636c 6528 7269  _create_cycle(ri
-0000cac0: 7665 725f 6465 6665 6174 2c20 6529 3a0a  ver_defeat, e):.
-0000cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cae0: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
-0000caf0: 2e72 656d 6f76 655f 6564 6765 2865 5b30  .remove_edge(e[0
-0000cb00: 5d2c 2065 5b31 5d29 0a20 2020 2020 2020  ], e[1]).       
-0000cb10: 2020 2020 200a 2020 2020 2020 2020 7269       .        ri
-0000cb20: 7665 725f 6465 6665 6174 732e 6170 7065  ver_defeats.appe
-0000cb30: 6e64 2872 6976 6572 5f64 6566 6561 7429  nd(river_defeat)
-0000cb40: 0a0a 2020 2020 7265 7475 726e 2072 6976  ..    return riv
-0000cb50: 6572 5f64 6566 6561 7473 0a0a 4076 6d28  er_defeats..@vm(
-0000cb60: 6e61 6d65 3d22 5269 7665 7222 2c0a 2020  name="River",.  
-0000cb70: 2020 736b 6970 5f72 6567 6973 7472 6174    skip_registrat
-0000cb80: 696f 6e3d 5472 7565 290a 6465 6620 7269  ion=True).def ri
-0000cb90: 7665 725f 7769 7468 5f74 6573 7428 6564  ver_with_test(ed
-0000cba0: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-0000cbb0: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
-0000cbc0: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
-0000cbd0: 293a 2020 200a 2020 2020 2222 2246 696e  ):   .    """Fin
-0000cbe0: 6420 7468 6520 5269 7665 7220 7769 6e6e  d the River winn
-0000cbf0: 6572 7320 7769 7468 2061 2074 6573 7420  ers with a test 
-0000cc00: 746f 2064 6574 6572 6d69 6e65 6420 6966  to determined if
-0000cc10: 2069 7420 7769 6c6c 2074 616b 6520 746f   it will take to
-0000cc20: 6f20 6c6f 6e67 2074 6f20 636f 6d70 7574  o long to comput
-0000cc30: 6520 7468 6520 5269 7665 7220 7769 6e6e  e the River winn
-0000cc40: 6572 732e 2049 6620 7468 6520 6361 6c63  ers. If the calc
-0000cc50: 756c 6174 696f 6e20 6f66 2074 6865 2077  ulation of the w
-0000cc60: 696e 6e65 7273 2077 696c 6c20 7461 6b65  inners will take
-0000cc70: 2074 6f6f 206c 6f6e 672c 2072 6574 7572   too long, retur
-0000cc80: 6e20 4e6f 6e65 2e20 0a20 2020 2020 2020  n None. .       
-0000cc90: 200a 2020 2020 2e2e 2069 6d70 6f72 7461   .    .. importa
-0000cca0: 6e74 3a3a 0a20 2020 2020 2020 2054 6869  nt::.        Thi
-0000ccb0: 7320 766f 7469 6e67 206d 6574 686f 6420  s voting method 
-0000ccc0: 7468 6174 206d 6967 6874 2072 6574 7572  that might retur
-0000ccd0: 6e20 4e6f 6e65 2072 6174 6865 7220 7468  n None rather th
-0000cce0: 616e 2061 206c 6973 7420 6f66 2063 616e  an a list of can
-0000ccf0: 6469 6461 7465 732e 2020 0a0a 2020 2020  didates.  ..    
-0000cd00: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-0000cd10: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-0000cd20: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-0000cd30: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-0000cd40: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-0000cd50: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-0000cd60: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-0000cd70: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-0000cd80: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-0000cd90: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-0000cda0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-0000cdb0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-0000cdc0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-0000cdd0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-0000cde0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-0000cdf0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-0000ce00: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-0000ce10: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-0000ce20: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-0000ce30: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-0000ce40: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-0000ce50: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-0000ce60: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-0000ce70: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-0000ce80: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-0000ce90: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-0000cea0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-0000ceb0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-0000cec0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-0000ced0: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
-0000cee0: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
-0000cef0: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
-0000cf00: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
-0000cf10: 202e 2e20 7365 6561 6c73 6f3a 3a0a 0a20   .. seealso::.. 
-0000cf20: 2020 2020 2020 203a 6d65 7468 3a60 7072         :meth:`pr
-0000cf30: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
-0000cf40: 5f62 6173 6564 5f6d 6574 686f 6473 2e72  _based_methods.r
-0000cf50: 616e 6b65 645f 7061 6972 735f 7769 7468  anked_pairs_with
-0000cf60: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-0000cf70: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000cf80: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000cf90: 7269 7665 7260 0a0a 2020 2020 2222 220a  river`..    """.
-0000cfa0: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-0000cfb0: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-0000cfc0: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-0000cfd0: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
-0000cfe0: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
-0000cff0: 6369 6478 5f74 6f5f 6361 6e64 203d 207b  cidx_to_cand = {
-0000d000: 6369 6478 3a20 6320 666f 7220 6369 6478  cidx: c for cidx
-0000d010: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
-0000d020: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
-0000d030: 2020 2020 6361 6e64 5f74 6f5f 6369 6478      cand_to_cidx
-0000d040: 203d 207b 633a 2063 6964 7820 666f 7220   = {c: cidx for 
-0000d050: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
-0000d060: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
-0000d070: 7d20 200a 0a20 2020 2073 7472 656e 6774  }  ..    strengt
-0000d080: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-0000d090: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-0000d0a0: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-0000d0b0: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-0000d0c0: 6e67 7468 5f66 756e 6374 696f 6e20 2020  ngth_function   
-0000d0d0: 200a 0a20 2020 2063 7720 3d20 6564 6174   ..    cw = edat
-0000d0e0: 612e 636f 6e64 6f72 6365 745f 7769 6e6e  a.condorcet_winn
-0000d0f0: 6572 2863 7572 725f 6361 6e64 733d 6375  er(curr_cands=cu
-0000d100: 7272 5f63 616e 6473 290a 2020 2020 2320  rr_cands).    # 
-0000d110: 5261 6e6b 6564 2050 6169 7273 2069 7320  Ranked Pairs is 
-0000d120: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
-0000d130: 7465 6e74 2c20 736f 2073 696d 706c 7920  tent, so simply 
-0000d140: 7265 7475 726e 2074 6865 2043 6f6e 646f  return the Condo
-0000d150: 7263 6574 2077 696e 6e65 7220 6966 2065  rcet winner if e
-0000d160: 7869 7374 730a 2020 2020 6966 2063 7720  xists.    if cw 
-0000d170: 6973 206e 6f74 204e 6f6e 653a 200a 2020  is not None: .  
-0000d180: 2020 2020 2020 7769 6e6e 6572 7320 3d20        winners = 
-0000d190: 5b63 775d 0a20 2020 2065 6c73 653a 0a20  [cw].    else:. 
-0000d1a0: 2020 2020 2020 2077 5f65 6467 6573 203d         w_edges =
-0000d1b0: 205b 2863 312c 2063 322c 2073 7472 656e   [(c1, c2, stren
-0000d1c0: 6774 685f 6675 6e63 7469 6f6e 2863 312c  gth_function(c1,
-0000d1d0: 2063 3229 2920 666f 7220 6331 2069 6e20   c2)) for c1 in 
-0000d1e0: 6361 6e64 6964 6174 6573 2066 6f72 2063  candidates for c
-0000d1f0: 3220 696e 2063 616e 6469 6461 7465 7320  2 in candidates 
-0000d200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d210: 2020 2020 6966 2063 3120 213d 2063 3220      if c1 != c2 
-0000d220: 616e 6420 2865 6461 7461 2e6d 616a 6f72  and (edata.major
-0000d230: 6974 795f 7072 6566 6572 7328 6331 2c20  ity_prefers(c1, 
-0000d240: 6332 2920 6f72 2065 6461 7461 2e69 735f  c2) or edata.is_
-0000d250: 7469 6564 2863 312c 2063 3229 295d 0a20  tied(c1, c2))]. 
-0000d260: 2020 2020 2020 2077 696e 6e65 7273 203d         winners =
-0000d270: 206c 6973 7428 2920 2020 2020 2020 2020   list()         
-0000d280: 2020 200a 2020 2020 2020 2020 7374 7265     .        stre
-0000d290: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
-0000d2a0: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
-0000d2b0: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
-0000d2c0: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
-0000d2d0: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
-0000d2e0: 6564 6765 7320 3d20 5b5b 6520 666f 7220  edges = [[e for 
-0000d2f0: 6520 696e 2077 5f65 6467 6573 2069 6620  e in w_edges if 
-0000d300: 655b 325d 203d 3d20 735d 2066 6f72 2073  e[2] == s] for s
-0000d310: 2069 6e20 7374 7265 6e67 7468 735d 0a20   in strengths]. 
-0000d320: 2020 2020 2020 2069 6620 6e70 2e70 726f         if np.pro
-0000d330: 6428 5b6d 6174 682e 6661 6374 6f72 6961  d([math.factoria
-0000d340: 6c28 6c65 6e28 6573 2929 2066 6f72 2065  l(len(es)) for e
-0000d350: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
-0000d360: 735d 2920 3e20 3330 3030 3a20 0a20 2020  s]) > 3000: .   
-0000d370: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000d380: 4e6f 6e65 0a20 2020 2020 2020 2065 6c73  None.        els
-0000d390: 653a 200a 2020 2020 2020 2020 2020 2020  e: .            
-0000d3a0: 7462 7320 3d20 7072 6f64 7563 7428 2a5b  tbs = product(*[
-0000d3b0: 7065 726d 7574 6174 696f 6e73 2865 6467  permutations(edg
-0000d3c0: 6573 2920 666f 7220 6564 6765 7320 696e  es) for edges in
-0000d3d0: 2073 6f72 7465 645f 6564 6765 735d 290a   sorted_edges]).
-0000d3e0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000d3f0: 7462 2069 6e20 7462 733a 0a20 2020 2020  tb in tbs:.     
-0000d400: 2020 2020 2020 2020 2020 2065 6467 6573             edges
-0000d410: 203d 2066 6c61 7474 656e 2874 6229 0a20   = flatten(tb). 
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d430: 765f 6465 6665 6174 203d 2053 504f 286c  v_defeat = SPO(l
-0000d440: 656e 2863 616e 6469 6461 7465 7329 290a  en(candidates)).
-0000d450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d460: 666f 7220 6530 2c65 312c 7320 696e 2065  for e0,e1,s in e
-0000d470: 6467 6573 3a20 0a20 2020 2020 2020 2020  dges: .         
-0000d480: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000d490: 7420 7276 5f64 6566 6561 742e 505b 6361  t rv_defeat.P[ca
-0000d4a0: 6e64 5f74 6f5f 6369 6478 5b65 315d 5d5b  nd_to_cidx[e1]][
-0000d4b0: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
-0000d4c0: 5d20 616e 6420 6c65 6e28 7276 5f64 6566  ] and len(rv_def
-0000d4d0: 6561 742e 7072 6564 735b 6361 6e64 5f74  eat.preds[cand_t
-0000d4e0: 6f5f 6369 6478 5b65 315d 5d29 203d 3d20  o_cidx[e1]]) == 
-0000d4f0: 303a 0a20 2020 2020 2020 2020 2020 2020  0:.             
-0000d500: 2020 2020 2020 2020 2020 2072 765f 6465             rv_de
-0000d510: 6665 6174 2e61 6464 2863 616e 645f 746f  feat.add(cand_to
-0000d520: 5f63 6964 785b 6530 5d2c 6361 6e64 5f74  _cidx[e0],cand_t
-0000d530: 6f5f 6369 6478 5b65 315d 290a 2020 2020  o_cidx[e1]).    
-0000d540: 2020 2020 2020 2020 2020 2020 7769 6e6e              winn
-0000d550: 6572 732e 6170 7065 6e64 2863 6964 785f  ers.append(cidx_
-0000d560: 746f 5f63 616e 645b 7276 5f64 6566 6561  to_cand[rv_defea
-0000d570: 742e 696e 6974 6961 6c5f 656c 656d 656e  t.initial_elemen
-0000d580: 7473 2829 5b30 5d5d 290a 2020 2020 7265  ts()[0]]).    re
-0000d590: 7475 726e 2073 6f72 7465 6428 6c69 7374  turn sorted(list
-0000d5a0: 2873 6574 2877 696e 6e65 7273 2929 290a  (set(winners))).
-0000d5b0: 0a72 705f 7462 5f70 726f 7065 7274 6965  .rp_tb_propertie
-0000d5c0: 7320 3d20 566f 7469 6e67 4d65 7468 6f64  s = VotingMethod
-0000d5d0: 5072 6f70 6572 7469 6573 280a 2020 2020  Properties(.    
-0000d5e0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
-0000d5f0: 3d54 7275 652c 200a 2020 2020 636f 6e64  =True, .    cond
-0000d600: 6f72 6365 745f 6c6f 7365 723d 5472 7565  orcet_loser=True
-0000d610: 2c0a 2020 2020 7061 7265 746f 5f64 6f6d  ,.    pareto_dom
-0000d620: 696e 616e 6365 3d54 7275 652c 0a20 2020  inance=True,.   
-0000d630: 2070 6f73 6974 6976 655f 696e 766f 6c76   positive_involv
-0000d640: 656d 656e 743d 4661 6c73 652c 200a 2020  ement=False, .  
-0000d650: 2020 290a 4076 6d28 6e61 6d65 3d22 5269    ).@vm(name="Ri
-0000d660: 7665 7220 5442 222c 0a20 2020 2070 726f  ver TB",.    pro
-0000d670: 7065 7274 6965 733d 7270 5f74 625f 7072  perties=rp_tb_pr
-0000d680: 6f70 6572 7469 6573 2c0a 2020 2020 696e  operties,.    in
-0000d690: 7075 745f 7479 7065 733d 5b45 6c65 6374  put_types=[Elect
-0000d6a0: 696f 6e54 7970 6573 2e50 524f 4649 4c45  ionTypes.PROFILE
-0000d6b0: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
-0000d6c0: 5052 4f46 494c 455f 5749 5448 5f54 4945  PROFILE_WITH_TIE
-0000d6d0: 532c 2045 6c65 6374 696f 6e54 7970 6573  S, ElectionTypes
-0000d6e0: 2e4d 4152 4749 4e5f 4752 4150 485d 290a  .MARGIN_GRAPH]).
-0000d6f0: 6465 6620 7269 7665 725f 7462 2865 6461  def river_tb(eda
-0000d700: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-0000d710: 204e 6f6e 652c 2074 6965 5f62 7265 616b   None, tie_break
-0000d720: 6572 203d 204e 6f6e 652c 2073 7472 656e  er = None, stren
-0000d730: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-0000d740: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-0000d750: 0a20 2020 2052 6976 6572 2077 6974 6820  .    River with 
-0000d760: 6120 6669 7865 6420 6c69 6e65 6172 206f  a fixed linear o
-0000d770: 7264 6572 206f 6e20 7468 6520 6361 6e64  rder on the cand
-0000d780: 6964 6174 6573 2074 6f20 6272 6561 6b20  idates to break 
-0000d790: 616e 7920 7469 6573 2069 6e20 7468 6520  any ties in the 
-0000d7a0: 6d61 7267 696e 732e 2020 5369 6e63 6520  margins.  Since 
-0000d7b0: 7468 6520 7469 655f 6272 6561 6b65 7220  the tie_breaker 
-0000d7c0: 6973 2061 206c 696e 6561 7220 6f72 6465  is a linear orde
-0000d7d0: 722c 2074 6869 7320 6d65 7468 6f64 2069  r, this method i
-0000d7e0: 7320 7265 736f 6c75 7465 2e20 2020 0a0a  s resolute.   ..
-0000d7f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000d800: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-0000d810: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-0000d820: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-0000d830: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-0000d840: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
-0000d850: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
-0000d860: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-0000d870: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-0000d880: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-0000d890: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-0000d8a0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-0000d8b0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-0000d8c0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-0000d8d0: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-0000d8e0: 616e 6473 6060 0a20 2020 2020 2020 2074  ands``.        t
-0000d8f0: 6965 5f62 7265 616b 6572 2028 4c69 7374  ie_breaker (List
-0000d900: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
-0000d910: 3a20 4120 6c69 6e65 6172 206f 7264 6572  : A linear order
-0000d920: 206f 6e20 7468 6520 6361 6e64 6964 6174   on the candidat
-0000d930: 6573 2e20 2049 6620 6e6f 7420 7365 742c  es.  If not set,
-0000d940: 2074 6865 6e20 7468 6520 6361 6e64 6964   then the candid
-0000d950: 6174 6573 2061 7265 2073 6f72 7465 6420  ates are sorted 
-0000d960: 696e 2061 7363 656e 6469 6e67 206f 7264  in ascending ord
-0000d970: 6572 2e0a 2020 2020 2020 2020 7374 7265  er..        stre
-0000d980: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
-0000d990: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
-0000d9a0: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
-0000d9b0: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0000d9c0: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
-0000d9d0: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
-0000d9e0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
-0000d9f0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
-0000da00: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
-0000da10: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
-0000da20: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
-0000da30: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
-0000da40: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
-0000da50: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
-0000da60: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
-0000da70: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
-0000da80: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
-0000da90: 2020 2222 220a 2020 2020 6361 6e64 6964    """.    candid
-0000daa0: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
-0000dab0: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
-0000dac0: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
-0000dad0: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
-0000dae0: 200a 2020 2020 6369 6478 5f74 6f5f 6361   .    cidx_to_ca
-0000daf0: 6e64 203d 207b 6369 6478 3a20 6320 666f  nd = {cidx: c fo
-0000db00: 7220 6369 6478 2c20 6320 696e 2065 6e75  r cidx, c in enu
-0000db10: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
-0000db20: 7329 7d20 200a 2020 2020 6361 6e64 5f74  s)}  .    cand_t
-0000db30: 6f5f 6369 6478 203d 207b 633a 2063 6964  o_cidx = {c: cid
-0000db40: 7820 666f 7220 6369 6478 2c20 6320 696e  x for cidx, c in
-0000db50: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
-0000db60: 6461 7465 7329 7d20 200a 2020 2020 7374  dates)}  .    st
-0000db70: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-0000db80: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
-0000db90: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
-0000dba0: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
-0000dbb0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000dbc0: 6f6e 2020 2020 0a0a 2020 2020 7462 5f72  on    ..    tb_r
-0000dbd0: 616e 6b69 6e67 203d 2074 6965 5f62 7265  anking = tie_bre
-0000dbe0: 616b 6572 2069 6620 7469 655f 6272 6561  aker if tie_brea
-0000dbf0: 6b65 7220 6973 206e 6f74 204e 6f6e 6520  ker is not None 
-0000dc00: 656c 7365 2073 6f72 7465 6428 6c69 7374  else sorted(list
-0000dc10: 2863 616e 6469 6461 7465 7329 290a 0a20  (candidates)).. 
-0000dc20: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
-0000dc30: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
-0000dc40: 7572 725f 6361 6e64 733d 6375 7272 5f63  urr_cands=curr_c
-0000dc50: 616e 6473 290a 2020 2020 2320 5269 7665  ands).    # Rive
-0000dc60: 7220 6973 2043 6f6e 646f 7263 6574 2063  r is Condorcet c
-0000dc70: 6f6e 7369 7374 656e 742c 2073 6f20 7369  onsistent, so si
-0000dc80: 6d70 6c79 2072 6574 7572 6e20 7468 6520  mply return the 
-0000dc90: 436f 6e64 6f72 6365 7420 7769 6e6e 6572  Condorcet winner
-0000dca0: 2069 6620 6578 6973 7473 0a20 2020 2069   if exists.    i
-0000dcb0: 6620 6377 2069 7320 6e6f 7420 4e6f 6e65  f cw is not None
-0000dcc0: 3a20 0a20 2020 2020 2020 2077 696e 6e65  : .        winne
-0000dcd0: 7273 203d 205b 6377 5d0a 2020 2020 656c  rs = [cw].    el
-0000dce0: 7365 3a0a 2020 2020 2020 2020 775f 6564  se:.        w_ed
-0000dcf0: 6765 7320 3d20 5b28 6331 2c20 6332 2c20  ges = [(c1, c2, 
-0000dd00: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-0000dd10: 6e28 6331 2c20 6332 2929 2066 6f72 2063  n(c1, c2)) for c
-0000dd20: 3120 696e 2063 616e 6469 6461 7465 7320  1 in candidates 
-0000dd30: 666f 7220 6332 2069 6e20 6361 6e64 6964  for c2 in candid
-0000dd40: 6174 6573 2069 6620 6331 2021 3d20 6332  ates if c1 != c2
-0000dd50: 2061 6e64 2028 6564 6174 612e 6d61 6a6f   and (edata.majo
-0000dd60: 7269 7479 5f70 7265 6665 7273 2863 312c  rity_prefers(c1,
-0000dd70: 2063 3229 206f 7220 6564 6174 612e 6973   c2) or edata.is
-0000dd80: 5f74 6965 6428 6331 2c20 6332 2929 5d0a  _tied(c1, c2))].
-0000dd90: 2020 2020 2020 2020 7769 6e6e 6572 7320          winners 
-0000dda0: 3d20 6c69 7374 2829 2020 0a20 2020 2020  = list()  .     
-0000ddb0: 2020 2073 7472 656e 6774 6873 203d 2073     strengths = s
-0000ddc0: 6f72 7465 6428 6c69 7374 2873 6574 285b  orted(list(set([
-0000ddd0: 655b 325d 2066 6f72 2065 2069 6e20 775f  e[2] for e in w_
-0000dde0: 6564 6765 735d 2929 2c20 7265 7665 7273  edges])), revers
-0000ddf0: 653d 5472 7565 290a 0a20 2020 2020 2020  e=True)..       
-0000de00: 2072 765f 6465 6665 6174 203d 2053 504f   rv_defeat = SPO
-0000de10: 286c 656e 2863 616e 6469 6461 7465 7329  (len(candidates)
-0000de20: 290a 0a20 2020 2020 2020 2066 6f72 2073  )..        for s
-0000de30: 2069 6e20 7374 7265 6e67 7468 733a 200a   in strengths: .
-0000de40: 2020 2020 2020 2020 2020 2020 6564 6765              edge
-0000de50: 7320 3d20 5b65 2066 6f72 2065 2069 6e20  s = [e for e in 
-0000de60: 775f 6564 6765 7320 6966 2065 5b32 5d20  w_edges if e[2] 
-0000de70: 3d3d 2073 5d0a 2020 2020 2020 2020 2020  == s].          
-0000de80: 2020 0a20 2020 2020 2020 2020 2020 2023    .            #
-0000de90: 2062 7265 616b 2074 6965 7320 7573 696e   break ties usin
-0000dea0: 6720 7468 6520 6c65 7869 636f 6772 6170  g the lexicograp
-0000deb0: 6869 6320 6f72 6465 7269 6e67 206f 6e20  hic ordering on 
-0000dec0: 7475 706c 6573 2067 6976 656e 2074 625f  tuples given tb_
-0000ded0: 7261 6e6b 696e 670a 2020 2020 2020 2020  ranking.        
-0000dee0: 2020 2020 736f 7274 6564 5f65 6467 6573      sorted_edges
-0000def0: 203d 2073 6f72 7465 6428 6564 6765 732c   = sorted(edges,
-0000df00: 206b 6579 203d 206c 616d 6264 6120 653a   key = lambda e:
-0000df10: 2028 7462 5f72 616e 6b69 6e67 2e69 6e64   (tb_ranking.ind
-0000df20: 6578 2865 5b30 5d29 2c20 7462 5f72 616e  ex(e[0]), tb_ran
-0000df30: 6b69 6e67 2e69 6e64 6578 2865 5b31 5d29  king.index(e[1])
-0000df40: 292c 2072 6576 6572 7365 3d46 616c 7365  ), reverse=False
-0000df50: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000df60: 7220 6530 2c65 312c 7320 696e 2073 6f72  r e0,e1,s in sor
-0000df70: 7465 645f 6564 6765 733a 200a 2020 2020  ted_edges: .    
-0000df80: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000df90: 6f74 2072 765f 6465 6665 6174 2e50 5b63  ot rv_defeat.P[c
-0000dfa0: 616e 645f 746f 5f63 6964 785b 6531 5d5d  and_to_cidx[e1]]
-0000dfb0: 5b63 616e 645f 746f 5f63 6964 785b 6530  [cand_to_cidx[e0
-0000dfc0: 5d5d 2061 6e64 206c 656e 2872 765f 6465  ]] and len(rv_de
-0000dfd0: 6665 6174 2e70 7265 6473 5b63 616e 645f  feat.preds[cand_
-0000dfe0: 746f 5f63 6964 785b 6531 5d5d 2920 3d3d  to_cidx[e1]]) ==
-0000dff0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
-0000e000: 2020 2020 2020 2020 7276 5f64 6566 6561          rv_defea
-0000e010: 742e 6164 6428 6361 6e64 5f74 6f5f 6369  t.add(cand_to_ci
-0000e020: 6478 5b65 305d 2c63 616e 645f 746f 5f63  dx[e0],cand_to_c
-0000e030: 6964 785b 6531 5d29 0a20 2020 2020 2020  idx[e1]).       
-0000e040: 2020 2020 2077 696e 6e65 7273 2e61 7070       winners.app
-0000e050: 656e 6428 6369 6478 5f74 6f5f 6361 6e64  end(cidx_to_cand
-0000e060: 5b72 765f 6465 6665 6174 2e69 6e69 7469  [rv_defeat.initi
-0000e070: 616c 5f65 6c65 6d65 6e74 7328 295b 305d  al_elements()[0]
-0000e080: 5d29 0a20 2020 2072 6574 7572 6e20 736f  ]).    return so
-0000e090: 7274 6564 286c 6973 7428 7365 7428 7769  rted(list(set(wi
-0000e0a0: 6e6e 6572 7329 2929 0a0a 7269 7665 725f  nners)))..river_
-0000e0b0: 7a74 5f70 726f 7065 7274 6965 7320 3d20  zt_properties = 
-0000e0c0: 566f 7469 6e67 4d65 7468 6f64 5072 6f70  VotingMethodProp
-0000e0d0: 6572 7469 6573 280a 2020 2020 636f 6e64  erties(.    cond
-0000e0e0: 6f72 6365 745f 7769 6e6e 6572 3d54 7275  orcet_winner=Tru
-0000e0f0: 652c 200a 2020 2020 636f 6e64 6f72 6365  e, .    condorce
-0000e100: 745f 6c6f 7365 723d 5472 7565 2c0a 2020  t_loser=True,.  
-0000e110: 2020 7061 7265 746f 5f64 6f6d 696e 616e    pareto_dominan
-0000e120: 6365 3d54 7275 652c 0a20 2020 2070 6f73  ce=True,.    pos
-0000e130: 6974 6976 655f 696e 766f 6c76 656d 656e  itive_involvemen
-0000e140: 743d 4661 6c73 652c 200a 2020 2020 290a  t=False, .    ).
-0000e150: 4076 6d28 6e61 6d65 3d22 5269 7665 7220  @vm(name="River 
-0000e160: 5a54 222c 0a20 2020 2070 726f 7065 7274  ZT",.    propert
-0000e170: 6965 733d 7269 7665 725f 7a74 5f70 726f  ies=river_zt_pro
-0000e180: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
-0000e190: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
-0000e1a0: 6f6e 5479 7065 732e 5052 4f46 494c 455d  onTypes.PROFILE]
-0000e1b0: 290a 6465 6620 7269 7665 725f 7a74 2870  ).def river_zt(p
-0000e1c0: 726f 6669 6c65 2c20 6375 7272 5f63 616e  rofile, curr_can
-0000e1d0: 6473 203d 204e 6f6e 652c 2073 7472 656e  ds = None, stren
-0000e1e0: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
-0000e1f0: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
-0000e200: 5269 7665 7220 7768 6572 6520 6120 6669  River where a fi
-0000e210: 7865 6420 766f 7465 7220 6272 6561 6b73  xed voter breaks
-0000e220: 2061 6e79 2074 6965 7320 696e 2074 6865   any ties in the
-0000e230: 206d 6172 6769 6e73 2e20 2049 7420 6973   margins.  It is
-0000e240: 2061 6c77 6179 7320 7468 6520 766f 7465   always the vote
-0000e250: 7220 696e 2070 6f73 6974 696f 6e20 3020  r in position 0 
-0000e260: 7468 6174 2062 7265 616b 7320 7468 6520  that breaks the 
-0000e270: 7469 6573 2e20 2053 696e 6365 2076 6f74  ties.  Since vot
-0000e280: 6572 7320 6861 7665 2073 7472 6963 7420  ers have strict 
-0000e290: 7072 6566 6572 656e 6365 732c 2074 6869  preferences, thi
-0000e2a0: 7320 6d65 7468 6f64 2069 7320 7265 736f  s method is reso
-0000e2b0: 6c75 7465 2e20 200a 0a20 2020 2041 7267  lute.  ..    Arg
-0000e2c0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-0000e2d0: 2028 5072 6f66 696c 6529 3a20 4120 7072   (Profile): A pr
-0000e2e0: 6f66 696c 6520 6f66 206c 696e 6561 7220  ofile of linear 
-0000e2f0: 6f72 6465 7273 0a20 2020 2020 2020 2063  orders.        c
-0000e300: 7572 725f 6361 6e64 7320 284c 6973 745b  urr_cands (List[
-0000e310: 696e 745d 2c20 6f70 7469 6f6e 616c 293a  int], optional):
-0000e320: 2049 6620 7365 742c 2074 6865 6e20 6669   If set, then fi
-0000e330: 6e64 2074 6865 2077 696e 6e65 7273 2066  nd the winners f
-0000e340: 6f72 2074 6865 2070 726f 6669 6c65 2072  or the profile r
-0000e350: 6573 7472 6963 7465 6420 746f 2074 6865  estricted to the
-0000e360: 2063 616e 6469 6461 7465 7320 696e 2060   candidates in `
-0000e370: 6063 7572 725f 6361 6e64 7360 600a 0a20  `curr_cands``.. 
-0000e380: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-0000e390: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-0000e3a0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-0000e3b0: 2e20 0a0a 2020 2020 2e2e 2073 6565 616c  . ..    .. seeal
-0000e3c0: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
-0000e3d0: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-0000e3e0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000e3f0: 7468 6f64 732e 7269 7665 7260 2c20 3a6d  thods.river`, :m
-0000e400: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
-0000e410: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
-0000e420: 7468 6f64 732e 7269 7665 725f 7769 7468  thods.river_with
-0000e430: 5f74 6573 7460 2c20 3a6d 6574 683a 6070  _test`, :meth:`p
-0000e440: 7265 665f 766f 7469 6e67 2e6d 6172 6769  ref_voting.margi
-0000e450: 6e5f 6261 7365 645f 6d65 7468 6f64 732e  n_based_methods.
-0000e460: 7261 6e6b 6564 5f70 6169 7273 600a 0a20  ranked_pairs`.. 
-0000e470: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
-0000e480: 6361 6e64 6964 6174 6573 203d 2070 726f  candidates = pro
-0000e490: 6669 6c65 2e63 616e 6469 6461 7465 7320  file.candidates 
-0000e4a0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
-0000e4b0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
-0000e4c0: 6361 6e64 7320 2020 200a 2020 2020 0a20  cands    .    . 
-0000e4d0: 2020 2023 2074 6865 2074 6965 2d62 7265     # the tie-bre
-0000e4e0: 616b 6572 2069 7320 616c 7761 7973 2074  aker is always t
-0000e4f0: 6865 2066 6972 7374 2076 6f74 6572 2e20  he first voter. 
-0000e500: 0a20 2020 2074 625f 7261 6e6b 696e 6720  .    tb_ranking 
-0000e510: 3d20 7475 706c 6528 5b63 2066 6f72 2063  = tuple([c for c
-0000e520: 2069 6e20 6c69 7374 2870 726f 6669 6c65   in list(profile
-0000e530: 2e5f 7261 6e6b 696e 6773 5b30 5d29 2069  ._rankings[0]) i
-0000e540: 6620 6320 696e 2063 616e 6469 6461 7465  f c in candidate
-0000e550: 735d 290a 2020 2020 0a20 2020 2072 6574  s]).    .    ret
-0000e560: 7572 6e20 7269 7665 725f 7462 2870 726f  urn river_tb(pro
-0000e570: 6669 6c65 2c20 6375 7272 5f63 616e 6473  file, curr_cands
-0000e580: 203d 2063 7572 725f 6361 6e64 732c 2074   = curr_cands, t
-0000e590: 6965 5f62 7265 616b 6572 203d 2074 625f  ie_breaker = tb_
-0000e5a0: 7261 6e6b 696e 672c 2073 7472 656e 6774  ranking, strengt
-0000e5b0: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
-0000e5c0: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
-0000e5d0: 2020 2020 0a0a 2320 5369 6d70 6c65 2053      ..# Simple S
-0000e5e0: 7461 626c 6520 566f 7469 6e67 200a 6465  table Voting .de
-0000e5f0: 6620 5f73 696d 706c 655f 7374 6162 6c65  f _simple_stable
-0000e600: 5f76 6f74 696e 6728 6375 7272 5f63 616e  _voting(curr_can
-0000e610: 6473 2c20 0a20 2020 2020 2020 2020 2020  ds, .           
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000e630: 6f72 7465 645f 6d61 7463 6865 732c 0a20  orted_matches,. 
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 2020 2020 2020 2020 206d 656d 5f73 765f           mem_sv_
-0000e660: 7769 6e6e 6572 7329 3a0a 2020 2020 2727  winners):.    ''
-0000e670: 270a 2020 2020 4465 7465 726d 696e 6520  '.    Determine 
-0000e680: 7468 6520 5369 6d70 6c65 2053 7461 626c  the Simple Stabl
-0000e690: 6520 566f 7469 6e67 2077 696e 6e65 7273  e Voting winners
-0000e6a0: 2077 6869 6c65 206b 6565 7069 6e67 2074   while keeping t
-0000e6b0: 7261 636b 200a 2020 2020 6f66 2074 6865  rack .    of the
-0000e6c0: 2077 696e 6e65 7273 2069 6e20 616e 7920   winners in any 
-0000e6d0: 7375 6270 726f 6669 6c65 7320 6368 6563  subprofiles chec
-0000e6e0: 6b65 6420 6475 7269 6e67 2063 6f6d 7075  ked during compu
-0000e6f0: 7461 7469 6f6e 2e20 0a20 2020 2027 2727  tation. .    '''
-0000e700: 0a20 2020 200a 2020 2020 7376 5f77 696e  .    .    sv_win
-0000e710: 6e65 7273 203d 206c 6973 7428 290a 2020  ners = list().  
-0000e720: 2020 2020 2020 0a20 2020 2069 6620 6c65        .    if le
-0000e730: 6e28 6375 7272 5f63 616e 6473 2920 3d3d  n(curr_cands) ==
-0000e740: 2031 3a20 0a20 2020 2020 2020 206d 656d   1: .        mem
-0000e750: 5f73 765f 7769 6e6e 6572 735b 7475 706c  _sv_winners[tupl
-0000e760: 6528 6375 7272 5f63 616e 6473 295d 203d  e(curr_cands)] =
-0000e770: 2063 7572 725f 6361 6e64 730a 2020 2020   curr_cands.    
-0000e780: 2020 2020 7265 7475 726e 2063 7572 725f      return curr_
-0000e790: 6361 6e64 732c 206d 656d 5f73 765f 7769  cands, mem_sv_wi
-0000e7a0: 6e6e 6572 730a 2020 2020 0a20 2020 206d  nners.    .    m
-0000e7b0: 6172 6769 6e5f 7769 746e 6573 7369 6e67  argin_witnessing
-0000e7c0: 5f77 696e 203d 202d 6d61 7468 2e69 6e66  _win = -math.inf
-0000e7d0: 0a0a 2020 2020 666f 7220 612c 2062 2c20  ..    for a, b, 
-0000e7e0: 7320 696e 2073 6f72 7465 645f 6d61 7463  s in sorted_matc
-0000e7f0: 6865 733a 0a20 2020 2020 2020 2069 6620  hes:.        if 
-0000e800: 7320 3c20 6d61 7267 696e 5f77 6974 6e65  s < margin_witne
-0000e810: 7373 696e 675f 7769 6e3a 200a 2020 2020  ssing_win: .    
-0000e820: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
-0000e830: 2020 2020 2020 6966 2061 206e 6f74 2069        if a not i
-0000e840: 6e20 7376 5f77 696e 6e65 7273 3a20 0a20  n sv_winners: . 
-0000e850: 2020 2020 2020 2020 2020 2063 616e 6473             cands
-0000e860: 5f6d 696e 7573 5f62 203d 205b 6320 666f  _minus_b = [c fo
-0000e870: 7220 6320 696e 2063 7572 725f 6361 6e64  r c in curr_cand
-0000e880: 7320 6966 2063 2021 3d20 625d 0a20 2020  s if c != b].   
-0000e890: 2020 2020 2020 2020 2063 616e 6473 5f6d           cands_m
-0000e8a0: 696e 7573 5f62 5f6b 6579 203d 2074 7570  inus_b_key = tup
-0000e8b0: 6c65 2873 6f72 7465 6428 6361 6e64 735f  le(sorted(cands_
-0000e8c0: 6d69 6e75 735f 6229 290a 2020 2020 2020  minus_b)).      
-0000e8d0: 2020 2020 2020 6966 2063 616e 6473 5f6d        if cands_m
-0000e8e0: 696e 7573 5f62 5f6b 6579 206e 6f74 2069  inus_b_key not i
-0000e8f0: 6e20 6d65 6d5f 7376 5f77 696e 6e65 7273  n mem_sv_winners
-0000e900: 2e6b 6579 7328 293a 200a 2020 2020 2020  .keys(): .      
-0000e910: 2020 2020 2020 2020 2020 7773 2c20 6d65            ws, me
-0000e920: 6d5f 7376 5f77 696e 6e65 7273 203d 205f  m_sv_winners = _
-0000e930: 7369 6d70 6c65 5f73 7461 626c 655f 766f  simple_stable_vo
-0000e940: 7469 6e67 2863 7572 725f 6361 6e64 7320  ting(curr_cands 
-0000e950: 3d20 6361 6e64 735f 6d69 6e75 735f 622c  = cands_minus_b,
-0000e960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e990: 2020 2020 2020 2020 2020 2020 736f 7274              sort
-0000e9a0: 6564 5f6d 6174 6368 6573 203d 205b 2861  ed_matches = [(a
-0000e9b0: 2c20 632c 2073 2920 666f 7220 612c 2063  , c, s) for a, c
-0000e9c0: 2c20 7320 696e 2073 6f72 7465 645f 6d61  , s in sorted_ma
-0000e9d0: 7463 6865 7320 6966 2061 2021 3d20 6220  tches if a != b 
-0000e9e0: 616e 6420 6320 213d 2062 5d2c 0a20 2020  and c != b],.   
-0000e9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
-0000ea30: 696e 6e65 7273 203d 206d 656d 5f73 765f  inners = mem_sv_
-0000ea40: 7769 6e6e 6572 7329 0a20 2020 2020 2020  winners).       
-0000ea50: 2020 2020 2020 2020 206d 656d 5f73 765f           mem_sv_
-0000ea60: 7769 6e6e 6572 735b 6361 6e64 735f 6d69  winners[cands_mi
-0000ea70: 6e75 735f 625f 6b65 795d 203d 2077 730a  nus_b_key] = ws.
-0000ea80: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000ea90: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
-0000eaa0: 2020 2077 7320 3d20 6d65 6d5f 7376 5f77     ws = mem_sv_w
-0000eab0: 696e 6e65 7273 5b63 616e 6473 5f6d 696e  inners[cands_min
-0000eac0: 7573 5f62 5f6b 6579 5d0a 2020 2020 2020  us_b_key].      
-0000ead0: 2020 2020 2020 6966 2061 2069 6e20 7773        if a in ws
-0000eae0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000eaf0: 2020 7376 5f77 696e 6e65 7273 2e61 7070    sv_winners.app
-0000eb00: 656e 6428 6129 0a20 2020 2020 2020 2020  end(a).         
-0000eb10: 2020 2020 2020 206d 6172 6769 6e5f 7769         margin_wi
-0000eb20: 746e 6573 7369 6e67 5f77 696e 203d 2073  tnessing_win = s
-0000eb30: 0a0a 2020 2020 7265 7475 726e 2073 765f  ..    return sv_
-0000eb40: 7769 6e6e 6572 732c 206d 656d 5f73 765f  winners, mem_sv_
-0000eb50: 7769 6e6e 6572 730a 2020 2020 0a0a 4076  winners.    ..@v
-0000eb60: 6d28 6e61 6d65 203d 2022 5369 6d70 6c65  m(name = "Simple
-0000eb70: 2053 7461 626c 6520 566f 7469 6e67 2229   Stable Voting")
-0000eb80: 0a64 6566 205f 7369 6d70 6c65 5f73 7461  .def _simple_sta
-0000eb90: 626c 655f 766f 7469 6e67 5f77 6974 685f  ble_voting_with_
-0000eba0: 636f 6e64 6f72 6365 745f 6368 6563 6b28  condorcet_check(
-0000ebb0: 0a20 2020 2065 6461 7461 2c20 0a20 2020  .    edata, .   
-0000ebc0: 2063 7572 725f 6361 6e64 7320 3d20 4e6f   curr_cands = No
-0000ebd0: 6e65 2c20 0a20 2020 2073 7472 656e 6774  ne, .    strengt
-0000ebe0: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
-0000ebf0: 6529 3a20 0a20 2020 2022 2222 5369 6d70  e): .    """Simp
-0000ec00: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
-0000ec10: 2069 7320 436f 6e64 6f72 6365 7420 636f   is Condorcet co
-0000ec20: 6e73 6973 7465 6e74 2e20 2020 4974 2069  nsistent.   It i
-0000ec30: 7320 6661 7374 6572 2074 6f20 736b 6970  s faster to skip
-0000ec40: 2065 7865 6375 7469 6e67 2074 6865 2072   executing the r
-0000ec50: 6563 7572 7369 7665 2061 6c67 6f72 6974  ecursive algorit
-0000ec60: 686d 2077 6865 6e20 7468 6572 6520 6973  hm when there is
-0000ec70: 2061 2043 6f6e 646f 7263 6574 2077 696e   a Condorcet win
-0000ec80: 6e65 7246 6972 7374 2063 6865 636b 2069  nerFirst check i
-0000ec90: 6620 7468 6572 6520 6973 2061 2043 6f6e  f there is a Con
-0000eca0: 646f 7263 6574 2077 696e 6e65 722e 2020  dorcet winner.  
-0000ecb0: 4966 2073 6f2c 2072 6574 7572 6e20 7468  If so, return th
-0000ecc0: 6520 436f 6e64 6f72 6365 7420 7769 6e6e  e Condorcet winn
-0000ecd0: 6572 2c20 6f74 6865 7277 6973 6520 6669  er, otherwise fi
-0000ece0: 6e64 2074 6865 2053 696d 706c 6520 5374  nd the Simple St
-0000ecf0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-0000ed00: 6572 2075 7369 6e67 205f 7369 6d70 6c65  er using _simple
-0000ed10: 5f73 7461 626c 655f 766f 7469 6e67 0a0a  _stable_voting..
-0000ed20: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000ed30: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-0000ed40: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-0000ed50: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-0000ed60: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-0000ed70: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
-0000ed80: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
-0000ed90: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
-0000eda0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
-0000edb0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
-0000edc0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
-0000edd0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
-0000ede0: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
-0000edf0: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
-0000ee00: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
-0000ee10: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
+00000290: 6573 2069 6d70 6f72 7420 456c 6563 7469  es import Electi
+000002a0: 6f6e 5479 7065 730a 696d 706f 7274 206d  onTypes.import m
+000002b0: 756c 7469 7072 6f63 6573 7369 6e67 2061  ultiprocessing a
+000002c0: 7320 6d70 0a66 726f 6d20 6d75 6c74 6970  s mp.from multip
+000002d0: 726f 6365 7373 696e 6720 696d 706f 7274  rocessing import
+000002e0: 2050 6f6f 6c0a 6672 6f6d 2066 756e 6374   Pool.from funct
+000002f0: 6f6f 6c73 2069 6d70 6f72 7420 7061 7274  ools import part
+00000300: 6961 6c0a 0a40 766d 286e 616d 6520 3d20  ial..@vm(name = 
+00000310: 224d 696e 696d 6178 222c 0a20 2020 2069  "Minimax",.    i
+00000320: 6e70 7574 5f74 7970 6573 3d5b 456c 6563  nput_types=[Elec
+00000330: 7469 6f6e 5479 7065 732e 5052 4f46 494c  tionTypes.PROFIL
+00000340: 452c 2045 6c65 6374 696f 6e54 7970 6573  E, ElectionTypes
+00000350: 2e50 524f 4649 4c45 5f57 4954 485f 5449  .PROFILE_WITH_TI
+00000360: 4553 2c20 456c 6563 7469 6f6e 5479 7065  ES, ElectionType
+00000370: 732e 4d41 5247 494e 5f47 5241 5048 5d0a  s.MARGIN_GRAPH].
+00000380: 2020 2020 290a 6465 6620 6d69 6e69 6d61      ).def minima
+00000390: 7828 6564 6174 612c 2063 7572 725f 6361  x(edata, curr_ca
+000003a0: 6e64 7320 3d20 4e6f 6e65 2c20 7374 7265  nds = None, stre
+000003b0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+000003c0: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+000003d0: 220a 2020 2020 5468 6520 4d69 6e69 6d61  ".    The Minima
+000003e0: 7820 7769 6e6e 6572 7320 6172 6520 7468  x winners are th
+000003f0: 6520 6361 6e64 6964 6174 6573 2077 6974  e candidates wit
+00000400: 6820 7468 6520 736d 616c 6c65 7374 206d  h the smallest m
+00000410: 6178 696d 756d 2070 6169 7277 6973 6520  aximum pairwise 
+00000420: 6c6f 7373 2e20 2054 6861 7420 6973 2c20  loss.  That is, 
+00000430: 666f 7220 6561 6368 2063 616e 6469 6461  for each candida
+00000440: 7465 203a 6d61 7468 3a60 6160 2c20 6669  te :math:`a`, fi
+00000450: 6e64 2074 6865 2062 6967 6765 7374 206d  nd the biggest m
+00000460: 6172 6769 6e20 6f66 2061 2063 616e 6469  argin of a candi
+00000470: 6461 7465 203a 6d61 7468 3a60 6260 206f  date :math:`b` o
+00000480: 7665 7220 3a6d 6174 683a 6061 602c 2074  ver :math:`a`, t
+00000490: 6865 6e20 656c 6563 7420 7468 6520 6361  hen elect the ca
+000004a0: 6e64 6964 6174 6528 7329 2077 6974 6820  ndidate(s) with 
+000004b0: 7468 6520 736d 616c 6c65 7374 2073 7563  the smallest suc
+000004c0: 6820 6c6f 7373 2e20 416c 736f 206b 6e6f  h loss. Also kno
+000004d0: 776e 2061 7320 7468 6520 5369 6d70 736f  wn as the Simpso
+000004e0: 6e2d 4b72 616d 6572 2052 756c 652e 0a20  n-Kramer Rule.. 
+000004f0: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
+00000500: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+00000510: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+00000520: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+00000530: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+00000540: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+00000550: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+00000560: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+00000570: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+00000580: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00000590: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+000005a0: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+000005b0: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+000005c0: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+000005d0: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+000005e0: 7272 5f63 616e 6473 6060 0a0a 2020 2020  rr_cands``..    
+000005f0: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+00000600: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+00000610: 6f66 2063 616e 6469 6461 7465 730a 0a20  of candidates.. 
+00000620: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
+00000630: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
+00000640: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00000650: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00000660: 2e6d 696e 696d 6178 5f73 636f 7265 7360  .minimax_scores`
+00000670: 0a0a 2020 2020 3a45 7861 6d70 6c65 3a20  ..    :Example: 
+00000680: 0a0a 2020 2020 2e2e 2070 6c6f 743a 3a20  ..    .. plot:: 
+00000690: 206d 6172 6769 6e5f 6772 6170 6873 5f65   margin_graphs_e
+000006a0: 7861 6d70 6c65 732f 6d67 5f65 785f 6d69  xamples/mg_ex_mi
+000006b0: 6e69 6d61 782e 7079 0a20 2020 2020 2020  nimax.py.       
+000006c0: 203a 636f 6e74 6578 743a 2072 6573 6574   :context: reset
+000006d0: 2020 0a20 2020 2020 2020 203a 696e 636c    .        :incl
+000006e0: 7564 652d 736f 7572 6365 3a20 5472 7565  ude-source: True
+000006f0: 0a0a 0a20 2020 202e 2e20 636f 6465 2d62  ...    .. code-b
+00000700: 6c6f 636b 3a3a 200a 0a20 2020 2020 2020  lock:: ..       
+00000710: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00000720: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00000730: 6574 686f 6473 2069 6d70 6f72 7420 6d69  ethods import mi
+00000740: 6e69 6d61 780a 0a20 2020 2020 2020 206d  nimax..        m
+00000750: 696e 696d 6178 2e64 6973 706c 6179 2870  inimax.display(p
+00000760: 726f 6629 0a0a 0a20 2020 202e 2e20 6578  rof)...    .. ex
+00000770: 6563 5f63 6f64 653a 3a20 0a20 2020 2020  ec_code:: .     
+00000780: 2020 203a 6869 6465 5f63 6f64 653a 0a0a     :hide_code:..
+00000790: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+000007a0: 665f 766f 7469 6e67 2e70 726f 6669 6c65  f_voting.profile
+000007b0: 7320 696d 706f 7274 2050 726f 6669 6c65  s import Profile
+000007c0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+000007d0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+000007e0: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+000007f0: 6d70 6f72 7420 6d69 6e69 6d61 780a 2020  mport minimax.  
+00000800: 2020 2020 2020 0a20 2020 2020 2020 2070        .        p
+00000810: 726f 6620 3d20 5072 6f66 696c 6528 5b5b  rof = Profile([[
+00000820: 332c 2030 2c20 312c 2032 5d2c 205b 312c  3, 0, 1, 2], [1,
+00000830: 2033 2c20 322c 2030 5d2c 205b 312c 2033   3, 2, 0], [1, 3
+00000840: 2c20 302c 2032 5d2c 205b 312c 2032 2c20  , 0, 2], [1, 2, 
+00000850: 302c 2033 5d2c 205b 332c 2032 2c20 302c  0, 3], [3, 2, 0,
+00000860: 2031 5d2c 205b 302c 2032 2c20 312c 2033   1], [0, 2, 1, 3
+00000870: 5d5d 2c20 5b31 2c20 312c 2031 2c20 312c  ]], [1, 1, 1, 1,
+00000880: 2032 2c20 315d 290a 0a20 2020 2020 2020   2, 1])..       
+00000890: 206d 696e 696d 6178 2e64 6973 706c 6179   minimax.display
+000008a0: 2870 726f 6629 0a0a 2020 2020 2222 220a  (prof)..    """.
+000008b0: 0a20 2020 2063 616e 6469 6461 7465 7320  .    candidates 
+000008c0: 3d20 6564 6174 612e 6361 6e64 6964 6174  = edata.candidat
+000008d0: 6573 2069 6620 6375 7272 5f63 616e 6473  es if curr_cands
+000008e0: 2069 7320 4e6f 6e65 2065 6c73 6520 6375   is None else cu
+000008f0: 7272 5f63 616e 6473 2020 2020 0a20 2020  rr_cands    .   
+00000900: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00000910: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+00000920: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+00000930: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+00000940: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+00000950: 6374 696f 6e0a 0a20 2020 2073 636f 7265  ction..    score
+00000960: 7320 3d20 7b63 3a20 6d61 7828 5b73 7472  s = {c: max([str
+00000970: 656e 6774 685f 6675 6e63 7469 6f6e 285f  ength_function(_
+00000980: 632c 2063 2920 666f 7220 5f63 2069 6e20  c, c) for _c in 
+00000990: 6564 6174 612e 646f 6d69 6e61 746f 7273  edata.dominators
+000009a0: 2863 2920 6966 205f 6320 696e 2063 616e  (c) if _c in can
+000009b0: 6469 6461 7465 735d 2920 6966 2061 6e79  didates]) if any
+000009c0: 285b 5f63 2069 6e20 6564 6174 612e 646f  ([_c in edata.do
+000009d0: 6d69 6e61 746f 7273 2863 2920 666f 7220  minators(c) for 
+000009e0: 5f63 2069 6e20 6361 6e64 6964 6174 6573  _c in candidates
+000009f0: 5d29 2065 6c73 6520 3020 0a20 2020 2020  ]) else 0 .     
+00000a00: 2020 2020 2020 2020 2066 6f72 2063 2069           for c i
+00000a10: 6e20 6361 6e64 6964 6174 6573 7d0a 2020  n candidates}.  
+00000a20: 2020 6d69 6e5f 7363 6f72 6520 3d20 6d69    min_score = mi
+00000a30: 6e28 7363 6f72 6573 2e76 616c 7565 7328  n(scores.values(
+00000a40: 2929 0a20 2020 2072 6574 7572 6e20 736f  )).    return so
+00000a50: 7274 6564 285b 6320 666f 7220 6320 696e  rted([c for c in
+00000a60: 2063 616e 6469 6461 7465 7320 6966 2073   candidates if s
+00000a70: 636f 7265 735b 635d 203d 3d20 6d69 6e5f  cores[c] == min_
+00000a80: 7363 6f72 655d 290a 0a0a 6465 6620 6d69  score])...def mi
+00000a90: 6e69 6d61 785f 7363 6f72 6573 2865 6461  nimax_scores(eda
+00000aa0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00000ab0: 204e 6f6e 652c 2073 636f 7265 5f6d 6574   None, score_met
+00000ac0: 686f 643d 226d 6172 6769 6e73 2229 3a0a  hod="margins"):.
+00000ad0: 2020 2020 2222 2252 6574 7572 6e20 7468      """Return th
+00000ae0: 6520 6d69 6e69 6d61 7820 7363 6f72 6573  e minimax scores
+00000af0: 2066 6f72 2065 6163 6820 6361 6e64 6964   for each candid
+00000b00: 6174 652c 2077 6865 7265 2074 6865 206d  ate, where the m
+00000b10: 696e 696d 6178 2073 636f 7265 2066 6f72  inimax score for
+00000b20: 203a 6d61 7468 3a60 6360 2069 7320 2d31   :math:`c` is -1
+00000b30: 202a 2074 6865 206d 6178 696d 756d 2070   * the maximum p
+00000b40: 6169 7277 6973 6520 6d61 6a6f 7269 7479  airwise majority
+00000b50: 206c 6f73 732e 200a 0a20 2020 2041 7267   loss. ..    Arg
+00000b60: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
+00000b70: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
+00000b80: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
+00000b90: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
+00000ba0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
+00000bb0: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
+00000bc0: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
+00000bd0: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
+00000be0: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
+00000bf0: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
+00000c00: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
+00000c10: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
+00000c20: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
+00000c30: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
+00000c40: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
+00000c50: 2020 2020 2020 2020 7363 6f72 655f 6d65          score_me
+00000c60: 7468 6f64 2028 7374 722c 206f 7074 696f  thod (str, optio
+00000c70: 6e61 6c29 3a20 4f70 7469 6f6e 7320 696e  nal): Options in
+00000c80: 636c 7564 6520 226d 6172 6769 6e73 2220  clude "margins" 
+00000c90: 2874 6865 2064 6566 6175 6c74 292c 2022  (the default), "
+00000ca0: 7769 6e6e 696e 6722 2061 7373 6967 6e73  winning" assigns
+00000cb0: 2074 6f20 6561 6368 2063 616e 6469 6461   to each candida
+00000cc0: 7465 203a 6d61 7468 3a60 6360 2074 6865  te :math:`c` the
+00000cd0: 206d 6178 696d 756d 2073 7570 706f 7274   maximum support
+00000ce0: 206f 6620 6120 6361 6e64 6964 6174 6520   of a candidate 
+00000cf0: 6d61 6a6f 7269 7479 2070 7265 6665 7272  majority preferr
+00000d00: 6564 2074 6f20 3a6d 6174 683a 6063 602c  ed to :math:`c`,
+00000d10: 2020 616e 6420 2270 6169 7277 6973 655f    and "pairwise_
+00000d20: 6f70 706f 7369 7469 6f6e 2220 6173 7369  opposition" assi
+00000d30: 676e 7320 746f 2065 6163 6820 6361 6e64  gns to each cand
+00000d40: 6964 6174 6520 3a6d 6174 683a 6063 6020  idate :math:`c` 
+00000d50: 7468 6520 6d61 7869 6d75 6d20 7375 7070  the maximum supp
+00000d60: 6f72 7420 6f66 2061 6e79 2063 616e 6469  ort of any candi
+00000d70: 6461 7465 206f 7665 7220 3a6d 6174 683a  date over :math:
+00000d80: 6063 602e 2020 2054 6865 7365 2073 636f  `c`.   These sco
+00000d90: 7265 7320 6f6e 6c79 206c 6561 6420 746f  res only lead to
+00000da0: 2064 6966 6665 7265 6e74 2072 6573 756c   different resul
+00000db0: 7473 206f 6e20 6e6f 6e2d 6c69 6e65 6172  ts on non-linear
+00000dc0: 2070 726f 6669 6c65 732e 200a 0a20 2020   profiles. ..   
+00000dd0: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
+00000de0: 2020 2041 2064 6963 7469 6f6e 6172 7920     A dictionary 
+00000df0: 6173 736f 6369 6174 696e 6720 6561 6368  associating each
+00000e00: 2063 616e 6469 6461 7465 2077 6974 6820   candidate with 
+00000e10: 6974 7320 6d69 6e69 6d61 7820 7363 6f72  its minimax scor
+00000e20: 652e 0a0a 2020 2020 2e2e 2073 6565 616c  e...    .. seeal
+00000e30: 736f 3a3a 0a0a 2020 2020 2020 2020 3a6d  so::..        :m
+00000e40: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+00000e50: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00000e60: 7468 6f64 732e 6d69 6e69 6d61 7860 0a0a  thods.minimax`..
+00000e70: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+00000e80: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+00000e90: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00000ea0: 6d70 6c65 732f 6d67 5f65 785f 6d69 6e69  mples/mg_ex_mini
+00000eb0: 6d61 782e 7079 0a20 2020 2020 2020 203a  max.py.        :
+00000ec0: 636f 6e74 6578 743a 2072 6573 6574 2020  context: reset  
+00000ed0: 0a20 2020 2020 2020 203a 696e 636c 7564  .        :includ
+00000ee0: 652d 736f 7572 6365 3a20 5472 7565 0a0a  e-source: True..
+00000ef0: 0a20 2020 202e 2e20 636f 6465 2d62 6c6f  .    .. code-blo
+00000f00: 636b 3a3a 200a 0a20 2020 2020 2020 2066  ck:: ..        f
+00000f10: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00000f20: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+00000f30: 686f 6473 2069 6d70 6f72 7420 6d69 6e69  hods import mini
+00000f40: 6d61 785f 7363 6f72 6573 2c20 6d69 6e69  max_scores, mini
+00000f50: 6d61 780a 0a20 2020 2020 2020 206d 696e  max..        min
+00000f60: 696d 6178 2e64 6973 706c 6179 2870 726f  imax.display(pro
+00000f70: 6629 0a20 2020 2020 2020 2070 7269 6e74  f).        print
+00000f80: 286d 696e 696d 6178 5f73 636f 7265 7328  (minimax_scores(
+00000f90: 7072 6f66 2929 0a0a 0a20 2020 202e 2e20  prof))...    .. 
+00000fa0: 6578 6563 5f63 6f64 653a 3a20 0a20 2020  exec_code:: .   
+00000fb0: 2020 2020 203a 6869 6465 5f63 6f64 653a       :hide_code:
+00000fc0: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
+00000fd0: 7265 665f 766f 7469 6e67 2e70 726f 6669  ref_voting.profi
+00000fe0: 6c65 7320 696d 706f 7274 2050 726f 6669  les import Profi
+00000ff0: 6c65 0a20 2020 2020 2020 2066 726f 6d20  le.        from 
+00001000: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+00001010: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+00001020: 2069 6d70 6f72 7420 6d69 6e69 6d61 782c   import minimax,
+00001030: 206d 696e 696d 6178 5f73 636f 7265 730a   minimax_scores.
+00001040: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001050: 2070 726f 6620 3d20 5072 6f66 696c 6528   prof = Profile(
+00001060: 5b5b 332c 2030 2c20 312c 2032 5d2c 205b  [[3, 0, 1, 2], [
+00001070: 312c 2033 2c20 322c 2030 5d2c 205b 312c  1, 3, 2, 0], [1,
+00001080: 2033 2c20 302c 2032 5d2c 205b 312c 2032   3, 0, 2], [1, 2
+00001090: 2c20 302c 2033 5d2c 205b 332c 2032 2c20  , 0, 3], [3, 2, 
+000010a0: 302c 2031 5d2c 205b 302c 2032 2c20 312c  0, 1], [0, 2, 1,
+000010b0: 2033 5d5d 2c20 5b31 2c20 312c 2031 2c20   3]], [1, 1, 1, 
+000010c0: 312c 2032 2c20 315d 290a 0a20 2020 2020  1, 2, 1])..     
+000010d0: 2020 206d 696e 696d 6178 2e64 6973 706c     minimax.displ
+000010e0: 6179 2870 726f 6629 0a20 2020 2020 2020  ay(prof).       
+000010f0: 2070 7269 6e74 286d 696e 696d 6178 5f73   print(minimax_s
+00001100: 636f 7265 7328 7072 6f66 2929 0a0a 2020  cores(prof))..  
+00001110: 2020 2222 220a 2020 2020 0a20 2020 2063    """.    .    c
+00001120: 616e 6469 6461 7465 7320 3d20 6564 6174  andidates = edat
+00001130: 612e 6361 6e64 6964 6174 6573 2069 6620  a.candidates if 
+00001140: 6375 7272 5f63 616e 6473 2069 7320 4e6f  curr_cands is No
+00001150: 6e65 2065 6c73 6520 6375 7272 5f63 616e  ne else curr_can
+00001160: 6473 0a0a 2020 2020 6966 206c 656e 2863  ds..    if len(c
+00001170: 616e 6469 6461 7465 7329 203d 3d20 313a  andidates) == 1:
+00001180: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00001190: 7b63 3a20 3020 666f 7220 6320 696e 2063  {c: 0 for c in c
+000011a0: 616e 6469 6461 7465 737d 0a20 2020 200a  andidates}.    .
+000011b0: 2020 2020 2320 7468 6572 6520 6172 6520      # there are 
+000011c0: 6469 6666 6572 656e 7420 7363 6f72 696e  different scorin
+000011d0: 6720 6675 6e63 7469 6f6e 7320 7468 6174  g functions that
+000011e0: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
+000011f0: 6d65 6173 7572 6520 7468 6520 776f 7273  measure the wors
+00001200: 6520 6c6f 7373 2066 6f72 2065 6163 6820  e loss for each 
+00001210: 0a20 2020 2023 2063 616e 6469 6461 7465  .    # candidate
+00001220: 2e20 5468 6573 6520 616c 6c20 7072 6f64  . These all prod
+00001230: 7563 6520 7468 6520 7361 6d65 2073 6574  uce the same set
+00001240: 206f 6620 7769 6e6e 6572 7320 7768 656e   of winners when
+00001250: 2076 6f74 6572 7320 7375 626d 6974 206c   voters submit l
+00001260: 696e 6561 7220 6f72 6465 7273 2e20 0a20  inear orders. . 
+00001270: 2020 2073 636f 7265 5f66 756e 6374 696f     score_functio
+00001280: 6e73 203d 207b 0a20 2020 2020 2020 2022  ns = {.        "
+00001290: 7769 6e6e 696e 6722 3a20 6c61 6d62 6461  winning": lambda
+000012a0: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
+000012b0: 7461 2e73 7570 706f 7274 285f 632c 6329  ta.support(_c,c)
+000012c0: 2066 6f72 205f 6320 696e 2063 735d 2920   for _c in cs]) 
+000012d0: 6966 206c 656e 2863 7329 203e 2030 2065  if len(cs) > 0 e
+000012e0: 6c73 6520 302c 0a20 2020 2020 2020 2022  lse 0,.        "
+000012f0: 6d61 7267 696e 7322 3a20 6c61 6d62 6461  margins": lambda
+00001300: 2063 732c 2063 3a20 6d61 7828 5b65 6461   cs, c: max([eda
+00001310: 7461 2e6d 6172 6769 6e28 5f63 2c63 2920  ta.margin(_c,c) 
+00001320: 666f 7220 5f63 2069 6e20 6373 5d29 2069  for _c in cs]) i
+00001330: 6620 6c65 6e28 6373 2920 3e20 3020 656c  f len(cs) > 0 el
+00001340: 7365 2030 2c0a 2020 2020 2020 2020 2270  se 0,.        "p
+00001350: 6169 7277 6973 655f 6f70 706f 7369 7469  airwise_oppositi
+00001360: 6f6e 223a 206c 616d 6264 6120 6373 2c20  on": lambda cs, 
+00001370: 633a 206d 6178 285b 6564 6174 612e 7375  c: max([edata.su
+00001380: 7070 6f72 7428 5f63 2c63 2920 666f 7220  pport(_c,c) for 
+00001390: 5f63 2069 6e20 6373 5d29 0a20 2020 207d  _c in cs]).    }
+000013a0: 200a 2020 2020 0a20 2020 2063 616e 6473   .    .    cands
+000013b0: 203d 207b 0a20 2020 2020 2020 2022 7769   = {.        "wi
+000013c0: 6e6e 696e 6722 3a20 6c61 6d62 6461 2063  nning": lambda c
+000013d0: 3a20 6564 6174 612e 646f 6d69 6e61 746f  : edata.dominato
+000013e0: 7273 2863 2c20 6375 7272 5f63 616e 6473  rs(c, curr_cands
+000013f0: 203d 2063 7572 725f 6361 6e64 7329 2c0a   = curr_cands),.
+00001400: 2020 2020 2020 2020 226d 6172 6769 6e73          "margins
+00001410: 223a 206c 616d 6264 6120 633a 2065 6461  ": lambda c: eda
+00001420: 7461 2e64 6f6d 696e 6174 6f72 7328 632c  ta.dominators(c,
+00001430: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+00001440: 7272 5f63 616e 6473 292c 0a20 2020 2020  rr_cands),.     
+00001450: 2020 2022 7061 6972 7769 7365 5f6f 7070     "pairwise_opp
+00001460: 6f73 6974 696f 6e22 3a20 6c61 6d62 6461  osition": lambda
+00001470: 2063 3a20 5b5f 6320 666f 7220 5f63 2069   c: [_c for _c i
+00001480: 6e20 6361 6e64 6964 6174 6573 2069 6620  n candidates if 
+00001490: 5f63 2021 3d20 635d 0a20 2020 207d 200a  _c != c].    } .
+000014a0: 0a20 2020 2072 6574 7572 6e20 7b63 3a20  .    return {c: 
+000014b0: 2d31 202a 2073 636f 7265 5f66 756e 6374  -1 * score_funct
+000014c0: 696f 6e73 5b73 636f 7265 5f6d 6574 686f  ions[score_metho
+000014d0: 645d 2863 616e 6473 5b73 636f 7265 5f6d  d](cands[score_m
+000014e0: 6574 686f 645d 2863 292c 2063 2920 666f  ethod](c), c) fo
+000014f0: 7220 6320 696e 2063 616e 6469 6461 7465  r c in candidate
+00001500: 737d 0a0a 0a64 6566 206d 6178 696d 616c  s}...def maximal
+00001510: 5f65 6c65 6d65 6e74 7328 6729 3a20 0a20  _elements(g): . 
+00001520: 2020 2022 2222 7265 7475 726e 2074 6865     """return the
+00001530: 206e 6f64 6573 2069 6e20 6720 7769 7468   nodes in g with
+00001540: 206e 6f20 696e 636f 6d69 6e67 2061 7272   no incoming arr
+00001550: 6f77 732e 2222 220a 2020 2020 7265 7475  ows.""".    retu
+00001560: 726e 205b 6e20 666f 7220 6e20 696e 2067  rn [n for n in g
+00001570: 2e6e 6f64 6573 2069 6620 672e 696e 5f64  .nodes if g.in_d
+00001580: 6567 7265 6528 6e29 203d 3d20 305d 0a0a  egree(n) == 0]..
+00001590: 0a64 6566 205f 6265 6174 5f70 6174 685f  .def _beat_path_
+000015a0: 6261 7369 6328 6564 6174 612c 200a 2020  basic(edata, .  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
+000015d0: 4e6f 6e65 2c20 0a20 2020 2020 2020 2020  None, .         
+000015e0: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+000015f0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00001600: 4e6f 6e65 293a 200a 2020 2020 2222 2241  None): .    """A
+00001610: 6e20 696d 706c 656d 656e 7461 7469 6f6e  n implementation
+00001620: 206f 6620 7468 6520 4265 6174 2050 6174   of the Beat Pat
+00001630: 6820 6d65 7468 6f64 2074 6861 7420 7573  h method that us
+00001640: 6573 2061 2062 6173 6963 2061 6c67 6f72  es a basic algor
+00001650: 6974 686d 2e20 2054 6869 7320 6973 206e  ithm.  This is n
+00001660: 6f74 2065 6666 6963 6965 6e74 2066 6f72  ot efficient for
+00001670: 206c 6172 6765 2067 7261 7068 732e 0a20   large graphs.. 
+00001680: 2020 200a 2020 2020 4172 6773 3a0a 2020     .    Args:.  
+00001690: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+000016a0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+000016b0: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+000016c0: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+000016d0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+000016e0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+000016f0: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+00001700: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+00001710: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+00001720: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+00001730: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+00001740: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+00001750: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+00001760: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+00001770: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+00001780: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00001790: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+000017a0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+000017b0: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+000017c0: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+000017d0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+000017e0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+000017f0: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+00001800: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+00001810: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+00001820: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+00001830: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+00001840: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+00001850: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
+00001860: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+00001870: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+00001880: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+00001890: 732e 200a 0a20 2020 2022 2222 0a20 2020  s. ..    """.   
+000018a0: 2063 616e 6469 6461 7465 7320 3d20 6564   candidates = ed
+000018b0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+000018c0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+000018d0: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+000018e0: 616e 6473 2020 2020 0a20 2020 2073 7472  ands    .    str
+000018f0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00001900: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+00001910: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00001920: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00001930: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00001940: 6e0a 2020 2020 0a20 2020 206d 6720 3d20  n.    .    mg = 
+00001950: 6765 745f 6d67 2865 6461 7461 2c20 6375  get_mg(edata, cu
+00001960: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+00001970: 6361 6e64 7329 0a20 2020 200a 2020 2020  cands).    .    
+00001980: 6265 6174 5f70 6174 6873 5f77 6569 6768  beat_paths_weigh
+00001990: 7473 203d 207b 633a 207b 6332 3a30 2066  ts = {c: {c2:0 f
+000019a0: 6f72 2063 3220 696e 2063 616e 6469 6461  or c2 in candida
+000019b0: 7465 7320 6966 2063 3220 213d 2063 7d20  tes if c2 != c} 
+000019c0: 666f 7220 6320 696e 2063 616e 6469 6461  for c in candida
+000019d0: 7465 737d 0a20 2020 2066 6f72 2063 2069  tes}.    for c i
+000019e0: 6e20 6361 6e64 6964 6174 6573 3a20 0a20  n candidates: . 
+000019f0: 2020 2020 2020 2066 6f72 206f 7468 6572         for other
+00001a00: 5f63 2069 6e20 6265 6174 5f70 6174 6873  _c in beat_paths
+00001a10: 5f77 6569 6768 7473 5b63 5d2e 6b65 7973  _weights[c].keys
+00001a20: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00001a30: 616c 6c5f 7061 7468 7320 3d20 206c 6973  all_paths =  lis
+00001a40: 7428 6e78 2e61 6c6c 5f73 696d 706c 655f  t(nx.all_simple_
+00001a50: 7061 7468 7328 6d67 2c20 632c 206f 7468  paths(mg, c, oth
+00001a60: 6572 5f63 2929 0a20 2020 2020 2020 2020  er_c)).         
+00001a70: 2020 2069 6620 6c65 6e28 616c 6c5f 7061     if len(all_pa
+00001a80: 7468 7329 203e 2030 3a0a 2020 2020 2020  ths) > 0:.      
+00001a90: 2020 2020 2020 2020 2020 6265 6174 5f70            beat_p
+00001aa0: 6174 6873 5f77 6569 6768 7473 5b63 5d5b  aths_weights[c][
+00001ab0: 6f74 6865 725f 635d 203d 206d 6178 285b  other_c] = max([
+00001ac0: 6d69 6e28 5b73 7472 656e 6774 685f 6675  min([strength_fu
+00001ad0: 6e63 7469 6f6e 2870 5b69 5d2c 2070 5b69  nction(p[i], p[i
+00001ae0: 2b31 5d29 200a 2020 2020 2020 2020 2020  +1]) .          
+00001af0: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+00001b00: 616e 6765 2830 2c6c 656e 2870 292d 3129  ange(0,len(p)-1)
+00001b10: 5d29 200a 2020 2020 2020 2020 2020 2020  ]) .            
+00001b20: 2020 2020 666f 7220 7020 696e 2061 6c6c      for p in all
+00001b30: 5f70 6174 6873 5d29 0a20 2020 200a 2020  _paths]).    .  
+00001b40: 2020 7769 6e6e 6572 7320 3d20 6c69 7374    winners = list
+00001b50: 2829 0a20 2020 2066 6f72 2063 2069 6e20  ().    for c in 
+00001b60: 6361 6e64 6964 6174 6573 3a20 0a20 2020  candidates: .   
+00001b70: 2020 2020 2069 6620 616c 6c28 5b62 6561       if all([bea
+00001b80: 745f 7061 7468 735f 7765 6967 6874 735b  t_paths_weights[
+00001b90: 635d 5b63 325d 203e 3d20 6265 6174 5f70  c][c2] >= beat_p
+00001ba0: 6174 6873 5f77 6569 6768 7473 5b63 325d  aths_weights[c2]
+00001bb0: 5b63 5d20 666f 7220 6332 2069 6e20 6361  [c] for c2 in ca
+00001bc0: 6e64 6964 6174 6573 2020 6966 2063 3220  ndidates  if c2 
+00001bd0: 213d 2063 5d29 3a0a 2020 2020 2020 2020  != c]):.        
+00001be0: 2020 2020 7769 6e6e 6572 732e 6170 7065      winners.appe
+00001bf0: 6e64 2863 290a 2020 2020 7265 7475 726e  nd(c).    return
+00001c00: 2073 6f72 7465 6428 6c69 7374 2877 696e   sorted(list(win
+00001c10: 6e65 7273 2929 0a0a 6465 6620 5f62 6561  ners))..def _bea
+00001c20: 745f 7061 7468 5f66 6c6f 7964 5f77 6172  t_path_floyd_war
+00001c30: 7368 616c 6c28 0a20 2020 2020 2020 2065  shall(.        e
+00001c40: 6461 7461 2c20 0a20 2020 2020 2020 2063  data, .        c
+00001c50: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+00001c60: 2c20 0a20 2020 2020 2020 2073 7472 656e  , .        stren
+00001c70: 6774 685f 6675 6e63 7469 6f6e 203d 204e  gth_function = N
+00001c80: 6f6e 6529 3a20 2020 0a20 2020 2022 2222  one):   .    """
+00001c90: 416e 2069 6d70 6c65 6d65 6e74 6174 696f  An implementatio
+00001ca0: 6e20 6f66 2042 6561 7420 5061 7468 2075  n of Beat Path u
+00001cb0: 7369 6e67 2061 2076 6172 6961 7469 6f6e  sing a variation
+00001cc0: 206f 6620 7468 6520 466c 6f79 642d 5761   of the Floyd-Wa
+00001cd0: 7273 6861 6c6c 2041 6c67 6f72 6974 686d  rshall Algorithm
+00001ce0: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+00001cf0: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00001d00: 672f 7769 6b69 2f53 6368 756c 7a65 5f6d  g/wiki/Schulze_m
+00001d10: 6574 686f 6423 496d 706c 656d 656e 7461  ethod#Implementa
+00001d20: 7469 6f6e 290a 200a 2020 2020 4172 6773  tion). .    Args
+00001d30: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00001d40: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00001d50: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00001d60: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00001d70: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00001d80: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+00001d90: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+00001da0: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+00001db0: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+00001dc0: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+00001dd0: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+00001de0: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+00001df0: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+00001e00: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+00001e10: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+00001e20: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+00001e30: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+00001e40: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+00001e50: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+00001e60: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+00001e70: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+00001e80: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+00001e90: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+00001ea0: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+00001eb0: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+00001ec0: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+00001ed0: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+00001ee0: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+00001ef0: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+00001f00: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
+00001f10: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+00001f20: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+00001f30: 6461 7465 732e 200a 0a20 2020 2022 2222  dates. ..    """
+00001f40: 0a0a 2020 2020 6361 6e64 6964 6174 6573  ..    candidates
+00001f50: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
+00001f60: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
+00001f70: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
+00001f80: 7572 725f 6361 6e64 7320 2020 200a 2020  urr_cands    .  
+00001f90: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00001fa0: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
+00001fb0: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
+00001fc0: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
+00001fd0: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
+00001fe0: 6e63 7469 6f6e 0a20 2020 2020 2020 200a  nction.        .
+00001ff0: 2020 2020 735f 6d61 7472 6978 203d 205b      s_matrix = [
+00002000: 5b2d 6e70 2e69 6e66 2066 6f72 205f 2069  [-np.inf for _ i
+00002010: 6e20 6361 6e64 6964 6174 6573 5d20 666f  n candidates] fo
+00002020: 7220 5f20 696e 2063 616e 6469 6461 7465  r _ in candidate
+00002030: 735d 0a20 2020 2066 6f72 2063 315f 6964  s].    for c1_id
+00002040: 782c 2063 3120 696e 2065 6e75 6d65 7261  x, c1 in enumera
+00002050: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+00002060: 2020 2020 2020 2020 666f 7220 6332 5f69          for c2_i
+00002070: 6478 2c20 6332 2069 6e20 656e 756d 6572  dx, c2 in enumer
+00002080: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00002090: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000020a0: 2865 6461 7461 2e6d 616a 6f72 6974 795f  (edata.majority_
+000020b0: 7072 6566 6572 7328 6331 2c20 6332 2920  prefers(c1, c2) 
+000020c0: 6f72 2063 3120 3d3d 2063 3229 3a0a 2020  or c1 == c2):.  
+000020d0: 2020 2020 2020 2020 2020 2020 2020 735f                s_
+000020e0: 6d61 7472 6978 5b63 315f 6964 785d 5b63  matrix[c1_idx][c
+000020f0: 325f 6964 785d 203d 2073 7472 656e 6774  2_idx] = strengt
+00002100: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
+00002110: 3229 200a 2020 2020 7374 7265 6e67 7468  2) .    strength
+00002120: 203d 206c 6973 7428 6d61 7028 6c61 6d62   = list(map(lamb
+00002130: 6461 2069 203a 206c 6973 7428 6d61 7028  da i : list(map(
+00002140: 6c61 6d62 6461 206a 203a 206a 202c 2069  lambda j : j , i
+00002150: 2929 202c 2073 5f6d 6174 7269 7829 290a  )) , s_matrix)).
+00002160: 2020 2020 666f 7220 695f 6964 782c 2069      for i_idx, i
+00002170: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00002180: 6e64 6964 6174 6573 293a 2020 2020 2020  ndidates):      
+00002190: 2020 200a 2020 2020 2020 2020 666f 7220     .        for 
+000021a0: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
+000021b0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+000021c0: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
+000021d0: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
+000021e0: 2020 2020 2020 2020 2020 666f 7220 6b5f            for k_
+000021f0: 6964 782c 206b 2069 6e20 656e 756d 6572  idx, k in enumer
+00002200: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00002210: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00002220: 2020 2020 2020 6966 2069 213d 206b 2061        if i!= k a
+00002230: 6e64 206a 2021 3d20 6b3a 0a20 2020 2020  nd j != k:.     
+00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002250: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
+00002260: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
+00002270: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
+00002280: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
+00002290: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
+000022a0: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
+000022b0: 785d 5b6b 5f69 6478 5d29 290a 2020 2020  x][k_idx])).    
+000022c0: 7769 6e6e 6572 7320 3d20 7b69 3a54 7275  winners = {i:Tru
+000022d0: 6520 666f 7220 6920 696e 2063 616e 6469  e for i in candi
+000022e0: 6461 7465 737d 0a20 2020 2066 6f72 2069  dates}.    for i
+000022f0: 5f69 6478 2c20 6920 696e 2065 6e75 6d65  _idx, i in enume
+00002300: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00002310: 3a20 0a20 2020 2020 2020 2066 6f72 206a  : .        for j
+00002320: 5f69 6478 2c20 6a20 696e 2065 6e75 6d65  _idx, j in enume
+00002330: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00002340: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00002350: 2069 213d 6a3a 0a20 2020 2020 2020 2020   i!=j:.         
+00002360: 2020 2020 2020 2069 6620 7374 7265 6e67         if streng
+00002370: 7468 5b6a 5f69 6478 5d5b 695f 6964 785d  th[j_idx][i_idx]
+00002380: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
+00002390: 785d 5b6a 5f69 6478 5d3a 0a20 2020 2020  x][j_idx]:.     
+000023a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000023b0: 696e 6e65 7273 5b69 5d20 3d20 4661 6c73  inners[i] = Fals
+000023c0: 650a 2020 2020 7265 7475 726e 2073 6f72  e.    return sor
+000023d0: 7465 6428 5b63 2066 6f72 2063 2069 6e20  ted([c for c in 
+000023e0: 6361 6e64 6964 6174 6573 2069 6620 7769  candidates if wi
+000023f0: 6e6e 6572 735b 635d 5d29 0a0a 6465 6620  nners[c]])..def 
+00002400: 5f73 6368 7761 7274 7a5f 7365 7175 656e  _schwartz_sequen
+00002410: 7469 616c 5f64 726f 7070 696e 6728 6564  tial_dropping(ed
+00002420: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
+00002430: 3d20 4e6f 6e65 2c20 7374 7265 6e67 7468  = None, strength
+00002440: 5f66 756e 6374 696f 6e20 3d20 4e6f 6e65  _function = None
+00002450: 293a 0a0a 2020 2020 2222 2254 6865 2053  ):..    """The S
+00002460: 6368 7761 7274 7a20 5365 7175 656e 7469  chwartz Sequenti
+00002470: 616c 2044 726f 7070 696e 6720 616c 676f  al Dropping algo
+00002480: 7269 7468 6d2e 2053 6565 2068 7474 7073  rithm. See https
+00002490: 3a2f 2f65 6e2e 7769 6b69 7065 6469 612e  ://en.wikipedia.
+000024a0: 6f72 672f 7769 6b69 2f53 6368 756c 7a65  org/wiki/Schulze
+000024b0: 5f6d 6574 686f 6423 5469 6573 5f61 6e64  _method#Ties_and
+000024c0: 5f61 6c74 6572 6e61 7469 7665 5f69 6d70  _alternative_imp
+000024d0: 6c65 6d65 6e74 6174 696f 6e73 2e0a 2020  lementations..  
+000024e0: 2020 0a20 2020 2041 7267 733a 0a20 2020    .    Args:.   
+000024f0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00002500: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00002510: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00002520: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00002530: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00002540: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00002550: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00002560: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00002570: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00002580: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00002590: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+000025a0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+000025b0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+000025c0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+000025d0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+000025e0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+000025f0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00002600: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00002610: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00002620: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00002630: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00002640: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00002650: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00002660: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00002670: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00002680: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00002690: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+000026a0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+000026b0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+000026c0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+000026d0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+000026e0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+000026f0: 2e20 0a20 2020 2022 2222 0a20 2020 2066  . .    """.    f
+00002700: 726f 6d20 7072 6566 5f76 6f74 696e 672e  rom pref_voting.
+00002710: 6331 5f6d 6574 686f 6473 2069 6d70 6f72  c1_methods impor
+00002720: 7420 676f 6368 610a 0a20 2020 2073 7472  t gocha..    str
+00002730: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00002740: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+00002750: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00002760: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00002770: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00002780: 6e0a 0a20 2020 206d 6720 3d20 6564 6174  n..    mg = edat
+00002790: 6120 6966 2069 7369 6e73 7461 6e63 6528  a if isinstance(
+000027a0: 6564 6174 612c 204d 6172 6769 6e47 7261  edata, MarginGra
+000027b0: 7068 2920 656c 7365 2065 6461 7461 2e6d  ph) else edata.m
+000027c0: 6172 6769 6e5f 6772 6170 6828 290a 2020  argin_graph().  
+000027d0: 2020 7363 6877 6172 747a 203d 2067 6f63    schwartz = goc
+000027e0: 6861 286d 672c 2063 7572 725f 6361 6e64  ha(mg, curr_cand
+000027f0: 7320 3d20 6375 7272 5f63 616e 6473 290a  s = curr_cands).
+00002800: 0a20 2020 2069 6620 6c65 6e28 7363 6877  .    if len(schw
+00002810: 6172 747a 2920 3d3d 2031 3a0a 2020 2020  artz) == 1:.    
+00002820: 2020 2020 7265 7475 726e 2073 6368 7761      return schwa
+00002830: 7274 7a0a 2020 2020 0a20 2020 2070 6f73  rtz.    .    pos
+00002840: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+00002850: 7468 7320 3d20 5b73 7472 656e 6774 685f  ths = [strength_
+00002860: 6675 6e63 7469 6f6e 2863 2c64 2920 666f  function(c,d) fo
+00002870: 7220 6320 696e 2073 6368 7761 7274 7a20  r c in schwartz 
+00002880: 666f 7220 6420 696e 2073 6368 7761 7274  for d in schwart
+00002890: 7a20 6966 2073 7472 656e 6774 685f 6675  z if strength_fu
+000028a0: 6e63 7469 6f6e 2863 2c64 2920 3e20 305d  nction(c,d) > 0]
+000028b0: 0a0a 2020 2020 6966 206c 656e 2870 6f73  ..    if len(pos
+000028c0: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+000028d0: 7468 7329 203d 3d20 303a 0a20 2020 2020  ths) == 0:.     
+000028e0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+000028f0: 2873 6368 7761 7274 7a29 0a0a 2020 2020  (schwartz)..    
+00002900: 6d61 785f 7363 6877 6172 747a 5f73 7472  max_schwartz_str
+00002910: 656e 6774 6820 3d20 6d61 7828 706f 735f  ength = max(pos_
+00002920: 7363 6877 6172 747a 5f73 7472 656e 6774  schwartz_strengt
+00002930: 6873 290a 2020 2020 6d69 6e5f 7363 6877  hs).    min_schw
+00002940: 6172 747a 5f73 7472 656e 6774 6820 3d20  artz_strength = 
+00002950: 6d69 6e28 706f 735f 7363 6877 6172 747a  min(pos_schwartz
+00002960: 5f73 7472 656e 6774 6873 290a 0a20 2020  _strengths)..   
+00002970: 2069 6620 6d61 785f 7363 6877 6172 747a   if max_schwartz
+00002980: 5f73 7472 656e 6774 6820 3d3d 206d 696e  _strength == min
+00002990: 5f73 6368 7761 7274 7a5f 7374 7265 6e67  _schwartz_streng
+000029a0: 7468 3a0a 2020 2020 2020 2020 7265 7475  th:.        retu
+000029b0: 726e 2073 6f72 7465 6428 7363 6877 6172  rn sorted(schwar
+000029c0: 747a 290a 2020 2020 0a20 2020 2065 6c73  tz).    .    els
+000029d0: 653a 0a20 2020 2020 2020 206e 6577 5f6d  e:.        new_m
+000029e0: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+000029f0: 7363 6877 6172 747a 2c5b 2863 2c64 2c20  schwartz,[(c,d, 
+00002a00: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00002a10: 6e28 632c 6429 2920 666f 7220 6320 696e  n(c,d)) for c in
+00002a20: 2073 6368 7761 7274 7a20 666f 7220 6420   schwartz for d 
+00002a30: 696e 2073 6368 7761 7274 7a20 6966 2073  in schwartz if s
+00002a40: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00002a50: 2863 2c64 2920 3e20 6d69 6e5f 7363 6877  (c,d) > min_schw
+00002a60: 6172 747a 5f73 7472 656e 6774 685d 290a  artz_strength]).
+00002a70: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00002a80: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
+00002a90: 6961 6c5f 6472 6f70 7069 6e67 286e 6577  ial_dropping(new
+00002aa0: 5f6d 672c 2073 6368 7761 7274 7a29 0a0a  _mg, schwartz)..
+00002ab0: 4076 6d28 6e61 6d65 3d22 4265 6174 2050  @vm(name="Beat P
+00002ac0: 6174 6822 2c0a 2020 2020 696e 7075 745f  ath",.    input_
+00002ad0: 7479 7065 733d 5b45 6c65 6374 696f 6e54  types=[ElectionT
+00002ae0: 7970 6573 2e50 524f 4649 4c45 2c20 456c  ypes.PROFILE, El
+00002af0: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
+00002b00: 494c 455f 5749 5448 5f54 4945 532c 2045  ILE_WITH_TIES, E
+00002b10: 6c65 6374 696f 6e54 7970 6573 2e4d 4152  lectionTypes.MAR
+00002b20: 4749 4e5f 4752 4150 485d 290a 6465 6620  GIN_GRAPH]).def 
+00002b30: 6265 6174 5f70 6174 6828 0a20 2020 2065  beat_path(.    e
+00002b40: 6461 7461 2c20 0a20 2020 2063 7572 725f  data, .    curr_
+00002b50: 6361 6e64 7320 3d20 4e6f 6e65 2c20 0a20  cands = None, . 
+00002b60: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+00002b70: 7469 6f6e 203d 204e 6f6e 652c 200a 2020  tion = None, .  
+00002b80: 2020 616c 676f 7269 7468 6d20 3d20 2766    algorithm = 'f
+00002b90: 6c6f 7964 5f77 6172 7368 616c 6c27 293a  loyd_warshall'):
+00002ba0: 2020 0a0a 2020 2020 2222 2246 6f72 2063    ..    """For c
+00002bb0: 616e 6469 6461 7465 7320 3a6d 6174 683a  andidates :math:
+00002bc0: 6061 6020 616e 6420 3a6d 6174 683a 6062  `a` and :math:`b
+00002bd0: 602c 2061 202a 2a70 6174 682a 2a20 6672  `, a **path** fr
+00002be0: 6f6d 203a 6d61 7468 3a60 6160 2074 6f20  om :math:`a` to 
+00002bf0: 3a6d 6174 683a 6062 6020 6973 2061 2073  :math:`b` is a s
+00002c00: 6571 7565 6e63 6520 0a20 2020 203a 6d61  equence .    :ma
+00002c10: 7468 3a60 785f 312c 205c 6c64 6f74 732c  th:`x_1, \ldots,
+00002c20: 2078 5f6e 6020 6f66 2064 6973 7469 6e63   x_n` of distinc
+00002c30: 7420 6361 6e64 6964 6174 6573 2020 7769  t candidates  wi
+00002c40: 7468 2020 3a6d 6174 683a 6078 5f31 3d61  th  :math:`x_1=a
+00002c50: 6020 616e 6420 3a6d 6174 683a 6078 5f6e  ` and :math:`x_n
+00002c60: 3d62 6020 7375 6368 2074 6861 7420 0a20  =b` such that . 
+00002c70: 2020 2066 6f72 203a 6d61 7468 3a60 315c     for :math:`1\
+00002c80: 6c65 7120 6b5c 6c65 7120 6e2d 3160 2c20  leq k\leq n-1`, 
+00002c90: 3a6d 6174 683a 6078 5f6b 6020 6973 206d  :math:`x_k` is m
+00002ca0: 616a 6f72 6974 7920 7072 6566 6572 7265  ajority preferre
+00002cb0: 6420 746f 203a 6d61 7468 3a60 785f 7b6b  d to :math:`x_{k
+00002cc0: 2b31 7d60 2e20 2054 6865 202a 2a73 7472  +1}`.  The **str
+00002cd0: 656e 6774 6820 6f66 2061 2070 6174 682a  ength of a path*
+00002ce0: 2a0a 2020 2020 6973 2074 6865 206d 696e  *.    is the min
+00002cf0: 696d 616c 206d 6172 6769 6e20 616c 6f6e  imal margin alon
+00002d00: 6720 7468 6174 2070 6174 682e 2020 5361  g that path.  Sa
+00002d10: 7920 7468 6174 203a 6d61 7468 3a60 6160  y that :math:`a`
+00002d20: 2064 6566 6561 7473 203a 6d61 7468 3a60   defeats :math:`
+00002d30: 6260 2061 6363 6f72 6469 6e67 2074 6f20  b` according to 
+00002d40: 4265 6174 2050 6174 6820 6966 2074 6865  Beat Path if the
+00002d50: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+00002d60: 2074 6865 2073 7472 6f6e 6765 7374 2070   the strongest p
+00002d70: 6174 6820 6672 6f6d 203a 6d61 7468 3a60  ath from :math:`
+00002d80: 6160 2074 6f20 3a6d 6174 683a 6062 6020  a` to :math:`b` 
+00002d90: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+00002da0: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
+00002db0: 7468 6520 7374 726f 6e67 6573 7420 7061  the strongest pa
+00002dc0: 7468 2066 726f 6d20 3a6d 6174 683a 6062  th from :math:`b
+00002dd0: 6020 746f 203a 6d61 7468 3a60 6160 2e20  ` to :math:`a`. 
+00002de0: 5468 656e 2074 6865 2063 616e 6469 6461  Then the candida
+00002df0: 7465 7320 7468 6174 2061 7265 2075 6e64  tes that are und
+00002e00: 6566 6561 7465 6420 6163 636f 7264 696e  efeated accordin
+00002e10: 6720 746f 2042 6561 7420 5061 7468 2061  g to Beat Path a
+00002e20: 7265 2074 6865 2077 696e 6e65 7273 2e20  re the winners. 
+00002e30: 2041 6c73 6f20 6b6e 6f77 6e20 6173 2074   Also known as t
+00002e40: 6865 2053 6368 756c 7a65 2052 756c 652e  he Schulze Rule.
+00002e50: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
+00002e60: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
+00002e70: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
+00002e80: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
+00002e90: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
+00002ea0: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
+00002eb0: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
+00002ec0: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
+00002ed0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+00002ee0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00002ef0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+00002f00: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+00002f10: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+00002f20: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00002f30: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00002f40: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
+00002f50: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+00002f60: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+00002f70: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+00002f80: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+00002f90: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+00002fa0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+00002fb0: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+00002fc0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+00002fd0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+00002fe0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+00002ff0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+00003000: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+00003010: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+00003020: 6e65 6172 206f 7264 6572 732e 200a 2020  near orders. .  
+00003030: 2020 2020 2020 616c 676f 7269 7468 6d20        algorithm 
+00003040: 2873 7472 293a 2053 7065 6369 6679 2077  (str): Specify w
+00003050: 6869 6368 2061 6c67 6f72 6974 686d 2074  hich algorithm t
+00003060: 6f20 7573 652e 2020 4f70 7469 6f6e 7320  o use.  Options 
+00003070: 6172 6520 2766 6c6f 7964 5f77 6172 7368  are 'floyd_warsh
+00003080: 616c 6c27 2028 7468 6520 6465 6661 756c  all' (the defaul
+00003090: 7429 2c20 2762 6173 6963 272c 2061 6e64  t), 'basic', and
+000030a0: 2027 7363 6877 6172 747a 5f73 6571 7565   'schwartz_seque
+000030b0: 6e74 6961 6c5f 6472 6f70 7069 6e67 272e  ntial_dropping'.
+000030c0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+000030d0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+000030e0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+000030f0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
+00003100: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
+00003110: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+00003120: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+00003130: 5f6d 6574 686f 6473 2e62 6561 745f 7061  _methods.beat_pa
+00003140: 7468 5f64 6566 6561 7460 0a0a 2020 2020  th_defeat`..    
+00003150: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+00003160: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+00003170: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+00003180: 732f 6d67 5f65 785f 6270 5f72 702e 7079  s/mg_ex_bp_rp.py
+00003190: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+000031a0: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+000031b0: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+000031c0: 6365 3a20 5472 7565 0a0a 0a20 2020 202e  ce: True...    .
+000031d0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 200a  . code-block:: .
+000031e0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+000031f0: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00003200: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+00003210: 6d70 6f72 7420 6265 6174 5f70 6174 680a  mport beat_path.
+00003220: 0a20 2020 2020 2020 2062 6561 745f 7061  .        beat_pa
+00003230: 7468 2e64 6973 706c 6179 286d 6729 0a0a  th.display(mg)..
+00003240: 0a20 2020 202e 2e20 6578 6563 5f63 6f64  .    .. exec_cod
+00003250: 653a 3a20 0a20 2020 2020 2020 203a 6869  e:: .        :hi
+00003260: 6465 5f63 6f64 653a 0a0a 2020 2020 2020  de_code:..      
+00003270: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+00003280: 6e67 2e77 6569 6768 7465 645f 6d61 6a6f  ng.weighted_majo
+00003290: 7269 7479 5f67 7261 7068 7320 696d 706f  rity_graphs impo
+000032a0: 7274 204d 6172 6769 6e47 7261 7068 0a20  rt MarginGraph. 
+000032b0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+000032c0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+000032d0: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+000032e0: 6f72 7420 6265 6174 5f70 6174 680a 2020  ort beat_path.  
+000032f0: 2020 2020 2020 0a20 2020 2020 2020 206d        .        m
+00003300: 6720 3d20 4d61 7267 696e 4772 6170 6828  g = MarginGraph(
+00003310: 5b30 2c20 312c 2032 2c20 335d 2c20 5b28  [0, 1, 2, 3], [(
+00003320: 302c 2032 2c20 3329 2c20 2831 2c20 302c  0, 2, 3), (1, 0,
+00003330: 2035 292c 2028 322c 2031 2c20 3529 2c20   5), (2, 1, 5), 
+00003340: 2832 2c20 332c 2031 292c 2028 332c 2030  (2, 3, 1), (3, 0
+00003350: 2c20 3329 2c20 2833 2c20 312c 2031 295d  , 3), (3, 1, 1)]
+00003360: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00003370: 2020 2062 6561 745f 7061 7468 2e64 6973     beat_path.dis
+00003380: 706c 6179 286d 6729 0a20 2020 2020 2020  play(mg).       
+00003390: 2062 6561 745f 7061 7468 2e64 6973 706c   beat_path.displ
+000033a0: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
+000033b0: 3d27 666c 6f79 645f 7761 7273 6861 6c6c  ='floyd_warshall
+000033c0: 2729 200a 2020 2020 2020 2020 6265 6174  ') .        beat
+000033d0: 5f70 6174 682e 6469 7370 6c61 7928 6d67  _path.display(mg
+000033e0: 2c20 616c 676f 7269 7468 6d3d 2762 6173  , algorithm='bas
+000033f0: 6963 2729 0a20 2020 2022 2222 0a0a 2020  ic').    """..  
+00003400: 2020 6966 2061 6c67 6f72 6974 686d 203d    if algorithm =
+00003410: 3d20 2766 6c6f 7964 5f77 6172 7368 616c  = 'floyd_warshal
+00003420: 6c27 3a0a 2020 2020 2020 2020 7265 7475  l':.        retu
+00003430: 726e 205f 6265 6174 5f70 6174 685f 666c  rn _beat_path_fl
+00003440: 6f79 645f 7761 7273 6861 6c6c 2865 6461  oyd_warshall(eda
+00003450: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00003460: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+00003470: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00003480: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00003490: 6f6e 290a 2020 2020 656c 6966 2061 6c67  on).    elif alg
+000034a0: 6f72 6974 686d 203d 3d20 2762 6173 6963  orithm == 'basic
+000034b0: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
+000034c0: 6e20 5f62 6561 745f 7061 7468 5f62 6173  n _beat_path_bas
+000034d0: 6963 2865 6461 7461 2c20 6375 7272 5f63  ic(edata, curr_c
+000034e0: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+000034f0: 732c 2073 7472 656e 6774 685f 6675 6e63  s, strength_func
+00003500: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
+00003510: 6675 6e63 7469 6f6e 290a 2020 2020 656c  function).    el
+00003520: 6966 2061 6c67 6f72 6974 686d 203d 3d20  if algorithm == 
+00003530: 2773 6368 7761 7274 7a5f 7365 7175 656e  'schwartz_sequen
+00003540: 7469 616c 5f64 726f 7070 696e 6727 3a0a  tial_dropping':.
+00003550: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00003560: 7363 6877 6172 747a 5f73 6571 7565 6e74  schwartz_sequent
+00003570: 6961 6c5f 6472 6f70 7069 6e67 2865 6461  ial_dropping(eda
+00003580: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00003590: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+000035a0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+000035b0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+000035c0: 6f6e 290a 2020 2020 656c 7365 3a0a 2020  on).    else:.  
+000035d0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+000035e0: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+000035f0: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
+00003600: 6965 642e 2229 0a0a 6465 6620 6265 6174  ied.")..def beat
+00003610: 5f70 6174 685f 6465 6665 6174 2865 6461  _path_defeat(eda
+00003620: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
+00003630: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
+00003640: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+00003650: 3a20 2020 0a20 2020 2022 2222 5265 7475  :   .    """Retu
+00003660: 726e 7320 7468 6520 6465 6665 6174 2072  rns the defeat r
+00003670: 656c 6174 696f 6e20 666f 7220 4265 6174  elation for Beat
+00003680: 2050 6174 682e 200a 2020 2020 0a20 2020   Path. .    .   
+00003690: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+000036a0: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+000036b0: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+000036c0: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+000036d0: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+000036e0: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+000036f0: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+00003700: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+00003710: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+00003720: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+00003730: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+00003740: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00003750: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00003760: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00003770: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00003780: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+00003790: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+000037a0: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+000037b0: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+000037c0: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+000037d0: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+000037e0: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+000037f0: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+00003800: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+00003810: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+00003820: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+00003830: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+00003840: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+00003850: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+00003860: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+00003870: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+00003880: 206e 6574 776f 726b 7820 4469 4772 6170   networkx DiGrap
+00003890: 6820 7265 7072 6573 656e 7469 6e67 2074  h representing t
+000038a0: 6865 2042 6561 7420 5061 7468 2064 6566  he Beat Path def
+000038b0: 6561 7420 7265 6c61 7469 6f6e 2e20 0a0a  eat relation. ..
+000038c0: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
+000038d0: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
+000038e0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+000038f0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00003900: 732e 6265 6174 5f70 6174 6860 2c20 3a6d  s.beat_path`, :m
+00003910: 6574 683a 6070 7265 665f 766f 7469 6e67  eth:`pref_voting
+00003920: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00003930: 7468 6f64 732e 6265 6174 5f70 6174 685f  thods.beat_path_
+00003940: 466c 6f79 645f 5761 7273 6861 6c6c 600a  Floyd_Warshall`.
+00003950: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+00003960: 0a20 2020 202e 2e20 706c 6f74 3a3a 2020  .    .. plot::  
+00003970: 6d61 7267 696e 5f67 7261 7068 735f 6578  margin_graphs_ex
+00003980: 616d 706c 6573 2f6d 675f 6578 5f62 705f  amples/mg_ex_bp_
+00003990: 6465 6665 6174 2e70 790a 2020 2020 2020  defeat.py.      
+000039a0: 2020 3a63 6f6e 7465 7874 3a20 7265 7365    :context: rese
+000039b0: 7420 200a 2020 2020 2020 2020 3a69 6e63  t  .        :inc
+000039c0: 6c75 6465 2d73 6f75 7263 653a 2054 7275  lude-source: Tru
+000039d0: 650a 0a20 2020 2022 2222 0a0a 2020 2020  e..    """..    
+000039e0: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+000039f0: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+00003a00: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+00003a10: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+00003a20: 6e64 7320 2020 200a 2020 2020 7374 7265  nds    .    stre
+00003a30: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00003a40: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
+00003a50: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00003a60: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
+00003a70: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00003a80: 0a20 2020 2020 2020 200a 2020 2020 735f  .        .    s_
+00003a90: 6d61 7472 6978 203d 205b 5b2d 6e70 2e69  matrix = [[-np.i
+00003aa0: 6e66 2066 6f72 205f 2069 6e20 6361 6e64  nf for _ in cand
+00003ab0: 6964 6174 6573 5d20 666f 7220 5f20 696e  idates] for _ in
+00003ac0: 2063 616e 6469 6461 7465 735d 0a20 2020   candidates].   
+00003ad0: 2066 6f72 2063 315f 6964 782c 2063 3120   for c1_idx, c1 
+00003ae0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+00003af0: 6469 6461 7465 7329 3a0a 2020 2020 2020  didates):.      
+00003b00: 2020 666f 7220 6332 5f69 6478 2c20 6332    for c2_idx, c2
+00003b10: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00003b20: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
+00003b30: 2020 2020 2020 2069 6620 2865 6461 7461         if (edata
+00003b40: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+00003b50: 7328 6331 2c20 6332 2920 6f72 2063 3120  s(c1, c2) or c1 
+00003b60: 3d3d 2063 3229 3a0a 2020 2020 2020 2020  == c2):.        
+00003b70: 2020 2020 2020 2020 735f 6d61 7472 6978          s_matrix
+00003b80: 5b63 315f 6964 785d 5b63 325f 6964 785d  [c1_idx][c2_idx]
+00003b90: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+00003ba0: 7469 6f6e 2863 312c 2063 3229 200a 2020  tion(c1, c2) .  
+00003bb0: 2020 7374 7265 6e67 7468 203d 206c 6973    strength = lis
+00003bc0: 7428 6d61 7028 6c61 6d62 6461 2069 203a  t(map(lambda i :
+00003bd0: 206c 6973 7428 6d61 7028 6c61 6d62 6461   list(map(lambda
+00003be0: 206a 203a 206a 202c 2069 2929 202c 2073   j : j , i)) , s
+00003bf0: 5f6d 6174 7269 7829 290a 2020 2020 666f  _matrix)).    fo
+00003c00: 7220 695f 6964 782c 2069 2069 6e20 656e  r i_idx, i in en
+00003c10: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+00003c20: 6573 293a 2020 2020 2020 2020 200a 2020  es):         .  
+00003c30: 2020 2020 2020 666f 7220 6a5f 6964 782c        for j_idx,
+00003c40: 206a 2069 6e20 656e 756d 6572 6174 6528   j in enumerate(
+00003c50: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
+00003c60: 2020 2020 2020 2020 2020 6966 2069 213d            if i!=
+00003c70: 206a 3a0a 2020 2020 2020 2020 2020 2020   j:.            
+00003c80: 2020 2020 666f 7220 6b5f 6964 782c 206b      for k_idx, k
+00003c90: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00003ca0: 6e64 6964 6174 6573 293a 200a 2020 2020  ndidates): .    
+00003cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003cc0: 6966 2069 213d 206b 2061 6e64 206a 2021  if i!= k and j !
+00003cd0: 3d20 6b3a 0a20 2020 2020 2020 2020 2020  = k:.           
+00003ce0: 2020 2020 2020 2020 2020 2020 2073 7472               str
+00003cf0: 656e 6774 685b 6a5f 6964 785d 5b6b 5f69  ength[j_idx][k_i
+00003d00: 6478 5d20 3d20 6d61 7828 7374 7265 6e67  dx] = max(streng
+00003d10: 7468 5b6a 5f69 6478 5d5b 6b5f 6964 785d  th[j_idx][k_idx]
+00003d20: 2c20 6d69 6e28 7374 7265 6e67 7468 5b6a  , min(strength[j
+00003d30: 5f69 6478 5d5b 695f 6964 785d 2c73 7472  _idx][i_idx],str
+00003d40: 656e 6774 685b 695f 6964 785d 5b6b 5f69  ength[i_idx][k_i
+00003d50: 6478 5d29 290a 0a20 2020 2064 6566 6561  dx]))..    defea
+00003d60: 745f 6772 6170 6820 3d20 6e78 2e44 6947  t_graph = nx.DiG
+00003d70: 7261 7068 2829 0a20 2020 2064 6566 6561  raph().    defea
+00003d80: 745f 6772 6170 682e 6164 645f 6e6f 6465  t_graph.add_node
+00003d90: 735f 6672 6f6d 2863 616e 6469 6461 7465  s_from(candidate
+00003da0: 7329 0a20 2020 200a 2020 2020 666f 7220  s).    .    for 
+00003db0: 695f 6964 782c 2069 2069 6e20 656e 756d  i_idx, i in enum
+00003dc0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00003dd0: 293a 200a 2020 2020 2020 2020 666f 7220  ): .        for 
+00003de0: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
+00003df0: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00003e00: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00003e10: 6620 6921 3d6a 3a0a 2020 2020 2020 2020  f i!=j:.        
+00003e20: 2020 2020 2020 2020 6966 2073 7472 656e          if stren
+00003e30: 6774 685b 6a5f 6964 785d 5b69 5f69 6478  gth[j_idx][i_idx
+00003e40: 5d20 3e20 7374 7265 6e67 7468 5b69 5f69  ] > strength[i_i
+00003e50: 6478 5d5b 6a5f 6964 785d 3a0a 2020 2020  dx][j_idx]:.    
+00003e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003e70: 6465 6665 6174 5f67 7261 7068 2e61 6464  defeat_graph.add
+00003e80: 5f77 6569 6768 7465 645f 6564 6765 735f  _weighted_edges_
+00003e90: 6672 6f6d 285b 286a 2c69 2c73 5f6d 6174  from([(j,i,s_mat
+00003ea0: 7269 785b 6a5f 6964 785d 5b69 5f69 6478  rix[j_idx][i_idx
+00003eb0: 5d29 5d29 0a0a 2020 2020 7265 7475 726e  ])])..    return
+00003ec0: 2064 6566 6561 745f 6772 6170 680a 0a0a   defeat_graph...
+00003ed0: 0a64 6566 2068 6173 5f73 7472 6f6e 675f  .def has_strong_
+00003ee0: 7061 7468 2841 2c20 736f 7572 6365 2c20  path(A, source, 
+00003ef0: 7461 7267 6574 2c20 6b29 3a0a 2020 2020  target, k):.    
+00003f00: 2222 2247 6976 656e 2061 2073 7175 6172  """Given a squar
+00003f10: 6520 6d61 7472 6978 2041 2c20 7265 7475  e matrix A, retu
+00003f20: 726e 2054 7275 6520 6966 2074 6865 7265  rn True if there
+00003f30: 2069 7320 6120 7061 7468 2066 726f 6d20   is a path from 
+00003f40: 736f 7572 6365 2074 6f20 7461 7267 6574  source to target
+00003f50: 2069 6e20 7468 6520 6173 736f 6369 6174   in the associat
+00003f60: 6564 2064 6972 6563 7465 6420 6772 6170  ed directed grap
+00003f70: 6820 2020 2020 7768 6572 6520 6561 6368  h     where each
+00003f80: 2065 6467 6520 6861 7320 6120 7765 6967   edge has a weig
+00003f90: 6874 2067 7265 6174 6572 2074 6861 6e20  ht greater than 
+00003fa0: 6f72 2065 7175 616c 2074 6f20 6b2c 2061  or equal to k, a
+00003fb0: 6e64 2046 616c 7365 206f 7468 6572 7769  nd False otherwi
+00003fc0: 7365 2e22 2222 0a20 2020 200a 2020 2020  se.""".    .    
+00003fd0: 6e20 3d20 412e 7368 6170 655b 305d 2023  n = A.shape[0] #
+00003fe0: 2061 7373 756d 6520 4120 6973 2061 2073   assume A is a s
+00003ff0: 7175 6172 6520 6d61 7472 6978 0a20 2020  quare matrix.   
+00004000: 2076 6973 6974 6564 203d 206e 702e 7a65   visited = np.ze
+00004010: 726f 7328 6e2c 2064 7479 7065 3d62 6f6f  ros(n, dtype=boo
+00004020: 6c29 0a0a 2020 2020 6465 6620 6466 7328  l)..    def dfs(
+00004030: 6e6f 6465 293a 0a20 2020 2020 2020 2069  node):.        i
+00004040: 6620 6e6f 6465 203d 3d20 7461 7267 6574  f node == target
+00004050: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00004060: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00004070: 2020 7669 7369 7465 645b 6e6f 6465 5d20    visited[node] 
+00004080: 3d20 5472 7565 0a20 2020 2020 2020 2066  = True.        f
+00004090: 6f72 206e 6569 6768 626f 722c 2077 6569  or neighbor, wei
+000040a0: 6768 7420 696e 2065 6e75 6d65 7261 7465  ght in enumerate
+000040b0: 2841 5b6e 6f64 652c 203a 5d29 3a0a 2020  (A[node, :]):.  
+000040c0: 2020 2020 2020 2020 2020 6966 2041 5b6e            if A[n
+000040d0: 6f64 655d 5b6e 6569 6768 626f 725d 203e  ode][neighbor] >
+000040e0: 2041 5b6e 6569 6768 626f 725d 5b6e 6f64   A[neighbor][nod
+000040f0: 655d 2061 6e64 2077 6569 6768 7420 3e3d  e] and weight >=
+00004100: 206b 2061 6e64 206e 6f74 2076 6973 6974   k and not visit
+00004110: 6564 5b6e 6569 6768 626f 725d 3a0a 2020  ed[neighbor]:.  
+00004120: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00004130: 2064 6673 286e 6569 6768 626f 7229 3a0a   dfs(neighbor):.
+00004140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004150: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+00004160: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+00004170: 616c 7365 0a0a 2020 2020 7265 7475 726e  alse..    return
+00004180: 2064 6673 2873 6f75 7263 6529 0a0a 6465   dfs(source)..de
+00004190: 6620 5f73 706c 6974 5f63 7963 6c65 5f62  f _split_cycle_b
+000041a0: 6173 6963 280a 2020 2020 2020 2020 6564  asic(.        ed
+000041b0: 6174 612c 200a 2020 2020 2020 2020 6375  ata, .        cu
+000041c0: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+000041d0: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
+000041e0: 7468 5f66 756e 6374 696f 6e20 3d20 4e6f  th_function = No
+000041f0: 6e65 293a 0a20 2020 2022 2222 416e 2069  ne):.    """An i
+00004200: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f66  mplementation of
+00004210: 2053 706c 6974 2043 7963 6c65 2062 6173   Split Cycle bas
+00004220: 6564 206f 6e20 7468 6520 6d61 7468 656d  ed on the mathem
+00004230: 6174 6963 616c 2064 6566 696e 6974 696f  atical definitio
+00004240: 6e2e 2020 200a 2020 2020 2222 220a 2020  n.   .    """.  
+00004250: 2020 7374 7265 6e67 7468 5f6d 6174 7269    strength_matri
+00004260: 782c 2063 616e 645f 746f 5f63 696e 6465  x, cand_to_cinde
+00004270: 7820 3d20 6564 6174 612e 7374 7265 6e67  x = edata.streng
+00004280: 7468 5f6d 6174 7269 7828 6375 7272 5f63  th_matrix(curr_c
+00004290: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+000042a0: 732c 2073 7472 656e 6774 685f 6675 6e63  s, strength_func
+000042b0: 7469 6f6e 3d73 7472 656e 6774 685f 6675  tion=strength_fu
+000042c0: 6e63 7469 6f6e 290a 0a20 2020 2063 616e  nction)..    can
+000042d0: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+000042e0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+000042f0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00004300: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00004310: 2020 0a0a 2020 2020 7374 7265 6e67 7468    ..    strength
+00004320: 5f66 756e 6374 696f 6e20 3d20 6564 6174  _function = edat
+00004330: 612e 6d61 7267 696e 2069 6620 7374 7265  a.margin if stre
+00004340: 6e67 7468 5f66 756e 6374 696f 6e20 6973  ngth_function is
+00004350: 204e 6f6e 6520 656c 7365 2073 7472 656e   None else stren
+00004360: 6774 685f 6675 6e63 7469 6f6e 200a 0a20  gth_function .. 
+00004370: 2020 2070 6f74 656e 7469 616c 5f77 696e     potential_win
+00004380: 6e65 7273 203d 2073 6574 2863 616e 6469  ners = set(candi
+00004390: 6461 7465 7329 0a0a 2020 2020 666f 7220  dates)..    for 
+000043a0: 6120 696e 2063 616e 6469 6461 7465 733a  a in candidates:
+000043b0: 0a20 2020 2020 2020 2066 6f72 2062 2069  .        for b i
+000043c0: 6e20 6361 6e64 6964 6174 6573 3a0a 2020  n candidates:.  
+000043d0: 2020 2020 2020 2020 2020 6966 2073 7472            if str
+000043e0: 656e 6774 685f 6675 6e63 7469 6f6e 2862  ength_function(b
+000043f0: 2c20 6129 203e 2073 7472 656e 6774 685f  , a) > strength_
+00004400: 6675 6e63 7469 6f6e 2861 2c20 6229 2061  function(a, b) a
+00004410: 6e64 206e 6f74 2068 6173 5f73 7472 6f6e  nd not has_stron
+00004420: 675f 7061 7468 2873 7472 656e 6774 685f  g_path(strength_
+00004430: 6d61 7472 6978 2c20 6361 6e64 5f74 6f5f  matrix, cand_to_
+00004440: 6369 6e64 6578 2861 292c 2063 616e 645f  cindex(a), cand_
+00004450: 746f 5f63 696e 6465 7828 6229 2c20 7374  to_cindex(b), st
+00004460: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
+00004470: 622c 6129 293a 0a20 2020 2020 2020 2020  b,a)):.         
+00004480: 2020 2020 2020 2070 6f74 656e 7469 616c         potential
+00004490: 5f77 696e 6e65 7273 2e64 6973 6361 7264  _winners.discard
+000044a0: 2861 290a 2020 2020 2020 2020 2020 2020  (a).            
+000044b0: 2020 2020 6272 6561 6b0a 0a20 2020 2072      break..    r
+000044c0: 6574 7572 6e20 736f 7274 6564 2870 6f74  eturn sorted(pot
+000044d0: 656e 7469 616c 5f77 696e 6e65 7273 290a  ential_winners).
+000044e0: 0a64 6566 205f 6973 5f63 616e 645f 7370  .def _is_cand_sp
+000044f0: 6c69 745f 6379 636c 655f 6465 6665 6174  lit_cycle_defeat
+00004500: 6564 2861 2c20 7374 7265 6e67 7468 5f6d  ed(a, strength_m
+00004510: 6174 7269 7829 3a0a 0a20 2020 2066 6f72  atrix):..    for
+00004520: 2062 2069 6e20 7261 6e67 6528 7374 7265   b in range(stre
+00004530: 6e67 7468 5f6d 6174 7269 782e 7368 6170  ngth_matrix.shap
+00004540: 655b 305d 293a 0a20 2020 2020 2020 2069  e[0]):.        i
+00004550: 6620 7374 7265 6e67 7468 5f6d 6174 7269  f strength_matri
+00004560: 785b 625d 5b61 5d20 3e20 7374 7265 6e67  x[b][a] > streng
+00004570: 7468 5f6d 6174 7269 785b 615d 5b62 5d20  th_matrix[a][b] 
+00004580: 616e 6420 6e6f 7420 6861 735f 7374 726f  and not has_stro
+00004590: 6e67 5f70 6174 6828 7374 7265 6e67 7468  ng_path(strength
+000045a0: 5f6d 6174 7269 782c 2061 2c20 2062 2c20  _matrix, a,  b, 
+000045b0: 7374 7265 6e67 7468 5f6d 6174 7269 785b  strength_matrix[
+000045c0: 625d 5b61 5d29 3a0a 2020 2020 2020 2020  b][a]):.        
+000045d0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000045e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
+000045f0: 0a0a 0a64 6566 2062 6174 6368 2869 7465  ...def batch(ite
+00004600: 7261 626c 652c 206e 3d31 293a 0a20 2020  rable, n=1):.   
+00004610: 206c 203d 206c 656e 2869 7465 7261 626c   l = len(iterabl
+00004620: 6529 0a20 2020 2066 6f72 206e 6478 2069  e).    for ndx i
+00004630: 6e20 7261 6e67 6528 302c 206c 2c20 6e29  n range(0, l, n)
+00004640: 3a0a 2020 2020 2020 2020 7969 656c 6420  :.        yield 
+00004650: 6974 6572 6162 6c65 5b6e 6478 3a6d 696e  iterable[ndx:min
+00004660: 286e 6478 202b 206e 2c20 6c29 5d0a 0a64  (ndx + n, l)]..d
+00004670: 6566 2070 726f 6365 7373 5f62 6174 6368  ef process_batch
+00004680: 5f6f 665f 6361 6e64 6964 6174 6573 2862  _of_candidates(b
+00004690: 6174 6368 2c20 7374 7265 6e67 7468 5f6d  atch, strength_m
+000046a0: 6174 7269 7829 3a0a 2020 2020 7265 7375  atrix):.    resu
+000046b0: 6c74 7320 3d20 5b5d 0a20 2020 2066 6f72  lts = [].    for
+000046c0: 2063 616e 6469 6461 7465 2069 6e20 6261   candidate in ba
+000046d0: 7463 683a 0a20 2020 2020 2020 2072 6573  tch:.        res
+000046e0: 756c 7420 3d20 5f69 735f 6361 6e64 5f73  ult = _is_cand_s
+000046f0: 706c 6974 5f63 7963 6c65 5f64 6566 6561  plit_cycle_defea
+00004700: 7465 6428 6361 6e64 6964 6174 652c 2073  ted(candidate, s
+00004710: 7472 656e 6774 685f 6d61 7472 6978 290a  trength_matrix).
+00004720: 2020 2020 2020 2020 7265 7375 6c74 732e          results.
+00004730: 6170 7065 6e64 2872 6573 756c 7429 0a20  append(result). 
+00004740: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
+00004750: 730a 0a64 6566 205f 7370 6c69 745f 6379  s..def _split_cy
+00004760: 636c 655f 6261 7369 635f 7061 7261 6c6c  cle_basic_parall
+00004770: 656c 2873 7472 656e 6774 685f 6d61 7472  el(strength_matr
+00004780: 6978 2c20 6e75 6d5f 6370 7573 3d34 293a  ix, num_cpus=4):
+00004790: 0a0a 2020 2020 6e75 6d5f 6361 6e64 7320  ..    num_cands 
+000047a0: 3d20 7374 7265 6e67 7468 5f6d 6174 7269  = strength_matri
+000047b0: 782e 7368 6170 655b 305d 0a20 2020 2063  x.shape[0].    c
+000047c0: 616e 6473 203d 206c 6973 7428 7261 6e67  ands = list(rang
+000047d0: 6528 6e75 6d5f 6361 6e64 7329 290a 2020  e(num_cands)).  
+000047e0: 2020 6261 7463 685f 7369 7a65 203d 206e    batch_size = n
+000047f0: 756d 5f63 616e 6473 202f 2f20 6e75 6d5f  um_cands // num_
+00004800: 6370 7573 202b 2028 6e75 6d5f 6361 6e64  cpus + (num_cand
+00004810: 7320 2520 6e75 6d5f 6370 7573 203e 2030  s % num_cpus > 0
+00004820: 290a 2020 2020 6361 6e64 6964 6174 655f  ).    candidate_
+00004830: 6261 7463 6865 7320 3d20 6c69 7374 2862  batches = list(b
+00004840: 6174 6368 2863 616e 6473 2c20 6261 7463  atch(cands, batc
+00004850: 685f 7369 7a65 2929 0a20 2020 2077 6974  h_size)).    wit
+00004860: 6820 506f 6f6c 286e 756d 5f63 7075 7329  h Pool(num_cpus)
+00004870: 2061 7320 706f 6f6c 3a0a 2020 2020 2020   as pool:.      
+00004880: 2020 6261 7463 685f 6172 6773 203d 205b    batch_args = [
+00004890: 2862 6174 6368 2c20 7374 7265 6e67 7468  (batch, strength
+000048a0: 5f6d 6174 7269 7829 200a 2020 2020 2020  _matrix) .      
+000048b0: 2020 666f 7220 6261 7463 6820 696e 2063    for batch in c
+000048c0: 616e 6469 6461 7465 5f62 6174 6368 6573  andidate_batches
+000048d0: 5d0a 2020 2020 2020 2020 7265 7375 6c74  ].        result
+000048e0: 7320 3d20 706f 6f6c 2e73 7461 726d 6170  s = pool.starmap
+000048f0: 2870 726f 6365 7373 5f62 6174 6368 5f6f  (process_batch_o
+00004900: 665f 6361 6e64 6964 6174 6573 2c20 6261  f_candidates, ba
+00004910: 7463 685f 6172 6773 290a 2020 2020 2320  tch_args).    # 
+00004920: 466c 6174 7465 6e20 7468 6520 6c69 7374  Flatten the list
+00004930: 206f 6620 7265 7375 6c74 730a 2020 2020   of results.    
+00004940: 7363 5f64 6566 6561 745f 6461 7461 203d  sc_defeat_data =
+00004950: 205b 6974 656d 2066 6f72 2073 7562 6c69   [item for subli
+00004960: 7374 2069 6e20 7265 7375 6c74 7320 666f  st in results fo
+00004970: 7220 6974 656d 2069 6e20 7375 626c 6973  r item in sublis
+00004980: 745d 0a0a 2020 2020 7265 7475 726e 2073  t]..    return s
+00004990: 6f72 7465 6428 5b63 2066 6f72 2063 2069  orted([c for c i
+000049a0: 6e20 6361 6e64 7320 6966 206e 6f74 2073  n cands if not s
+000049b0: 635f 6465 6665 6174 5f64 6174 615b 635d  c_defeat_data[c]
+000049c0: 5d29 0a0a 6465 6620 5f73 706c 6974 5f63  ])..def _split_c
+000049d0: 7963 6c65 5f66 6c6f 7964 5f77 6172 7368  ycle_floyd_warsh
+000049e0: 616c 6c28 0a20 2020 2020 2020 2065 6461  all(.        eda
+000049f0: 7461 2c20 0a20 2020 2020 2020 2063 7572  ta, .        cur
+00004a00: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
+00004a10: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00004a20: 685f 6675 6e63 7469 6f6e 203d 204e 6f6e  h_function = Non
+00004a30: 6529 3a20 2020 0a20 2020 2022 2222 416e  e):   .    """An
+00004a40: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+00004a50: 6f66 2053 706c 6974 2043 7963 6c65 2062  of Split Cycle b
+00004a60: 6173 6564 206f 6e20 7468 6520 466c 6f79  ased on the Floy
+00004a70: 642d 5761 7273 6861 6c6c 2041 6c67 6f72  d-Warshall Algor
+00004a80: 6974 686d 2e20 0a0a 2020 2020 5365 6520  ithm. ..    See 
+00004a90: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00004aa0: 6f6d 2f65 7061 6375 6974 2f73 706c 6974  om/epacuit/split
+00004ab0: 6379 636c 6520 616e 6420 7468 6520 7061  cycle and the pa
+00004ac0: 7065 7220 6874 7470 733a 2f2f 6172 7869  per https://arxi
+00004ad0: 762e 6f72 672f 6162 732f 3230 3034 2e30  v.org/abs/2004.0
+00004ae0: 3233 3530 2066 6f72 206d 6f72 6520 696e  2350 for more in
+00004af0: 666f 726d 6174 696f 6e2e 200a 0a20 2020  formation. ..   
+00004b00: 2022 2222 0a0a 2020 2020 6361 6e64 6964   """..    candid
+00004b10: 6174 6573 203d 2065 6461 7461 2e63 616e  ates = edata.can
+00004b20: 6469 6461 7465 7320 6966 2063 7572 725f  didates if curr_
+00004b30: 6361 6e64 7320 6973 204e 6f6e 6520 656c  cands is None el
+00004b40: 7365 2063 7572 725f 6361 6e64 7320 2020  se curr_cands   
+00004b50: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+00004b60: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
+00004b70: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
+00004b80: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
+00004b90: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
+00004ba0: 685f 6675 6e63 7469 6f6e 200a 200a 2020  h_function . .  
+00004bb0: 2020 7765 616b 5f63 6f6e 646f 7263 6574    weak_condorcet
+00004bc0: 5f77 696e 6e65 7273 203d 207b 633a 5472  _winners = {c:Tr
+00004bd0: 7565 2066 6f72 2063 2069 6e20 6361 6e64  ue for c in cand
+00004be0: 6964 6174 6573 7d0a 2020 2020 735f 6d61  idates}.    s_ma
+00004bf0: 7472 6978 203d 205b 5b2d 6e70 2e69 6e66  trix = [[-np.inf
+00004c00: 2066 6f72 205f 2069 6e20 6361 6e64 6964   for _ in candid
+00004c10: 6174 6573 5d20 666f 7220 5f20 696e 2063  ates] for _ in c
+00004c20: 616e 6469 6461 7465 735d 0a20 2020 200a  andidates].    .
+00004c30: 2020 2020 2320 696e 6974 6961 6c69 7a65      # initialize
+00004c40: 2074 6865 2073 5f6d 6174 7269 780a 2020   the s_matrix.  
+00004c50: 2020 666f 7220 6331 5f69 6478 2c20 6331    for c1_idx, c1
+00004c60: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00004c70: 6e64 6964 6174 6573 293a 0a20 2020 2020  ndidates):.     
+00004c80: 2020 2066 6f72 2063 325f 6964 782c 2063     for c2_idx, c
+00004c90: 3220 696e 2065 6e75 6d65 7261 7465 2863  2 in enumerate(c
+00004ca0: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
+00004cb0: 2020 2020 2020 2020 6966 2028 6564 6174          if (edat
+00004cc0: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
+00004cd0: 7273 2863 312c 2063 3229 206f 7220 6331  rs(c1, c2) or c1
+00004ce0: 203d 3d20 6332 293a 0a20 2020 2020 2020   == c2):.       
+00004cf0: 2020 2020 2020 2020 2073 5f6d 6174 7269           s_matri
+00004d00: 785b 6331 5f69 6478 5d5b 6332 5f69 6478  x[c1_idx][c2_idx
+00004d10: 5d20 3d20 7374 7265 6e67 7468 5f66 756e  ] = strength_fun
+00004d20: 6374 696f 6e28 6331 2c20 6332 2920 0a20  ction(c1, c2) . 
+00004d30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+00004d40: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
+00004d50: 6e6e 6572 735b 6332 5d20 3d20 7765 616b  nners[c2] = weak
+00004d60: 5f63 6f6e 646f 7263 6574 5f77 696e 6e65  _condorcet_winne
+00004d70: 7273 5b63 325d 2061 6e64 2028 6331 203d  rs[c2] and (c1 =
+00004d80: 3d20 6332 2920 2320 5765 616b 2043 6f6e  = c2) # Weak Con
+00004d90: 646f 7263 6574 2077 696e 6e65 7273 2061  dorcet winners a
+00004da0: 7265 2053 706c 6974 2043 7963 6c65 2077  re Split Cycle w
+00004db0: 696e 6e65 7273 0a20 2020 200a 2020 2020  inners.    .    
+00004dc0: 7374 7265 6e67 7468 203d 206c 6973 7428  strength = list(
+00004dd0: 6d61 7028 6c61 6d62 6461 2069 203a 206c  map(lambda i : l
+00004de0: 6973 7428 6d61 7028 6c61 6d62 6461 206a  ist(map(lambda j
+00004df0: 203a 206a 202c 2069 2929 202c 2073 5f6d   : j , i)) , s_m
+00004e00: 6174 7269 7829 290a 2020 2020 666f 7220  atrix)).    for 
+00004e10: 695f 6964 782c 2069 2069 6e20 656e 756d  i_idx, i in enum
+00004e20: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00004e30: 293a 200a 2020 2020 2020 2020 666f 7220  ): .        for 
+00004e40: 6a5f 6964 782c 206a 2069 6e20 656e 756d  j_idx, j in enum
+00004e50: 6572 6174 6528 6361 6e64 6964 6174 6573  erate(candidates
+00004e60: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00004e70: 6620 6921 3d20 6a3a 0a20 2020 2020 2020  f i!= j:.       
+00004e80: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00004e90: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
+00004ea0: 696e 6e65 7273 5b6a 5d3a 2023 2077 6561  inners[j]: # wea
+00004eb0: 6b20 436f 6e64 6f72 6365 7420 7769 6e6e  k Condorcet winn
+00004ec0: 6572 7320 6172 6520 5370 6c69 7420 4379  ers are Split Cy
+00004ed0: 636c 6520 7769 6e6e 6572 730a 2020 2020  cle winners.    
+00004ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ef0: 666f 7220 6b5f 6964 782c 206b 2069 6e20  for k_idx, k in 
+00004f00: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+00004f10: 6174 6573 293a 200a 2020 2020 2020 2020  ates): .        
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 6966 2069 2021 3d20 6b20 616e 6420 6a20  if i != k and j 
+00004f40: 213d 206b 3a0a 2020 2020 2020 2020 2020  != k:.          
+00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f60: 2020 7374 7265 6e67 7468 5b6a 5f69 6478    strength[j_idx
+00004f70: 5d5b 6b5f 6964 785d 203d 206d 6178 2873  ][k_idx] = max(s
+00004f80: 7472 656e 6774 685b 6a5f 6964 785d 5b6b  trength[j_idx][k
+00004f90: 5f69 6478 5d2c 206d 696e 2873 7472 656e  _idx], min(stren
+00004fa0: 6774 685b 6a5f 6964 785d 5b69 5f69 6478  gth[j_idx][i_idx
+00004fb0: 5d2c 7374 7265 6e67 7468 5b69 5f69 6478  ],strength[i_idx
+00004fc0: 5d5b 6b5f 6964 785d 2929 0a20 2020 2077  ][k_idx])).    w
+00004fd0: 696e 6e65 7273 203d 207b 693a 5472 7565  inners = {i:True
+00004fe0: 2066 6f72 2069 2069 6e20 6361 6e64 6964   for i in candid
+00004ff0: 6174 6573 7d0a 2020 2020 666f 7220 695f  ates}.    for i_
+00005000: 6964 782c 2069 2069 6e20 656e 756d 6572  idx, i in enumer
+00005010: 6174 6528 6361 6e64 6964 6174 6573 293a  ate(candidates):
+00005020: 0a20 2020 2020 2020 2066 6f72 206a 5f69  .        for j_i
+00005030: 6478 2c20 6a20 696e 2065 6e75 6d65 7261  dx, j in enumera
+00005040: 7465 2863 616e 6469 6461 7465 7329 3a0a  te(candidates):.
+00005050: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00005060: 2021 3d20 6a3a 0a20 2020 2020 2020 2020   != j:.         
+00005070: 2020 2020 2020 2069 6620 735f 6d61 7472         if s_matr
+00005080: 6978 5b6a 5f69 6478 5d5b 695f 6964 785d  ix[j_idx][i_idx]
+00005090: 203e 2073 7472 656e 6774 685b 695f 6964   > strength[i_id
+000050a0: 785d 5b6a 5f69 6478 5d3a 2023 2074 6865  x][j_idx]: # the
+000050b0: 206d 6169 6e20 6469 6666 6572 656e 6365   main difference
+000050c0: 2077 6974 6820 4265 6174 2050 6174 680a   with Beat Path.
+000050d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050e0: 2020 2020 7769 6e6e 6572 735b 695d 203d      winners[i] =
+000050f0: 2046 616c 7365 0a20 2020 2072 6574 7572   False.    retur
+00005100: 6e20 736f 7274 6564 285b 6320 666f 7220  n sorted([c for 
+00005110: 6320 696e 2063 616e 6469 6461 7465 7320  c in candidates 
+00005120: 6966 2077 696e 6e65 7273 5b63 5d5d 290a  if winners[c]]).
+00005130: 0a40 766d 286e 616d 653d 2253 706c 6974  .@vm(name="Split
+00005140: 2043 7963 6c65 222c 0a20 2020 2069 6e70   Cycle",.    inp
+00005150: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
+00005160: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
+00005170: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
+00005180: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
+00005190: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+000051a0: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
+000051b0: 6566 2073 706c 6974 5f63 7963 6c65 280a  ef split_cycle(.
+000051c0: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
+000051d0: 6375 7272 5f63 616e 6473 3d4e 6f6e 652c  curr_cands=None,
+000051e0: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+000051f0: 756e 6374 696f 6e3d 4e6f 6e65 2c0a 2020  unction=None,.  
+00005200: 2020 616c 676f 7269 7468 6d3d 2762 6173    algorithm='bas
+00005210: 6963 272c 0a20 2020 206e 756d 5f63 7075  ic',.    num_cpu
+00005220: 733d 3429 3a0a 0a20 2020 2022 2222 4120  s=4):..    """A 
+00005230: 2a2a 6d61 6a6f 7269 7479 2063 7963 6c65  **majority cycle
+00005240: 2a2a 2069 7320 6120 7365 7175 656e 6365  ** is a sequence
+00005250: 203a 6d61 7468 3a60 785f 312c 205c 6c64   :math:`x_1, \ld
+00005260: 6f74 7320 2c78 5f6e 6020 6f66 2064 6973  ots ,x_n` of dis
+00005270: 7469 6e63 7420 6361 6e64 6964 6174 6573  tinct candidates
+00005280: 2077 6974 6820 3a6d 6174 683a 6078 5f31   with :math:`x_1
+00005290: 3d78 5f6e 6020 7375 6368 2074 6861 7420  =x_n` such that 
+000052a0: 666f 7220 3a6d 6174 683a 6031 205c 6c65  for :math:`1 \le
+000052b0: 7120 6b20 5c6c 6571 206e 2d31 602c 2020  q k \leq n-1`,  
+000052c0: 3a6d 6174 683a 6078 5f6b 6020 6973 206d  :math:`x_k` is m
+000052d0: 616a 6f72 6974 7920 7072 6566 6572 7265  ajority preferre
+000052e0: 6420 746f 203a 6d61 7468 3a60 785f 7b6b  d to :math:`x_{k
+000052f0: 2b31 7d60 2e20 2054 6865 2053 706c 6974  +1}`.  The Split
+00005300: 2043 7963 6c65 2077 696e 6e65 7273 2061   Cycle winners a
+00005310: 7265 2064 6574 6572 6d69 6e65 6420 6173  re determined as
+00005320: 2066 6f6c 6c6f 7773 3a20 200a 2020 2020   follows:  .    
+00005330: 0a20 2020 2049 6620 6361 6e64 6964 6174  .    If candidat
+00005340: 6520 7820 6861 7320 6120 706f 7369 7469  e x has a positi
+00005350: 7665 206d 6172 6769 6e20 6f76 6572 2079  ve margin over y
+00005360: 2061 6e64 2028 782c 7929 2069 7320 6e6f   and (x,y) is no
+00005370: 7420 7468 6520 7765 616b 6573 7420 6564  t the weakest ed
+00005380: 6765 2069 6e20 6120 6379 636c 652c 2074  ge in a cycle, t
+00005390: 6865 6e20 7820 6465 6665 6174 7320 792e  hen x defeats y.
+000053a0: 2045 7175 6976 616c 656e 746c 792c 2069   Equivalently, i
+000053b0: 6620 7820 6861 7320 6120 706f 7369 7469  f x has a positi
+000053c0: 7665 206d 6172 6769 6e20 6f76 6572 2079  ve margin over y
+000053d0: 2061 6e64 2074 6865 7265 2069 7320 6e6f   and there is no
+000053e0: 2070 6174 6820 6672 6f6d 2079 2062 6163   path from y bac
+000053f0: 6b20 746f 2078 206f 6620 7374 7265 6e67  k to x of streng
+00005400: 7468 2061 7420 6c65 6173 7420 7468 6520  th at least the 
+00005410: 6d61 7267 696e 206f 6620 7820 6f76 6572  margin of x over
+00005420: 2079 2c20 7468 656e 2078 2064 6566 6561   y, then x defea
+00005430: 7473 2079 2e20 0a20 2020 200a 2020 2020  ts y. .    .    
+00005440: 5468 6520 6361 6e64 6964 6174 6573 2074  The candidates t
+00005450: 6861 7420 6172 6520 756e 6465 6665 6174  hat are undefeat
+00005460: 6564 2061 7265 2074 6865 2053 706c 6974  ed are the Split
+00005470: 2043 7963 6c65 2077 696e 6e65 7273 2e0a   Cycle winners..
+00005480: 0a20 2020 2053 6565 2068 7474 7073 3a2f  .    See https:/
+00005490: 2f67 6974 6875 622e 636f 6d2f 6570 6163  /github.com/epac
+000054a0: 7569 742f 7370 6c69 7463 7963 6c65 2061  uit/splitcycle a
+000054b0: 6e64 2074 6865 2070 6170 6572 2068 7474  nd the paper htt
+000054c0: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+000054d0: 6273 2f32 3030 342e 3032 3335 3020 666f  bs/2004.02350 fo
+000054e0: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
+000054f0: 6f6e 2e20 0a0a 2020 2020 4172 6773 3a0a  on. ..    Args:.
+00005500: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00005510: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00005520: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00005530: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00005540: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00005550: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+00005560: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+00005570: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+00005580: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+00005590: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+000055a0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+000055b0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+000055c0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+000055d0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+000055e0: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+000055f0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+00005600: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+00005610: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00005620: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+00005630: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+00005640: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+00005650: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+00005660: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+00005670: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+00005680: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+00005690: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+000056a0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+000056b0: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+000056c0: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+000056d0: 0a20 2020 2020 2020 2061 6c67 6f72 6974  .        algorit
+000056e0: 686d 2028 7374 7229 3a20 5370 6563 6966  hm (str): Specif
+000056f0: 7920 7768 6963 6820 616c 676f 7269 7468  y which algorith
+00005700: 6d20 746f 2075 7365 2e20 204f 7074 696f  m to use.  Optio
+00005710: 6e73 2061 7265 2027 6261 7369 6327 2028  ns are 'basic' (
+00005720: 7468 6520 6465 6661 756c 7429 2061 6e64  the default) and
+00005730: 2027 666c 6f79 645f 7761 7273 6861 6c6c   'floyd_warshall
+00005740: 272e 0a0a 2020 2020 5265 7475 726e 733a  '...    Returns:
+00005750: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+00005760: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+00005770: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
+00005780: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+00005790: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+000057a0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+000057b0: 6564 5f6d 6574 686f 6473 2e73 706c 6974  ed_methods.split
+000057c0: 5f63 7963 6c65 5f64 6566 6561 7460 0a0a  _cycle_defeat`..
+000057d0: 2020 2020 3a45 7861 6d70 6c65 3a20 0a0a      :Example: ..
+000057e0: 2020 2020 2e2e 2070 6c6f 743a 3a20 206d      .. plot::  m
+000057f0: 6172 6769 6e5f 6772 6170 6873 5f65 7861  argin_graphs_exa
+00005800: 6d70 6c65 732f 6d67 5f65 785f 6270 5f72  mples/mg_ex_bp_r
+00005810: 702e 7079 0a20 2020 2020 2020 203a 636f  p.py.        :co
+00005820: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
+00005830: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
+00005840: 736f 7572 6365 3a20 5472 7565 0a0a 2020  source: True..  
+00005850: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
+00005860: 3a20 0a0a 2020 2020 2020 2020 6672 6f6d  : ..        from
+00005870: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+00005880: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00005890: 7320 696d 706f 7274 2073 706c 6974 5f63  s import split_c
+000058a0: 7963 6c65 0a0a 2020 2020 2020 2020 7370  ycle..        sp
+000058b0: 6c69 745f 6379 636c 652e 6469 7370 6c61  lit_cycle.displa
+000058c0: 7928 6d67 290a 0a0a 2020 2020 2e2e 2065  y(mg)...    .. e
+000058d0: 7865 635f 636f 6465 3a3a 200a 2020 2020  xec_code:: .    
+000058e0: 2020 2020 3a68 6964 655f 636f 6465 3a0a      :hide_code:.
+000058f0: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+00005900: 6566 5f76 6f74 696e 672e 7765 6967 6874  ef_voting.weight
+00005910: 6564 5f6d 616a 6f72 6974 795f 6772 6170  ed_majority_grap
+00005920: 6873 2069 6d70 6f72 7420 4d61 7267 696e  hs import Margin
+00005930: 4772 6170 680a 2020 2020 2020 2020 6672  Graph.        fr
+00005940: 6f6d 2070 7265 665f 766f 7469 6e67 2e6d  om pref_voting.m
+00005950: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
+00005960: 6f64 7320 696d 706f 7274 2073 706c 6974  ods import split
+00005970: 5f63 7963 6c65 0a20 2020 2020 2020 200a  _cycle.        .
+00005980: 2020 2020 2020 2020 6d67 203d 204d 6172          mg = Mar
+00005990: 6769 6e47 7261 7068 285b 302c 2031 2c20  ginGraph([0, 1, 
+000059a0: 322c 2033 5d2c 205b 2830 2c20 322c 2033  2, 3], [(0, 2, 3
+000059b0: 292c 2028 312c 2030 2c20 3529 2c20 2832  ), (1, 0, 5), (2
+000059c0: 2c20 312c 2035 292c 2028 322c 2033 2c20  , 1, 5), (2, 3, 
+000059d0: 3129 2c20 2833 2c20 302c 2033 292c 2028  1), (3, 0, 3), (
+000059e0: 332c 2031 2c20 3129 5d29 0a20 2020 2020  3, 1, 1)]).     
+000059f0: 2020 200a 2020 2020 2020 2020 7370 6c69     .        spli
+00005a00: 745f 6379 636c 652e 6469 7370 6c61 7928  t_cycle.display(
+00005a10: 6d67 290a 2020 2020 2020 2020 7370 6c69  mg).        spli
+00005a20: 745f 6379 636c 652e 6469 7370 6c61 7928  t_cycle.display(
+00005a30: 6d67 2c20 616c 676f 7269 7468 6d3d 2762  mg, algorithm='b
+00005a40: 6173 6963 2729 0a20 2020 2020 2020 2073  asic').        s
+00005a50: 706c 6974 5f63 7963 6c65 2e64 6973 706c  plit_cycle.displ
+00005a60: 6179 286d 672c 2061 6c67 6f72 6974 686d  ay(mg, algorithm
+00005a70: 3d27 666c 6f79 645f 7761 7273 6861 6c6c  ='floyd_warshall
+00005a80: 2729 0a20 2020 2022 2222 0a20 2020 200a  ').    """.    .
+00005a90: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
+00005aa0: 203d 3d20 2762 6173 6963 273a 0a20 2020   == 'basic':.   
+00005ab0: 2020 2020 2072 6574 7572 6e20 5f73 706c       return _spl
+00005ac0: 6974 5f63 7963 6c65 5f62 6173 6963 2865  it_cycle_basic(e
+00005ad0: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00005ae0: 203d 2063 7572 725f 6361 6e64 732c 2073   = curr_cands, s
+00005af0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00005b00: 203d 2073 7472 656e 6774 685f 6675 6e63   = strength_func
+00005b10: 7469 6f6e 290a 2020 2020 656c 6966 2061  tion).    elif a
+00005b20: 6c67 6f72 6974 686d 203d 3d20 2766 6c6f  lgorithm == 'flo
+00005b30: 7964 5f77 6172 7368 616c 6c27 3a0a 2020  yd_warshall':.  
+00005b40: 2020 2020 2020 7265 7475 726e 205f 7370        return _sp
+00005b50: 6c69 745f 6379 636c 655f 666c 6f79 645f  lit_cycle_floyd_
+00005b60: 7761 7273 6861 6c6c 2865 6461 7461 2c20  warshall(edata, 
+00005b70: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
+00005b80: 725f 6361 6e64 732c 2073 7472 656e 6774  r_cands, strengt
+00005b90: 685f 6675 6e63 7469 6f6e 203d 2073 7472  h_function = str
+00005ba0: 656e 6774 685f 6675 6e63 7469 6f6e 290a  ength_function).
+00005bb0: 2020 2020 656c 6966 2061 6c67 6f72 6974      elif algorit
+00005bc0: 686d 203d 3d20 2762 6173 6963 5f70 6172  hm == 'basic_par
+00005bd0: 616c 6c65 6c27 3a0a 2020 2020 2020 2020  allel':.        
+00005be0: 6375 7272 5f63 616e 6473 203d 2065 6461  curr_cands = eda
+00005bf0: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+00005c00: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+00005c10: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+00005c20: 6e64 730a 2020 2020 2020 2020 7374 7265  nds.        stre
+00005c30: 6e67 7468 5f6d 6174 7269 782c 2063 616e  ngth_matrix, can
+00005c40: 645f 746f 5f63 696e 6465 7820 3d20 6564  d_to_cindex = ed
+00005c50: 6174 612e 7374 7265 6e67 7468 5f6d 6174  ata.strength_mat
+00005c60: 7269 7828 6375 7272 5f63 616e 6473 203d  rix(curr_cands =
+00005c70: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
+00005c80: 656e 6774 685f 6675 6e63 7469 6f6e 3d73  ength_function=s
+00005c90: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00005ca0: 290a 2020 2020 2020 2020 6369 6e64 785f  ).        cindx_
+00005cb0: 746f 5f63 616e 6420 3d20 7b63 616e 645f  to_cand = {cand_
+00005cc0: 746f 5f63 696e 6465 7828 6329 3a63 2066  to_cindex(c):c f
+00005cd0: 6f72 2063 2069 6e20 6375 7272 5f63 616e  or c in curr_can
+00005ce0: 6473 7d0a 2020 2020 2020 2020 7363 5f77  ds}.        sc_w
+00005cf0: 7320 3d20 5f73 706c 6974 5f63 7963 6c65  s = _split_cycle
+00005d00: 5f62 6173 6963 5f70 6172 616c 6c65 6c28  _basic_parallel(
+00005d10: 7374 7265 6e67 7468 5f6d 6174 7269 782c  strength_matrix,
+00005d20: 6e75 6d5f 6370 7573 3d6e 756d 5f63 7075  num_cpus=num_cpu
+00005d30: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00005d40: 6e20 736f 7274 6564 285b 6369 6e64 785f  n sorted([cindx_
+00005d50: 746f 5f63 616e 645b 635d 2066 6f72 2063  to_cand[c] for c
+00005d60: 2069 6e20 7363 5f77 735d 290a 2020 2020   in sc_ws]).    
+00005d70: 656c 7365 3a0a 2020 2020 2020 2020 7261  else:.        ra
+00005d80: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00005d90: 496e 7661 6c69 6420 616c 676f 7269 7468  Invalid algorith
+00005da0: 6d20 7370 6563 6966 6965 642e 2229 0a0a  m specified.")..
+00005db0: 0a64 6566 2073 706c 6974 5f63 7963 6c65  .def split_cycle
+00005dc0: 5f64 6566 6561 7428 6564 6174 612c 2063  _defeat(edata, c
+00005dd0: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+00005de0: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00005df0: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
+00005e00: 2020 2020 2222 220a 2020 2020 5265 7475      """.    Retu
+00005e10: 726e 7320 7468 6520 5370 6c69 7420 4379  rns the Split Cy
+00005e20: 636c 6520 6465 6665 6174 2072 656c 6174  cle defeat relat
+00005e30: 696f 6e2e 200a 0a20 2020 2053 6565 2068  ion. ..    See h
+00005e40: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00005e50: 2f61 6273 2f32 3030 382e 3038 3435 3120  /abs/2008.08451 
+00005e60: 666f 7220 616e 2065 7874 656e 6465 6420  for an extended 
+00005e70: 6469 7363 7573 7369 6f6e 206f 6620 7468  discussion of th
+00005e80: 6973 206e 6f74 696f 6e20 6f66 2064 6566  is notion of def
+00005e90: 6561 7420 696e 2061 6e20 656c 6563 7469  eat in an electi
+00005ea0: 6f6e 2e20 0a0a 2020 2020 4172 6773 3a0a  on. ..    Args:.
+00005eb0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00005ec0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00005ed0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00005ee0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00005ef0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00005f00: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+00005f10: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+00005f20: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+00005f30: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+00005f40: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+00005f50: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+00005f60: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+00005f70: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+00005f80: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+00005f90: 6375 7272 5f63 616e 6473 6060 0a0a 2020  curr_cands``..  
+00005fa0: 2020 5265 7475 726e 733a 200a 2020 2020    Returns: .    
+00005fb0: 2020 2020 4120 6e65 7477 6f72 6b78 2044      A networkx D
+00005fc0: 6947 7261 7068 2072 6570 7265 7365 6e74  iGraph represent
+00005fd0: 696e 6720 7468 6520 5370 6c69 7420 4379  ing the Split Cy
+00005fe0: 636c 6520 6465 6665 6174 2072 656c 6174  cle defeat relat
+00005ff0: 696f 6e2e 200a 0a20 2020 202e 2e20 7365  ion. ..    .. se
+00006000: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
+00006010: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+00006020: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+00006030: 5f6d 6574 686f 6473 2e73 706c 6974 5f63  _methods.split_c
+00006040: 7963 6c65 602c 203a 6d65 7468 3a60 7072  ycle`, :meth:`pr
+00006050: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00006060: 5f62 6173 6564 5f6d 6574 686f 6473 2e73  _based_methods.s
+00006070: 706c 6974 5f63 7963 6c65 5f46 6c6f 7964  plit_cycle_Floyd
+00006080: 5f57 6172 7368 616c 6c60 0a0a 2020 2020  _Warshall`..    
+00006090: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+000060a0: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+000060b0: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+000060c0: 732f 6d67 5f65 785f 7363 5f64 6566 6561  s/mg_ex_sc_defea
+000060d0: 742e 7079 0a20 2020 2020 2020 203a 636f  t.py.        :co
+000060e0: 6e74 6578 743a 2072 6573 6574 2020 0a20  ntext: reset  . 
+000060f0: 2020 2020 2020 203a 696e 636c 7564 652d         :include-
+00006100: 736f 7572 6365 3a20 5472 7565 0a0a 2020  source: True..  
+00006110: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
+00006120: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+00006130: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00006140: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+00006150: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+00006160: 2020 0a20 2020 2073 7472 656e 6774 685f    .    strength_
+00006170: 6675 6e63 7469 6f6e 203d 2065 6461 7461  function = edata
+00006180: 2e6d 6172 6769 6e20 6966 2073 7472 656e  .margin if stren
+00006190: 6774 685f 6675 6e63 7469 6f6e 2069 7320  gth_function is 
+000061a0: 4e6f 6e65 2065 6c73 6520 7374 7265 6e67  None else streng
+000061b0: 7468 5f66 756e 6374 696f 6e20 0a20 0a20  th_function . . 
+000061c0: 2020 2077 6561 6b5f 636f 6e64 6f72 6365     weak_condorce
+000061d0: 745f 7769 6e6e 6572 7320 3d20 7b63 3a54  t_winners = {c:T
+000061e0: 7275 6520 666f 7220 6320 696e 2063 616e  rue for c in can
+000061f0: 6469 6461 7465 737d 0a20 2020 2073 5f6d  didates}.    s_m
+00006200: 6174 7269 7820 3d20 5b5b 2d6e 702e 696e  atrix = [[-np.in
+00006210: 6620 666f 7220 5f20 696e 2063 616e 6469  f for _ in candi
+00006220: 6461 7465 735d 2066 6f72 205f 2069 6e20  dates] for _ in 
+00006230: 6361 6e64 6964 6174 6573 5d0a 2020 2020  candidates].    
+00006240: 0a20 2020 2023 2069 6e69 7469 616c 697a  .    # initializ
+00006250: 6520 7468 6520 735f 6d61 7472 6978 0a20  e the s_matrix. 
+00006260: 2020 2066 6f72 2063 315f 6964 782c 2063     for c1_idx, c
+00006270: 3120 696e 2065 6e75 6d65 7261 7465 2863  1 in enumerate(c
+00006280: 616e 6469 6461 7465 7329 3a0a 2020 2020  andidates):.    
+00006290: 2020 2020 666f 7220 6332 5f69 6478 2c20      for c2_idx, 
+000062a0: 6332 2069 6e20 656e 756d 6572 6174 6528  c2 in enumerate(
+000062b0: 6361 6e64 6964 6174 6573 293a 0a20 2020  candidates):.   
+000062c0: 2020 2020 2020 2020 2069 6620 2865 6461           if (eda
+000062d0: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+000062e0: 6572 7328 6331 2c20 6332 2920 6f72 2063  ers(c1, c2) or c
+000062f0: 3120 3d3d 2063 3229 3a0a 2020 2020 2020  1 == c2):.      
+00006300: 2020 2020 2020 2020 2020 735f 6d61 7472            s_matr
+00006310: 6978 5b63 315f 6964 785d 5b63 325f 6964  ix[c1_idx][c2_id
+00006320: 785d 203d 2073 7472 656e 6774 685f 6675  x] = strength_fu
+00006330: 6e63 7469 6f6e 2863 312c 2063 3229 200a  nction(c1, c2) .
+00006340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006350: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
+00006360: 696e 6e65 7273 5b63 325d 203d 2077 6561  inners[c2] = wea
+00006370: 6b5f 636f 6e64 6f72 6365 745f 7769 6e6e  k_condorcet_winn
+00006380: 6572 735b 6332 5d20 616e 6420 2863 3120  ers[c2] and (c1 
+00006390: 3d3d 2063 3229 2023 2077 6561 6b20 436f  == c2) # weak Co
+000063a0: 6e64 6f72 6365 7420 7769 6e6e 6572 7320  ndorcet winners 
+000063b0: 6172 6520 5370 6c69 7420 4379 636c 6520  are Split Cycle 
+000063c0: 7769 6e6e 6572 730a 2020 2020 0a20 2020  winners.    .   
+000063d0: 2073 7472 656e 6774 6820 3d20 6c69 7374   strength = list
+000063e0: 286d 6170 286c 616d 6264 6120 6920 3a20  (map(lambda i : 
+000063f0: 6c69 7374 286d 6170 286c 616d 6264 6120  list(map(lambda 
+00006400: 6a20 3a20 6a20 2c20 6929 2920 2c20 735f  j : j , i)) , s_
+00006410: 6d61 7472 6978 2929 0a20 2020 2066 6f72  matrix)).    for
+00006420: 2069 5f69 6478 2c20 6920 696e 2065 6e75   i_idx, i in enu
+00006430: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00006440: 7329 3a20 0a20 2020 2020 2020 2066 6f72  s): .        for
+00006450: 206a 5f69 6478 2c20 6a20 696e 2065 6e75   j_idx, j in enu
+00006460: 6d65 7261 7465 2863 616e 6469 6461 7465  merate(candidate
+00006470: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00006480: 6966 2069 213d 206a 3a0a 2020 2020 2020  if i!= j:.      
+00006490: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+000064a0: 2077 6561 6b5f 636f 6e64 6f72 6365 745f   weak_condorcet_
+000064b0: 7769 6e6e 6572 735b 6a5d 3a20 2320 7765  winners[j]: # we
+000064c0: 616b 2043 6f6e 646f 7263 6574 2077 696e  ak Condorcet win
+000064d0: 6e65 7273 2061 7265 2053 706c 6974 2043  ners are Split C
+000064e0: 7963 6c65 2077 696e 6e65 7273 0a20 2020  ycle winners.   
+000064f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006500: 2066 6f72 206b 5f69 6478 2c20 6b20 696e   for k_idx, k in
+00006510: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+00006520: 6461 7465 7329 3a20 0a20 2020 2020 2020  dates): .       
+00006530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006540: 2069 6620 6920 213d 206b 2061 6e64 206a   if i != k and j
+00006550: 2021 3d20 6b3a 0a20 2020 2020 2020 2020   != k:.         
+00006560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006570: 2020 2073 7472 656e 6774 685b 6a5f 6964     strength[j_id
+00006580: 785d 5b6b 5f69 6478 5d20 3d20 6d61 7828  x][k_idx] = max(
+00006590: 7374 7265 6e67 7468 5b6a 5f69 6478 5d5b  strength[j_idx][
+000065a0: 6b5f 6964 785d 2c20 6d69 6e28 7374 7265  k_idx], min(stre
+000065b0: 6e67 7468 5b6a 5f69 6478 5d5b 695f 6964  ngth[j_idx][i_id
+000065c0: 785d 2c73 7472 656e 6774 685b 695f 6964  x],strength[i_id
+000065d0: 785d 5b6b 5f69 6478 5d29 290a 200a 2020  x][k_idx])). .  
+000065e0: 2020 6465 6665 6174 5f67 7261 7068 203d    defeat_graph =
+000065f0: 206e 782e 4469 4772 6170 6828 290a 2020   nx.DiGraph().  
+00006600: 2020 6465 6665 6174 5f67 7261 7068 2e61    defeat_graph.a
+00006610: 6464 5f6e 6f64 6573 5f66 726f 6d28 6361  dd_nodes_from(ca
+00006620: 6e64 6964 6174 6573 290a 0a20 2020 2066  ndidates)..    f
+00006630: 6f72 2069 5f69 6478 2c20 6920 696e 2065  or i_idx, i in e
+00006640: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+00006650: 7465 7329 3a0a 2020 2020 2020 2020 666f  tes):.        fo
+00006660: 7220 6a5f 6964 782c 206a 2069 6e20 656e  r j_idx, j in en
+00006670: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+00006680: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+00006690: 2069 6620 6920 213d 206a 3a0a 2020 2020   if i != j:.    
+000066a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+000066b0: 5f6d 6174 7269 785b 6a5f 6964 785d 5b69  _matrix[j_idx][i
+000066c0: 5f69 6478 5d20 3e20 7374 7265 6e67 7468  _idx] > strength
+000066d0: 5b69 5f69 6478 5d5b 6a5f 6964 785d 3a20  [i_idx][j_idx]: 
+000066e0: 2320 7468 6520 6d61 696e 2064 6966 6665  # the main diffe
+000066f0: 7265 6e63 6520 7769 7468 2042 6561 7420  rence with Beat 
+00006700: 5061 7468 0a20 2020 2020 2020 2020 2020  Path.           
+00006710: 2020 2020 2020 2020 2064 6566 6561 745f           defeat_
+00006720: 6772 6170 682e 6164 645f 7765 6967 6874  graph.add_weight
+00006730: 6564 5f65 6467 6573 5f66 726f 6d28 5b28  ed_edges_from([(
+00006740: 6a2c 692c 735f 6d61 7472 6978 5b6a 5f69  j,i,s_matrix[j_i
+00006750: 6478 5d5b 695f 6964 785d 295d 290a 2020  dx][i_idx])]).  
+00006760: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+00006770: 2020 2072 6574 7572 6e20 6465 6665 6174     return defeat
+00006780: 5f67 7261 7068 0a0a 0a23 2066 6c61 7474  _graph...# flatt
+00006790: 656e 2061 2032 6420 6c69 7374 202d 2074  en a 2d list - t
+000067a0: 7572 6e20 6120 3264 206c 6973 7420 696e  urn a 2d list in
+000067b0: 746f 2061 2073 696e 676c 6520 6c69 7374  to a single list
+000067c0: 206f 6620 6974 656d 730a 666c 6174 7465   of items.flatte
+000067d0: 6e20 3d20 6c61 6d62 6461 206c 3a20 5b69  n = lambda l: [i
+000067e0: 7465 6d20 666f 7220 7375 626c 6973 7420  tem for sublist 
+000067f0: 696e 206c 2066 6f72 2069 7465 6d20 696e  in l for item in
+00006800: 2073 7562 6c69 7374 5d0a 0a64 6566 2064   sublist]..def d
+00006810: 6f65 735f 6372 6561 7465 5f63 7963 6c65  oes_create_cycle
+00006820: 2867 2c20 6564 6765 293a 0a20 2020 2027  (g, edge):.    '
+00006830: 2727 7265 7475 726e 2054 7275 6520 6966  ''return True if
+00006840: 2061 6464 696e 6720 7468 6520 6564 6765   adding the edge
+00006850: 2074 6f20 6720 6372 6561 7465 2061 2063   to g create a c
+00006860: 7963 6c65 2e0a 2020 2020 6974 2069 7320  ycle..    it is 
+00006870: 6173 7375 6d65 6420 7468 6174 2065 6467  assumed that edg
+00006880: 6520 6973 2061 6c72 6561 6479 2069 6e20  e is already in 
+00006890: 6727 2727 0a20 2020 2073 6f75 7263 6520  g'''.    source 
+000068a0: 3d20 6564 6765 5b30 5d0a 2020 2020 7461  = edge[0].    ta
+000068b0: 7267 6574 203d 2065 6467 655b 315d 0a20  rget = edge[1]. 
+000068c0: 2020 2066 6f72 206e 2069 6e20 672e 7072     for n in g.pr
+000068d0: 6564 6563 6573 736f 7273 2873 6f75 7263  edecessors(sourc
+000068e0: 6529 3a0a 2020 2020 2020 2020 6966 206e  e):.        if n
+000068f0: 782e 6861 735f 7061 7468 2867 2c20 7461  x.has_path(g, ta
+00006900: 7267 6574 2c20 6e29 3a20 0a20 2020 2020  rget, n): .     
+00006910: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00006920: 7565 0a20 2020 2072 6574 7572 6e20 4661  ue.    return Fa
+00006930: 6c73 650a 0a0a 0a64 6566 2070 6f77 6572  lse....def power
+00006940: 7365 7428 6974 6572 6162 6c65 293a 0a20  set(iterable):. 
+00006950: 2020 2022 2222 0a20 2020 2052 6574 7572     """.    Retur
+00006960: 6e20 7468 6520 706f 7765 7273 6574 206f  n the powerset o
+00006970: 6620 6060 6974 6572 6162 6c65 6060 0a0a  f ``iterable``..
+00006980: 2020 2020 706f 7765 7273 6574 285b 312c      powerset([1,
+00006990: 322c 335d 2920 2d2d 3e20 2829 2028 312c  2,3]) --> () (1,
+000069a0: 2920 2832 2c29 2028 332c 2920 2831 2c32  ) (2,) (3,) (1,2
+000069b0: 2920 2831 2c33 2920 2832 2c33 2920 2831  ) (1,3) (2,3) (1
+000069c0: 2c32 2c33 290a 2020 2020 2222 220a 2020  ,2,3).    """.  
+000069d0: 2020 7320 3d20 6c69 7374 2869 7465 7261    s = list(itera
+000069e0: 626c 6529 0a20 2020 2072 6574 7572 6e20  ble).    return 
+000069f0: 6368 6169 6e2e 6672 6f6d 5f69 7465 7261  chain.from_itera
+00006a00: 626c 6528 636f 6d62 696e 6174 696f 6e73  ble(combinations
+00006a10: 2873 2c20 7229 2066 6f72 2072 2069 6e20  (s, r) for r in 
+00006a20: 7261 6e67 6528 6c65 6e28 7329 2b31 2929  range(len(s)+1))
+00006a30: 0a0a 0a64 6566 2069 735f 7374 6163 6b28  ...def is_stack(
+00006a40: 6564 6174 612c 2063 616e 645f 6c69 7374  edata, cand_list
+00006a50: 2c20 6375 7272 5f63 616e 6473 3d4e 6f6e  , curr_cands=Non
+00006a60: 6529 3a20 0a20 2020 2022 2222 0a20 2020  e): .    """.   
+00006a70: 2041 202a 2a73 7461 636b 2a2a 2069 7320   A **stack** is 
+00006a80: 6120 6c69 6e65 6172 206f 7264 6572 203a  a linear order :
+00006a90: 6d61 7468 3a60 4c60 206f 6e20 7468 6520  math:`L` on the 
+00006aa0: 6361 6e64 6964 6174 6520 7375 6368 2074  candidate such t
+00006ab0: 6861 7420 666f 7220 616c 6c20 6361 6e64  hat for all cand
+00006ac0: 6964 6174 6573 203a 6d61 7468 3a60 6160  idates :math:`a`
+00006ad0: 2061 6e64 203a 6d61 7468 3a60 6260 2c20   and :math:`b`, 
+00006ae0: 6966 203a 6d61 7468 3a60 614c 6260 2c20  if :math:`aLb`, 
+00006af0: 7468 656e 2074 6865 7265 2061 7265 2064  then there are d
+00006b00: 6973 7469 6e63 7420 6361 6e64 6964 6174  istinct candidat
+00006b10: 6573 203a 6d61 7468 3a60 785f 312c 5c64  es :math:`x_1,\d
+00006b20: 6f74 732c 785f 6e60 2077 6974 6820 3a6d  ots,x_n` with :m
+00006b30: 6174 683a 6078 5f31 3d61 6020 616e 6420  ath:`x_1=a` and 
+00006b40: 3a6d 6174 683a 6078 5f6e 3d62 6020 7375  :math:`x_n=b` su
+00006b50: 6368 2074 6861 7420 3a6d 6174 683a 6078  ch that :math:`x
+00006b60: 5f69 204c 2078 5f7b 692b 317d 6020 616e  _i L x_{i+1}` an
+00006b70: 6420 666f 7220 616c 6c20 3a6d 6174 683a  d for all :math:
+00006b80: 6069 5c69 6e20 5c7b 312c 5c64 6f74 732c  `i\in \{1,\dots,
+00006b90: 206e 2d31 5c7d 602c 2074 6865 206d 6172   n-1\}`, the mar
+00006ba0: 6769 6e20 6f66 203a 6d61 7468 3a60 785f  gin of :math:`x_
+00006bb0: 3160 206f 7665 7220 3a6d 6174 683a 6078  1` over :math:`x
+00006bc0: 5f7b 692b 317d 6020 6973 2067 7265 6174  _{i+1}` is great
+00006bd0: 6572 2074 6861 6e20 6f72 2065 7175 616c  er than or equal
+00006be0: 2074 6f20 7468 6520 6d61 7267 696e 206f   to the margin o
+00006bf0: 6620 3a6d 6174 683a 6062 6020 6f76 6572  f :math:`b` over
+00006c00: 203a 6d61 7468 3a60 6160 2e0a 0a20 2020   :math:`a`...   
+00006c10: 2054 6869 7320 6465 6669 6e69 7469 6f6e   This definition
+00006c20: 2069 7320 6475 6520 746f 205a 6176 6973   is due to Zavis
+00006c30: 7420 616e 6420 5469 6465 6d61 6e20 3139  t and Tideman 19
+00006c40: 3839 2c20 616e 6420 6973 2075 7365 6420  89, and is used 
+00006c50: 6173 2061 6e20 616c 7465 726e 6174 6976  as an alternativ
+00006c60: 6520 6368 6172 6163 7465 7269 7a61 7469  e characterizati
+00006c70: 6f6e 206f 6620 5261 6e6b 6564 2050 6169  on of Ranked Pai
+00006c80: 7273 3a20 3a6d 6174 683a 6061 6020 6973  rs: :math:`a` is
+00006c90: 2061 2052 616e 6b65 6420 5061 6972 7320   a Ranked Pairs 
+00006ca0: 7769 6e6e 6572 2069 6620 616e 6420 6f6e  winner if and on
+00006cb0: 6c79 2069 6620 3a6d 6174 683a 6061 6020  ly if :math:`a` 
+00006cc0: 6973 2074 6865 206d 6178 696d 756d 2065  is the maximum e
+00006cd0: 6c65 6d65 6e74 206f 6620 736f 6d65 2073  lement of some s
+00006ce0: 7461 636b 2e20 0a0a 2020 2020 4172 6773  tack. ..    Args
+00006cf0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+00006d00: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+00006d10: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+00006d20: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+00006d30: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+00006d40: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+00006d50: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+00006d60: 6361 6e64 5f6c 6973 7420 286c 6973 7429  cand_list (list)
+00006d70: 3a20 5468 6520 6c69 7374 206f 6620 6361  : The list of ca
+00006d80: 6e64 6964 6174 6573 2074 6861 7420 6d61  ndidates that ma
+00006d90: 7920 6265 2061 2073 7461 636b 0a20 2020  y be a stack.   
+00006da0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+00006db0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+00006dc0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+00006dd0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+00006de0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+00006df0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00006e00: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00006e10: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00006e20: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
+00006e30: 3a20 0a20 2020 2020 2020 2054 7275 6520  : .        True 
+00006e40: 6966 2060 6063 616e 645f 6c69 7374 6060  if ``cand_list``
+00006e50: 2069 7320 6120 7374 6163 6b20 616e 6420   is a stack and 
+00006e60: 4661 6c73 6520 6f74 6865 7277 6973 650a  False otherwise.
+00006e70: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
+00006e80: 2020 2020 0a20 2020 202e 2e20 706c 6f74      .    .. plot
+00006e90: 3a3a 2020 6d61 7267 696e 5f67 7261 7068  ::  margin_graph
+00006ea0: 735f 6578 616d 706c 6573 2f6d 675f 6578  s_examples/mg_ex
+00006eb0: 5f72 705f 7374 6163 6b73 2e70 790a 2020  _rp_stacks.py.  
+00006ec0: 2020 2020 2020 3a63 6f6e 7465 7874 3a20        :context: 
+00006ed0: 7265 7365 7420 200a 2020 2020 2020 2020  reset  .        
+00006ee0: 3a69 6e63 6c75 6465 2d73 6f75 7263 653a  :include-source:
+00006ef0: 2054 7275 650a 0a0a 2020 2020 2e2e 2065   True...    .. e
+00006f00: 7865 635f 636f 6465 3a3a 0a20 2020 2020  xec_code::.     
+00006f10: 2020 200a 2020 2020 2020 2020 6672 6f6d     .        from
+00006f20: 2070 7265 665f 766f 7469 6e67 2e77 6569   pref_voting.wei
+00006f30: 6768 7465 645f 6d61 6a6f 7269 7479 5f67  ghted_majority_g
+00006f40: 7261 7068 7320 696d 706f 7274 204d 6172  raphs import Mar
+00006f50: 6769 6e47 7261 7068 0a20 2020 2020 2020  ginGraph.       
+00006f60: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+00006f70: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00006f80: 6574 686f 6473 2069 6d70 6f72 7420 6973  ethods import is
+00006f90: 5f73 7461 636b 0a20 2020 2020 2020 2066  _stack.        f
+00006fa0: 726f 6d20 6974 6572 746f 6f6c 7320 696d  rom itertools im
+00006fb0: 706f 7274 2070 6572 6d75 7461 7469 6f6e  port permutation
+00006fc0: 730a 2020 2020 2020 2020 0a20 2020 2020  s.        .     
+00006fd0: 2020 206d 6720 3d20 4d61 7267 696e 4772     mg = MarginGr
+00006fe0: 6170 6828 5b30 2c20 312c 2032 5d2c 205b  aph([0, 1, 2], [
+00006ff0: 2830 2c20 312c 2032 292c 2028 312c 2032  (0, 1, 2), (1, 2
+00007000: 2c20 3429 2c20 2832 2c20 302c 2032 295d  , 4), (2, 0, 2)]
+00007010: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+00007020: 2020 2066 6f72 2063 6c69 7374 2069 6e20     for clist in 
+00007030: 7065 726d 7574 6174 696f 6e73 286d 672e  permutations(mg.
+00007040: 6361 6e64 6964 6174 6573 293a 200a 2020  candidates): .  
+00007050: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00007060: 6622 7b63 6c69 7374 7d20 7b27 6973 2720  f"{clist} {'is' 
+00007070: 6966 2069 735f 7374 6163 6b28 6d67 2c20  if is_stack(mg, 
+00007080: 636c 6973 7429 2065 6c73 6520 2769 7320  clist) else 'is 
+00007090: 6e6f 7427 7d20 6120 7374 6163 6b22 290a  not'} a stack").
+000070a0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+000070b0: 2022 2222 0a20 2020 200a 2020 2020 6361   """.    .    ca
+000070c0: 6e64 6964 6174 6573 203d 2063 7572 725f  ndidates = curr_
+000070d0: 6361 6e64 7320 6966 2063 7572 725f 6361  cands if curr_ca
+000070e0: 6e64 7320 6973 206e 6f74 204e 6f6e 6520  nds is not None 
+000070f0: 656c 7365 2065 6461 7461 2e63 616e 6469  else edata.candi
+00007100: 6461 7465 730a 2020 2020 6361 6e64 5f70  dates.    cand_p
+00007110: 6169 7273 203d 205b 2861 2c20 6229 2069  airs = [(a, b) i
+00007120: 6620 6361 6e64 5f6c 6973 742e 696e 6465  f cand_list.inde
+00007130: 7828 6129 203c 2063 616e 645f 6c69 7374  x(a) < cand_list
+00007140: 2e69 6e64 6578 2862 2920 656c 7365 2028  .index(b) else (
+00007150: 622c 2061 2920 666f 7220 612c 2062 2069  b, a) for a, b i
+00007160: 6e20 636f 6d62 696e 6174 696f 6e73 2863  n combinations(c
+00007170: 616e 6469 6461 7465 732c 2032 295d 0a20  andidates, 2)]. 
+00007180: 2020 2020 2020 200a 2020 2020 666f 7220         .    for 
+00007190: 612c 2062 2069 6e20 6361 6e64 5f70 6169  a, b in cand_pai
+000071a0: 7273 3a0a 2020 2020 2020 2020 6f74 6865  rs:.        othe
+000071b0: 725f 6361 6e64 7320 3d20 5b63 2066 6f72  r_cands = [c for
+000071c0: 2063 2069 6e20 6361 6e64 6964 6174 6573   c in candidates
+000071d0: 2069 6620 6320 213d 2061 2061 6e64 2063   if c != a and c
+000071e0: 2021 3d20 625d 0a20 2020 2020 2020 2066   != b].        f
+000071f0: 6f75 6e64 5f70 6174 6820 3d20 4661 6c73  ound_path = Fals
+00007200: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
+00007210: 2020 2073 7562 6c69 7374 203d 2063 616e     sublist = can
+00007220: 645f 6c69 7374 5b63 616e 645f 6c69 7374  d_list[cand_list
+00007230: 2e69 6e64 6578 2861 2920 2b20 313a 6361  .index(a) + 1:ca
+00007240: 6e64 5f6c 6973 742e 696e 6465 7828 6229  nd_list.index(b)
+00007250: 5d0a 2020 2020 2020 2020 0a20 2020 2020  ].        .     
+00007260: 2020 2066 6f72 2069 6e64 6963 6573 2069     for indices i
+00007270: 6e20 706f 7765 7273 6574 2872 616e 6765  n powerset(range
+00007280: 286c 656e 2873 7562 6c69 7374 2929 293a  (len(sublist))):
+00007290: 200a 2020 2020 2020 2020 2020 2020 0a20   .            . 
+000072a0: 2020 2020 2020 2020 2020 2070 6174 6820             path 
+000072b0: 3d20 5b61 5d20 2b20 5b73 7562 6c69 7374  = [a] + [sublist
+000072c0: 5b69 5d20 666f 7220 6920 696e 2073 6f72  [i] for i in sor
+000072d0: 7465 6428 696e 6469 6365 7329 5d20 2b20  ted(indices)] + 
+000072e0: 5b62 5d0a 2020 2020 2020 2020 2020 2020  [b].            
+000072f0: 6d61 7267 696e 7320 3d20 5b65 6461 7461  margins = [edata
+00007300: 2e6d 6172 6769 6e28 7869 2c20 7061 7468  .margin(xi, path
+00007310: 5b69 202b 2031 5d29 2066 6f72 2069 2c20  [i + 1]) for i, 
+00007320: 7869 2069 6e20 656e 756d 6572 6174 6528  xi in enumerate(
+00007330: 7061 7468 5b30 3a2d 315d 295d 0a20 2020  path[0:-1])].   
+00007340: 2020 2020 2020 2020 2069 6620 616c 6c28           if all(
+00007350: 5b63 616e 645f 6c69 7374 2e69 6e64 6578  [cand_list.index
+00007360: 2878 6929 203c 2063 616e 645f 6c69 7374  (xi) < cand_list
+00007370: 2e69 6e64 6578 2870 6174 685b 692b 315d  .index(path[i+1]
+00007380: 2920 666f 7220 692c 2078 6920 696e 2065  ) for i, xi in e
+00007390: 6e75 6d65 7261 7465 2870 6174 685b 303a  numerate(path[0:
+000073a0: 2d31 5d29 5d29 2061 6e64 2061 6c6c 285b  -1])]) and all([
+000073b0: 6d20 3e3d 2065 6461 7461 2e6d 6172 6769  m >= edata.margi
+000073c0: 6e28 622c 2061 2920 666f 7220 6d20 696e  n(b, a) for m in
+000073d0: 206d 6172 6769 6e73 5d29 3a20 0a20 2020   margins]): .   
+000073e0: 2020 2020 2020 2020 2020 2020 2066 6f75               fou
+000073f0: 6e64 5f70 6174 6820 3d20 5472 7565 0a20  nd_path = True. 
+00007400: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00007410: 7265 616b 0a20 2020 2020 2020 2069 6620  reak.        if 
+00007420: 6e6f 7420 666f 756e 645f 7061 7468 3a20  not found_path: 
+00007430: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00007440: 7572 6e20 4661 6c73 650a 2020 2020 7265  urn False.    re
+00007450: 7475 726e 2054 7275 650a 0a64 6566 205f  turn True..def _
+00007460: 7261 6e6b 6564 5f70 6169 7273 5f66 726f  ranked_pairs_fro
+00007470: 6d5f 7374 6163 6b73 2865 6461 7461 2c20  m_stacks(edata, 
+00007480: 6375 7272 5f63 616e 6473 203d 204e 6f6e  curr_cands = Non
+00007490: 6529 3a20 0a20 2020 2022 2222 4669 6e64  e): .    """Find
+000074a0: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
+000074b0: 7320 7769 6e6e 6572 7320 6279 2069 7465  s winners by ite
+000074c0: 7261 7469 6e67 206f 7665 7220 616c 6c20  rating over all 
+000074d0: 7065 726d 7574 6174 696f 6e73 206f 6620  permutations of 
+000074e0: 6361 6e64 6964 6174 6573 2028 7265 7374  candidates (rest
+000074f0: 7269 6374 6564 2074 6f20 6060 6375 7272  ricted to ``curr
+00007500: 5f63 616e 6473 6060 2069 6620 6e6f 7420  _cands`` if not 
+00007510: 4e6f 6e65 292c 2061 6e64 2063 6865 636b  None), and check
+00007520: 696e 6720 6966 2074 6865 206c 6973 7420  ing if the list 
+00007530: 6973 2061 2073 7461 636b 2e20 0a0a 2020  is a stack. ..  
+00007540: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00007550: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00007560: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00007570: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+00007580: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+00007590: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+000075a0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+000075b0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+000075c0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+000075d0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+000075e0: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+000075f0: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+00007600: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+00007610: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+00007620: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00007630: 6473 6060 0a0a 2020 2020 5265 7475 726e  ds``..    Return
+00007640: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+00007650: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+00007660: 6469 6461 7465 732e 200a 0a20 2020 202e  didates. ..    .
+00007670: 2e20 7365 6561 6c73 6f3a 3a0a 2020 2020  . seealso::.    
+00007680: 2020 2020 0a20 2020 2020 2020 203a 6d65      .        :me
+00007690: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+000076a0: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+000076b0: 686f 6473 2e69 735f 7374 6163 6b60 0a0a  hods.is_stack`..
+000076c0: 0a20 2020 2022 2222 2020 2020 0a0a 2020  .    """    ..  
+000076d0: 2020 6361 6e64 6964 6174 6573 203d 2063    candidates = c
+000076e0: 7572 725f 6361 6e64 7320 6966 2063 7572  urr_cands if cur
+000076f0: 725f 6361 6e64 7320 6973 206e 6f74 204e  r_cands is not N
+00007700: 6f6e 6520 656c 7365 2065 6461 7461 2e63  one else edata.c
+00007710: 616e 6469 6461 7465 730a 2020 2020 7769  andidates.    wi
+00007720: 6e6e 6572 7320 3d20 6c69 7374 2829 0a20  nners = list(). 
+00007730: 2020 2066 6f72 2063 6c69 7374 2069 6e20     for clist in 
+00007740: 7065 726d 7574 6174 696f 6e73 2863 616e  permutations(can
+00007750: 6469 6461 7465 7329 3a20 0a20 2020 2020  didates): .     
+00007760: 2020 2069 7373 7461 636b 203d 2069 735f     isstack = is_
+00007770: 7374 6163 6b28 6564 6174 612c 2063 6c69  stack(edata, cli
+00007780: 7374 2c20 6375 7272 5f63 616e 6473 203d  st, curr_cands =
+00007790: 2063 7572 725f 6361 6e64 7329 0a20 2020   curr_cands).   
+000077a0: 2020 2020 2069 6620 6973 7374 6163 6b3a       if isstack:
+000077b0: 200a 2020 2020 2020 2020 2020 2020 7769   .            wi
+000077c0: 6e6e 6572 732e 6170 7065 6e64 2863 6c69  nners.append(cli
+000077d0: 7374 5b30 5d29 0a20 2020 2020 2020 2020  st[0]).         
+000077e0: 2020 200a 2020 2020 7265 7475 726e 2073     .    return s
+000077f0: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
+00007800: 696e 6e65 7273 2929 290a 0a64 6566 205f  inners)))..def _
+00007810: 7261 6e6b 6564 5f70 6169 7273 5f62 6173  ranked_pairs_bas
+00007820: 6963 280a 2020 2020 6564 6174 612c 200a  ic(.    edata, .
+00007830: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
+00007840: 204e 6f6e 652c 200a 2020 2020 7374 7265   None, .    stre
+00007850: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00007860: 4e6f 6e65 293a 2020 200a 2020 2020 2222  None):   .    ""
+00007870: 2241 6e20 696d 706c 656d 656e 7461 7469  "An implementati
+00007880: 6f6e 206f 6620 5261 6e6b 6564 2050 6169  on of Ranked Pai
+00007890: 7273 2074 6861 7420 7573 6573 2061 2062  rs that uses a b
+000078a0: 6173 6963 2061 6c67 6f72 6974 686d 2e20  asic algorithm. 
+000078b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000078c0: 2020 2020 6564 6174 6120 2850 726f 6669      edata (Profi
+000078d0: 6c65 2c20 5072 6f66 696c 6557 6974 6854  le, ProfileWithT
+000078e0: 6965 732c 204d 6172 6769 6e47 7261 7068  ies, MarginGraph
+000078f0: 293a 2041 6e79 2065 6c65 6374 696f 6e20  ): Any election 
+00007900: 6461 7461 2074 6861 7420 6861 7320 6120  data that has a 
+00007910: 606d 6172 6769 6e60 206d 6574 686f 642e  `margin` method.
+00007920: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
+00007930: 616e 6473 2028 4c69 7374 5b69 6e74 5d2c  ands (List[int],
+00007940: 206f 7074 696f 6e61 6c29 3a20 4966 2073   optional): If s
+00007950: 6574 2c20 7468 656e 2066 696e 6420 7468  et, then find th
+00007960: 6520 7769 6e6e 6572 7320 666f 7220 7468  e winners for th
+00007970: 6520 7072 6f66 696c 6520 7265 7374 7269  e profile restri
+00007980: 6374 6564 2074 6f20 7468 6520 6361 6e64  cted to the cand
+00007990: 6964 6174 6573 2069 6e20 6060 6375 7272  idates in ``curr
+000079a0: 5f63 616e 6473 6060 0a0a 2020 2020 5265  _cands``..    Re
+000079b0: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
+000079c0: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
+000079d0: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
+000079e0: 2020 2022 2222 0a20 2020 2063 616e 6469     """.    candi
+000079f0: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+00007a00: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00007a10: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+00007a20: 6c73 6520 6375 7272 5f63 616e 6473 200a  lse curr_cands .
+00007a30: 2020 2020 6369 6478 5f74 6f5f 6361 6e64      cidx_to_cand
+00007a40: 203d 207b 6369 6478 3a20 6320 666f 7220   = {cidx: c for 
+00007a50: 6369 6478 2c20 6320 696e 2065 6e75 6d65  cidx, c in enume
+00007a60: 7261 7465 2863 616e 6469 6461 7465 7329  rate(candidates)
+00007a70: 7d20 200a 2020 2020 6361 6e64 5f74 6f5f  }  .    cand_to_
+00007a80: 6369 6478 203d 207b 633a 2063 6964 7820  cidx = {c: cidx 
+00007a90: 666f 7220 6369 6478 2c20 6320 696e 2065  for cidx, c in e
+00007aa0: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+00007ab0: 7465 7329 7d20 200a 2020 2020 7374 7265  tes)}  .    stre
+00007ac0: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00007ad0: 6564 6174 612e 6d61 7267 696e 2069 6620  edata.margin if 
+00007ae0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00007af0: 6e20 6973 204e 6f6e 6520 656c 7365 2073  n is None else s
+00007b00: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00007b10: 2020 2020 0a0a 2020 2020 6377 203d 2065      ..    cw = e
+00007b20: 6461 7461 2e63 6f6e 646f 7263 6574 5f77  data.condorcet_w
+00007b30: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
+00007b40: 3d63 7572 725f 6361 6e64 7329 0a20 2020  =curr_cands).   
+00007b50: 2023 2052 616e 6b65 6420 5061 6972 7320   # Ranked Pairs 
+00007b60: 6973 2043 6f6e 646f 7263 6574 2063 6f6e  is Condorcet con
+00007b70: 7369 7374 656e 742c 2073 6f20 7369 6d70  sistent, so simp
+00007b80: 6c79 2072 6574 7572 6e20 7468 6520 436f  ly return the Co
+00007b90: 6e64 6f72 6365 7420 7769 6e6e 6572 2069  ndorcet winner i
+00007ba0: 6620 6578 6973 7473 0a20 2020 2069 6620  f exists.    if 
+00007bb0: 6377 2069 7320 6e6f 7420 4e6f 6e65 3a20  cw is not None: 
+00007bc0: 0a20 2020 2020 2020 2077 696e 6e65 7273  .        winners
+00007bd0: 203d 205b 6377 5d0a 2020 2020 656c 7365   = [cw].    else
+00007be0: 3a0a 2020 2020 2020 2020 775f 6564 6765  :.        w_edge
+00007bf0: 7320 3d20 5b28 6331 2c20 6332 2c20 7374  s = [(c1, c2, st
+00007c00: 7265 6e67 7468 5f66 756e 6374 696f 6e28  rength_function(
+00007c10: 6331 2c20 6332 2929 2066 6f72 2063 3120  c1, c2)) for c1 
+00007c20: 696e 2063 616e 6469 6461 7465 7320 666f  in candidates fo
+00007c30: 7220 6332 2069 6e20 6361 6e64 6964 6174  r c2 in candidat
+00007c40: 6573 200a 2020 2020 2020 2020 2020 2020  es .            
+00007c50: 2020 2020 2020 2069 6620 6331 2021 3d20         if c1 != 
+00007c60: 6332 2061 6e64 2028 6564 6174 612e 6d61  c2 and (edata.ma
+00007c70: 6a6f 7269 7479 5f70 7265 6665 7273 2863  jority_prefers(c
+00007c80: 312c 2063 3229 206f 7220 6564 6174 612e  1, c2) or edata.
+00007c90: 6973 5f74 6965 6428 6331 2c20 6332 2929  is_tied(c1, c2))
+00007ca0: 5d0a 2020 2020 2020 2020 7769 6e6e 6572  ].        winner
+00007cb0: 7320 3d20 6c69 7374 2829 2020 200a 2020  s = list()   .  
+00007cc0: 2020 2020 2020 6966 206c 656e 2877 5f65        if len(w_e
+00007cd0: 6467 6573 2920 3e20 303a 2020 2020 2020  dges) > 0:      
+00007ce0: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00007cf0: 2073 7472 656e 6774 6873 203d 2073 6f72   strengths = sor
+00007d00: 7465 6428 6c69 7374 2873 6574 285b 655b  ted(list(set([e[
+00007d10: 325d 2066 6f72 2065 2069 6e20 775f 6564  2] for e in w_ed
+00007d20: 6765 735d 2929 2c20 7265 7665 7273 653d  ges])), reverse=
+00007d30: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00007d40: 2020 736f 7274 6564 5f65 6467 6573 203d    sorted_edges =
+00007d50: 205b 5b65 2066 6f72 2065 2069 6e20 775f   [[e for e in w_
+00007d60: 6564 6765 7320 6966 2065 5b32 5d20 3d3d  edges if e[2] ==
+00007d70: 2073 5d20 666f 7220 7320 696e 2073 7472   s] for s in str
+00007d80: 656e 6774 6873 5d0a 2020 2020 2020 2020  engths].        
+00007d90: 2020 2020 7462 7320 3d20 7072 6f64 7563      tbs = produc
+00007da0: 7428 2a5b 7065 726d 7574 6174 696f 6e73  t(*[permutations
+00007db0: 2865 6467 6573 2920 666f 7220 6564 6765  (edges) for edge
+00007dc0: 7320 696e 2073 6f72 7465 645f 6564 6765  s in sorted_edge
+00007dd0: 735d 290a 2020 2020 2020 2020 2020 2020  s]).            
+00007de0: 666f 7220 7462 2069 6e20 7462 733a 0a20  for tb in tbs:. 
+00007df0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00007e00: 6467 6573 203d 2066 6c61 7474 656e 2874  dges = flatten(t
+00007e10: 6229 0a20 2020 2020 2020 2020 2020 2020  b).             
+00007e20: 2020 2072 705f 6465 6665 6174 203d 2053     rp_defeat = S
+00007e30: 504f 286c 656e 2863 616e 6469 6461 7465  PO(len(candidate
+00007e40: 7329 290a 2020 2020 2020 2020 2020 2020  s)).            
+00007e50: 2020 2020 666f 7220 6530 2c65 312c 7320      for e0,e1,s 
+00007e60: 696e 2065 6467 6573 3a20 0a20 2020 2020  in edges: .     
+00007e70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00007e80: 6620 6e6f 7420 7270 5f64 6566 6561 742e  f not rp_defeat.
+00007e90: 505b 6361 6e64 5f74 6f5f 6369 6478 5b65  P[cand_to_cidx[e
+00007ea0: 315d 5d5b 6361 6e64 5f74 6f5f 6369 6478  1]][cand_to_cidx
+00007eb0: 5b65 305d 5d3a 0a20 2020 2020 2020 2020  [e0]]:.         
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007ed0: 705f 6465 6665 6174 2e61 6464 2863 616e  p_defeat.add(can
+00007ee0: 645f 746f 5f63 6964 785b 6530 5d2c 6361  d_to_cidx[e0],ca
+00007ef0: 6e64 5f74 6f5f 6369 6478 5b65 315d 290a  nd_to_cidx[e1]).
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 7769 6e6e 6572 732e 6170 7065 6e64 2863  winners.append(c
+00007f20: 6964 785f 746f 5f63 616e 645b 7270 5f64  idx_to_cand[rp_d
+00007f30: 6566 6561 742e 696e 6974 6961 6c5f 656c  efeat.initial_el
+00007f40: 656d 656e 7473 2829 5b30 5d5d 290a 2020  ements()[0]]).  
+00007f50: 2020 2020 2020 656c 7365 3a20 0a20 2020        else: .   
+00007f60: 2020 2020 2020 2020 2077 696e 6e65 7273           winners
+00007f70: 203d 2063 616e 6469 6461 7465 730a 2020   = candidates.  
+00007f80: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
+00007f90: 6c69 7374 2873 6574 2877 696e 6e65 7273  list(set(winners
+00007fa0: 2929 290a 0a0a 4076 6d28 6e61 6d65 3d22  )))...@vm(name="
+00007fb0: 5261 6e6b 6564 2050 6169 7273 222c 0a20  Ranked Pairs",. 
+00007fc0: 2020 2069 6e70 7574 5f74 7970 6573 3d5b     input_types=[
+00007fd0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+00007fe0: 4f46 494c 452c 2045 6c65 6374 696f 6e54  OFILE, ElectionT
+00007ff0: 7970 6573 2e50 524f 4649 4c45 5f57 4954  ypes.PROFILE_WIT
+00008000: 485f 5449 4553 2c20 456c 6563 7469 6f6e  H_TIES, Election
+00008010: 5479 7065 732e 4d41 5247 494e 5f47 5241  Types.MARGIN_GRA
+00008020: 5048 5d29 0a64 6566 2072 616e 6b65 645f  PH]).def ranked_
+00008030: 7061 6972 7328 0a20 2020 2065 6461 7461  pairs(.    edata
+00008040: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
+00008050: 733d 4e6f 6e65 2c20 0a20 2020 2073 7472  s=None, .    str
+00008060: 656e 6774 685f 6675 6e63 7469 6f6e 3d4e  ength_function=N
+00008070: 6f6e 652c 200a 2020 2020 616c 676f 7269  one, .    algori
+00008080: 7468 6d3d 2762 6173 6963 2729 3a20 2020  thm='basic'):   
+00008090: 0a20 2020 2022 2222 0a20 2020 204f 7264  .    """.    Ord
+000080a0: 6572 2074 6865 2065 6467 6573 2069 6e20  er the edges in 
+000080b0: 7468 6520 6d61 7267 696e 2067 7261 7068  the margin graph
+000080c0: 2066 726f 6d20 6c61 7267 6573 7420 746f   from largest to
+000080d0: 2073 6d61 6c6c 6573 7420 616e 6420 6c6f   smallest and lo
+000080e0: 636b 2074 6865 6d20 696e 2069 6e20 7468  ck them in in th
+000080f0: 6174 206f 7264 6572 2c20 736b 6970 7069  at order, skippi
+00008100: 6e67 2065 6467 6573 2074 6861 7420 6372  ng edges that cr
+00008110: 6561 7465 2061 2063 7963 6c65 2e20 2049  eate a cycle.  I
+00008120: 6620 7468 6572 6520 6172 6520 7469 6573  f there are ties
+00008130: 2069 6e20 7468 6520 6d61 7267 696e 732c   in the margins,
+00008140: 2062 7265 616b 2074 6865 2074 6965 7320   break the ties 
+00008150: 7573 696e 6720 6120 7469 652d 6272 6561  using a tie-brea
+00008160: 6b69 6e67 2072 756c 653a 2061 206c 696e  king rule: a lin
+00008170: 6561 7220 6f72 6465 7269 6e67 206f 7665  ear ordering ove
+00008180: 7220 7468 6520 6564 6765 732e 2020 2041  r the edges.   A
+00008190: 2063 616e 6469 6461 7465 2069 7320 6120   candidate is a 
+000081a0: 5261 6e6b 6564 2050 6169 7273 2077 696e  Ranked Pairs win
+000081b0: 6e65 7220 6966 2069 7420 7769 6e73 2061  ner if it wins a
+000081c0: 6363 6f72 6469 6e67 2074 6f20 736f 6d65  ccording to some
+000081d0: 2074 6965 2d62 7265 616b 696e 6720 7275   tie-breaking ru
+000081e0: 6c65 2e20 416c 736f 206b 6e6f 776e 2061  le. Also known a
+000081f0: 7320 5469 6465 6d61 6e27 7320 5275 6c65  s Tideman's Rule
+00008200: 2e0a 0a20 2020 202e 2e20 7761 726e 696e  ...    .. warnin
+00008210: 673a 3a20 0a20 2020 2020 2020 2054 6869  g:: .        Thi
+00008220: 7320 6d65 7468 6f64 2063 616e 2074 616b  s method can tak
+00008230: 6520 6120 7665 7279 206c 6f6e 6720 7469  e a very long ti
+00008240: 6d65 2074 6f20 6669 6e64 2077 696e 6e65  me to find winne
+00008250: 7273 2e20 0a20 2020 2020 2020 200a 2020  rs. .        .  
+00008260: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008270: 6564 6174 6120 2850 726f 6669 6c65 2c20  edata (Profile, 
+00008280: 5072 6f66 696c 6557 6974 6854 6965 732c  ProfileWithTies,
+00008290: 204d 6172 6769 6e47 7261 7068 293a 2041   MarginGraph): A
+000082a0: 6e79 2065 6c65 6374 696f 6e20 6461 7461  ny election data
+000082b0: 2074 6861 7420 6861 7320 6120 606d 6172   that has a `mar
+000082c0: 6769 6e60 206d 6574 686f 642e 200a 2020  gin` method. .  
+000082d0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
+000082e0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+000082f0: 696f 6e61 6c29 3a20 4966 2073 6574 2c20  ional): If set, 
+00008300: 7468 656e 2066 696e 6420 7468 6520 7769  then find the wi
+00008310: 6e6e 6572 7320 666f 7220 7468 6520 7072  nners for the pr
+00008320: 6f66 696c 6520 7265 7374 7269 6374 6564  ofile restricted
+00008330: 2074 6f20 7468 6520 6361 6e64 6964 6174   to the candidat
+00008340: 6573 2069 6e20 6060 6375 7272 5f63 616e  es in ``curr_can
+00008350: 6473 6060 0a20 2020 2020 2020 2073 7472  ds``.        str
+00008360: 656e 6774 685f 6675 6e63 7469 6f6e 2028  ength_function (
+00008370: 6675 6e63 7469 6f6e 2c20 6f70 7469 6f6e  function, option
+00008380: 616c 293a 2054 6865 2073 7472 656e 6774  al): The strengt
+00008390: 6820 6675 6e63 7469 6f6e 2074 6f20 6265  h function to be
+000083a0: 2075 7365 6420 746f 2063 616c 6375 6c61   used to calcula
+000083b0: 7465 2074 6865 2073 7472 656e 6774 6820  te the strength 
+000083c0: 6f66 2061 2070 6174 682e 2020 2054 6865  of a path.   The
+000083d0: 2064 6566 6175 6c74 2069 7320 7468 6520   default is the 
+000083e0: 6d61 7267 696e 206d 6574 686f 6420 6f66  margin method of
+000083f0: 2060 6065 6461 7461 6060 2e20 2020 5468   ``edata``.   Th
+00008400: 6973 206f 6e6c 7920 6d61 7474 6572 7320  is only matters 
+00008410: 7768 656e 2074 6865 2062 616c 6c6f 7473  when the ballots
+00008420: 2061 7265 206e 6f74 206c 696e 6561 7220   are not linear 
+00008430: 6f72 6465 7273 2e20 0a20 2020 2020 2020  orders. .       
+00008440: 2061 6c67 6f72 6974 686d 2028 7374 722c   algorithm (str,
+00008450: 206f 7074 696f 6e61 6c29 3a20 5370 6563   optional): Spec
+00008460: 6966 7920 7768 6963 6820 616c 676f 7269  ify which algori
+00008470: 7468 6d20 746f 2075 7365 2e20 204f 7074  thm to use.  Opt
+00008480: 696f 6e73 2061 7265 2027 6261 7369 6327  ions are 'basic'
+00008490: 2028 7468 6520 6465 6661 756c 7429 2061   (the default) a
+000084a0: 6e64 2027 6672 6f6d 5f73 7461 636b 7327  nd 'from_stacks'
+000084b0: 2e0a 0a20 2020 2052 6574 7572 6e73 3a20  ...    Returns: 
+000084c0: 0a20 2020 2020 2020 2041 2073 6f72 7465  .        A sorte
+000084d0: 6420 6c69 7374 206f 6620 6361 6e64 6964  d list of candid
+000084e0: 6174 6573 2e20 0a0a 2020 2020 2e2e 2073  ates. ..    .. s
+000084f0: 6565 616c 736f 3a3a 0a0a 2020 2020 2020  eealso::..      
+00008500: 2020 3a6d 6574 683a 6070 7265 665f 766f    :meth:`pref_vo
+00008510: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+00008520: 645f 6d65 7468 6f64 732e 7261 6e6b 6564  d_methods.ranked
+00008530: 5f70 6169 7273 5f77 6974 685f 7465 7374  _pairs_with_test
+00008540: 602c 203a 6d65 7468 3a60 7072 6566 5f76  `, :meth:`pref_v
+00008550: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+00008560: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+00008570: 645f 7061 6972 735f 7a74 602c 203a 6d65  d_pairs_zt`, :me
+00008580: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+00008590: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+000085a0: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+000085b0: 735f 6465 6665 6174 7360 0a0a 2020 2020  s_defeats`..    
+000085c0: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
+000085d0: 2e2e 2070 6c6f 743a 3a20 206d 6172 6769  .. plot::  margi
+000085e0: 6e5f 6772 6170 6873 5f65 7861 6d70 6c65  n_graphs_example
+000085f0: 732f 6d67 5f65 785f 6270 5f72 702e 7079  s/mg_ex_bp_rp.py
+00008600: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00008610: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00008620: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00008630: 6365 3a20 5472 7565 0a0a 0a20 2020 202e  ce: True...    .
+00008640: 2e20 636f 6465 2d62 6c6f 636b 3a3a 200a  . code-block:: .
+00008650: 0a20 2020 2020 2020 2066 726f 6d20 7072  .        from pr
+00008660: 6566 5f76 6f74 696e 672e 6d61 7267 696e  ef_voting.margin
+00008670: 5f62 6173 6564 5f6d 6574 686f 6473 2069  _based_methods i
+00008680: 6d70 6f72 7420 7261 6e6b 6564 5f70 6169  mport ranked_pai
+00008690: 7273 0a0a 2020 2020 2020 2020 7261 6e6b  rs..        rank
+000086a0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+000086b0: 286d 6729 0a20 2020 2020 2020 2072 616e  (mg).        ran
+000086c0: 6b65 645f 7061 6972 732e 6469 7370 6c61  ked_pairs.displa
+000086d0: 7928 6d67 2c20 616c 676f 7269 7468 6d3d  y(mg, algorithm=
+000086e0: 2762 6173 6963 2729 200a 2020 2020 2020  'basic') .      
+000086f0: 2020 7261 6e6b 6564 5f70 6169 7273 2e64    ranked_pairs.d
+00008700: 6973 706c 6179 286d 672c 2061 6c67 6f72  isplay(mg, algor
+00008710: 6974 686d 3d27 6672 6f6d 5f73 7461 636b  ithm='from_stack
+00008720: 7327 2920 2020 200a 0a0a 2020 2020 2e2e  s')    ...    ..
+00008730: 2065 7865 635f 636f 6465 3a3a 200a 2020   exec_code:: .  
+00008740: 2020 2020 2020 3a68 6964 655f 636f 6465        :hide_code
+00008750: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+00008760: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+00008770: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+00008780: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+00008790: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+000087a0: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+000087b0: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+000087c0: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
+000087d0: 6b65 645f 7061 6972 730a 2020 2020 2020  ked_pairs.      
+000087e0: 2020 0a20 2020 2020 2020 206d 6720 3d20    .        mg = 
+000087f0: 4d61 7267 696e 4772 6170 6828 5b30 2c20  MarginGraph([0, 
+00008800: 312c 2032 2c20 335d 2c20 5b28 302c 2032  1, 2, 3], [(0, 2
+00008810: 2c20 3329 2c20 2831 2c20 302c 2035 292c  , 3), (1, 0, 5),
+00008820: 2028 322c 2031 2c20 3529 2c20 2832 2c20   (2, 1, 5), (2, 
+00008830: 332c 2031 292c 2028 332c 2030 2c20 3329  3, 1), (3, 0, 3)
+00008840: 2c20 2833 2c20 312c 2031 295d 290a 2020  , (3, 1, 1)]).  
+00008850: 2020 2020 2020 0a20 2020 2020 2020 2072        .        r
+00008860: 616e 6b65 645f 7061 6972 732e 6469 7370  anked_pairs.disp
+00008870: 6c61 7928 6d67 290a 2020 2020 2020 2020  lay(mg).        
+00008880: 7261 6e6b 6564 5f70 6169 7273 2e64 6973  ranked_pairs.dis
+00008890: 706c 6179 286d 672c 2061 6c67 6f72 6974  play(mg, algorit
+000088a0: 686d 3d27 6261 7369 6327 290a 2020 2020  hm='basic').    
+000088b0: 2020 2020 7261 6e6b 6564 5f70 6169 7273      ranked_pairs
+000088c0: 2e64 6973 706c 6179 286d 672c 2061 6c67  .display(mg, alg
+000088d0: 6f72 6974 686d 3d27 6672 6f6d 5f73 7461  orithm='from_sta
+000088e0: 636b 7327 290a 0a20 2020 2022 2222 0a0a  cks')..    """..
+000088f0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
+00008900: 203d 3d20 2762 6173 6963 273a 0a20 2020   == 'basic':.   
+00008910: 2020 2020 2072 6574 7572 6e20 5f72 616e       return _ran
+00008920: 6b65 645f 7061 6972 735f 6261 7369 6328  ked_pairs_basic(
+00008930: 6564 6174 612c 2063 7572 725f 6361 6e64  edata, curr_cand
+00008940: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
+00008950: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00008960: 6e20 3d20 7374 7265 6e67 7468 5f66 756e  n = strength_fun
+00008970: 6374 696f 6e29 0a20 2020 2065 6c69 6620  ction).    elif 
+00008980: 616c 676f 7269 7468 6d20 3d3d 2027 6672  algorithm == 'fr
+00008990: 6f6d 5f73 7461 636b 7327 3a0a 2020 2020  om_stacks':.    
+000089a0: 2020 2020 7265 7475 726e 205f 7261 6e6b      return _rank
+000089b0: 6564 5f70 6169 7273 5f66 726f 6d5f 7374  ed_pairs_from_st
+000089c0: 6163 6b73 2865 6461 7461 2c20 6375 7272  acks(edata, curr
+000089d0: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+000089e0: 6e64 7329 0a20 2020 2065 6c73 653a 0a20  nds).    else:. 
+000089f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00008a00: 7565 4572 726f 7228 2249 6e76 616c 6964  ueError("Invalid
+00008a10: 2061 6c67 6f72 6974 686d 2073 7065 6369   algorithm speci
+00008a20: 6669 6564 2e22 290a 0a40 766d 286e 616d  fied.")..@vm(nam
+00008a30: 653d 2252 616e 6b65 6420 5061 6972 7322  e="Ranked Pairs"
+00008a40: 2c0a 2020 2020 736b 6970 5f72 6567 6973  ,.    skip_regis
+00008a50: 7472 6174 696f 6e3d 5472 7565 290a 6465  tration=True).de
+00008a60: 6620 7261 6e6b 6564 5f70 6169 7273 5f77  f ranked_pairs_w
+00008a70: 6974 685f 7465 7374 280a 2020 2020 6564  ith_test(.    ed
+00008a80: 6174 612c 200a 2020 2020 6375 7272 5f63  ata, .    curr_c
+00008a90: 616e 6473 3d4e 6f6e 652c 200a 2020 2020  ands=None, .    
+00008aa0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00008ab0: 6e3d 4e6f 6e65 293a 2020 200a 2020 2020  n=None):   .    
+00008ac0: 2222 2246 696e 6420 7468 6520 5261 6e6b  """Find the Rank
+00008ad0: 6564 2050 6169 7273 2077 696e 6e65 7273  ed Pairs winners
+00008ae0: 2c20 6275 7420 696e 636c 7564 6520 6120  , but include a 
+00008af0: 7465 7374 2074 6f20 6465 7465 726d 696e  test to determin
+00008b00: 6564 2069 6620 6974 2077 696c 6c20 7461  ed if it will ta
+00008b10: 6b65 2074 6f6f 206c 6f6e 6720 746f 2063  ke too long to c
+00008b20: 6f6d 7075 7465 2074 6865 2052 616e 6b65  ompute the Ranke
+00008b30: 6420 5061 6972 7320 7769 6e6e 6572 732e  d Pairs winners.
+00008b40: 2049 6620 7468 6520 6361 6c63 756c 6174   If the calculat
+00008b50: 696f 6e20 6f66 2074 6865 2077 696e 6e65  ion of the winne
+00008b60: 7273 2077 696c 6c20 7461 6b65 2074 6f6f  rs will take too
+00008b70: 206c 6f6e 672c 2072 6574 7572 6e20 4e6f   long, return No
+00008b80: 6e65 2e0a 0a20 2020 202e 2e20 696d 706f  ne...    .. impo
+00008b90: 7274 616e 743a 3a0a 2020 2020 2020 2020  rtant::.        
+00008ba0: 5468 6973 2076 6f74 696e 6720 6d65 7468  This voting meth
+00008bb0: 6f64 2074 6861 7420 6d69 6768 7420 7265  od that might re
+00008bc0: 7475 726e 204e 6f6e 6520 7261 7468 6572  turn None rather
+00008bd0: 2074 6861 6e20 6120 6c69 7374 206f 6620   than a list of 
+00008be0: 6361 6e64 6964 6174 6573 2e20 200a 0a20  candidates.  .. 
+00008bf0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00008c00: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
+00008c10: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
+00008c20: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
+00008c30: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
+00008c40: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
+00008c50: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
+00008c60: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+00008c70: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
+00008c80: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
+00008c90: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
+00008ca0: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
+00008cb0: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
+00008cc0: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
+00008cd0: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
+00008ce0: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
+00008cf0: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00008d00: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
+00008d10: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
+00008d20: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
+00008d30: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
+00008d40: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
+00008d50: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
+00008d60: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
+00008d70: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
+00008d80: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
+00008d90: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
+00008da0: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
+00008db0: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
+00008dc0: 206f 7264 6572 732e 200a 0a20 2020 2052   orders. ..    R
+00008dd0: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+00008de0: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
+00008df0: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
+00008e00: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
+00008e10: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
+00008e20: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+00008e30: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00008e40: 732e 7261 6e6b 6564 5f70 6169 7273 5f77  s.ranked_pairs_w
+00008e50: 6974 685f 7465 7374 602c 203a 6d65 7468  ith_test`, :meth
+00008e60: 3a60 7072 6566 5f76 6f74 696e 672e 6d61  :`pref_voting.ma
+00008e70: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
+00008e80: 6473 2e72 616e 6b65 645f 7061 6972 735f  ds.ranked_pairs_
+00008e90: 7a74 602c 203a 6d65 7468 3a60 7072 6566  zt`, :meth:`pref
+00008ea0: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00008eb0: 6173 6564 5f6d 6574 686f 6473 2e72 616e  ased_methods.ran
+00008ec0: 6b65 645f 7061 6972 735f 6465 6665 6174  ked_pairs_defeat
+00008ed0: 7360 0a0a 2020 2020 3a45 7861 6d70 6c65  s`..    :Example
+00008ee0: 3a20 0a0a 2020 2020 2e2e 2070 6c6f 743a  : ..    .. plot:
+00008ef0: 3a20 206d 6172 6769 6e5f 6772 6170 6873  :  margin_graphs
+00008f00: 5f65 7861 6d70 6c65 732f 6d67 5f65 785f  _examples/mg_ex_
+00008f10: 7270 5f77 6974 685f 7465 7374 2e70 790a  rp_with_test.py.
+00008f20: 2020 2020 2020 2020 3a63 6f6e 7465 7874          :context
+00008f30: 3a20 7265 7365 7420 200a 2020 2020 2020  : reset  .      
+00008f40: 2020 3a69 6e63 6c75 6465 2d73 6f75 7263    :include-sourc
+00008f50: 653a 2054 7275 650a 0a0a 2020 2020 2e2e  e: True...    ..
+00008f60: 2063 6f64 652d 626c 6f63 6b3a 3a20 0a0a   code-block:: ..
+00008f70: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+00008f80: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00008f90: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+00008fa0: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
+00008fb0: 735f 7769 7468 5f74 6573 740a 0a20 2020  s_with_test..   
+00008fc0: 2020 2020 2072 616e 6b65 645f 7061 6972       ranked_pair
+00008fd0: 735f 7769 7468 5f74 6573 742e 6469 7370  s_with_test.disp
+00008fe0: 6c61 7928 6d67 290a 0a0a 2020 2020 2e2e  lay(mg)...    ..
+00008ff0: 2065 7865 635f 636f 6465 3a3a 200a 2020   exec_code:: .  
+00009000: 2020 2020 2020 3a68 6964 655f 636f 6465        :hide_code
+00009010: 3a0a 0a20 2020 2020 2020 2066 726f 6d20  :..        from 
+00009020: 7072 6566 5f76 6f74 696e 672e 7765 6967  pref_voting.weig
+00009030: 6874 6564 5f6d 616a 6f72 6974 795f 6772  hted_majority_gr
+00009040: 6170 6873 2069 6d70 6f72 7420 4d61 7267  aphs import Marg
+00009050: 696e 4772 6170 680a 2020 2020 2020 2020  inGraph.        
+00009060: 6672 6f6d 2070 7265 665f 766f 7469 6e67  from pref_voting
+00009070: 2e6d 6172 6769 6e5f 6261 7365 645f 6d65  .margin_based_me
+00009080: 7468 6f64 7320 696d 706f 7274 2072 616e  thods import ran
+00009090: 6b65 645f 7061 6972 735f 7769 7468 5f74  ked_pairs_with_t
+000090a0: 6573 740a 2020 2020 2020 2020 0a20 2020  est.        .   
+000090b0: 2020 2020 206d 6720 3d20 4d61 7267 696e       mg = Margin
+000090c0: 4772 6170 6828 5b30 2c20 312c 2032 2c20  Graph([0, 1, 2, 
+000090d0: 335d 2c20 5b28 312c 2032 2c20 3229 2c20  3], [(1, 2, 2), 
+000090e0: 2831 2c20 332c 2032 292c 2028 322c 2030  (1, 3, 2), (2, 0
+000090f0: 2c20 3229 5d29 0a20 2020 2020 2020 200a  , 2)]).        .
+00009100: 2020 2020 2020 2020 7261 6e6b 6564 5f70          ranked_p
+00009110: 6169 7273 5f77 6974 685f 7465 7374 2e64  airs_with_test.d
+00009120: 6973 706c 6179 286d 6729 0a0a 0a20 2020  isplay(mg)...   
+00009130: 2022 2222 2020 2020 0a20 2020 2063 616e   """    .    can
+00009140: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+00009150: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+00009160: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00009170: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00009180: 2020 2020 0a20 2020 2063 6964 785f 746f      .    cidx_to
+00009190: 5f63 616e 6420 3d20 7b63 6964 783a 2063  _cand = {cidx: c
+000091a0: 2066 6f72 2063 6964 782c 2063 2069 6e20   for cidx, c in 
+000091b0: 656e 756d 6572 6174 6528 6361 6e64 6964  enumerate(candid
+000091c0: 6174 6573 297d 2020 0a20 2020 2063 616e  ates)}  .    can
+000091d0: 645f 746f 5f63 6964 7820 3d20 7b63 3a20  d_to_cidx = {c: 
+000091e0: 6369 6478 2066 6f72 2063 6964 782c 2063  cidx for cidx, c
+000091f0: 2069 6e20 656e 756d 6572 6174 6528 6361   in enumerate(ca
+00009200: 6e64 6964 6174 6573 297d 2020 0a20 2020  ndidates)}  .   
+00009210: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+00009220: 756e 6374 696f 6e20 3d20 6564 6174 612e  unction = edata.
+00009230: 6d61 7267 696e 2069 6620 7374 7265 6e67  margin if streng
+00009240: 7468 5f66 756e 6374 696f 6e20 6973 204e  th_function is N
+00009250: 6f6e 6520 656c 7365 2073 7472 656e 6774  one else strengt
+00009260: 685f 6675 6e63 7469 6f6e 2020 200a 0a20  h_function   .. 
+00009270: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
+00009280: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
+00009290: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+000092a0: 5f63 616e 6473 290a 2020 2020 2320 5261  _cands).    # Ra
+000092b0: 6e6b 6564 2050 6169 7273 2069 7320 436f  nked Pairs is Co
+000092c0: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
+000092d0: 6e74 2c20 736f 2073 696d 706c 7920 7265  nt, so simply re
+000092e0: 7475 726e 2074 6865 2043 6f6e 646f 7263  turn the Condorc
+000092f0: 6574 2077 696e 6e65 7220 6966 2065 7869  et winner if exi
+00009300: 7374 730a 2020 2020 6966 2063 7720 6973  sts.    if cw is
+00009310: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
+00009320: 2020 2020 7769 6e6e 6572 7320 3d20 5b63      winners = [c
+00009330: 775d 0a20 2020 2065 6c73 653a 0a20 2020  w].    else:.   
+00009340: 2020 2020 2077 5f65 6467 6573 203d 205b       w_edges = [
+00009350: 2863 312c 2063 322c 2073 7472 656e 6774  (c1, c2, strengt
+00009360: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
+00009370: 3229 2920 666f 7220 6331 2069 6e20 6361  2)) for c1 in ca
+00009380: 6e64 6964 6174 6573 2066 6f72 2063 3220  ndidates for c2 
+00009390: 696e 2063 616e 6469 6461 7465 7320 0a20  in candidates . 
+000093a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000093b0: 2020 6966 2063 3120 213d 2063 3220 616e    if c1 != c2 an
+000093c0: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
+000093d0: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
+000093e0: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
+000093f0: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
+00009400: 2020 2020 2077 696e 6e65 7273 203d 206c       winners = l
+00009410: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
+00009420: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
+00009430: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
+00009440: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
+00009450: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
+00009460: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
+00009470: 2020 2020 2020 2073 6f72 7465 645f 6564         sorted_ed
+00009480: 6765 7320 3d20 5b5b 6520 666f 7220 6520  ges = [[e for e 
+00009490: 696e 2077 5f65 6467 6573 2069 6620 655b  in w_edges if e[
+000094a0: 325d 203d 3d20 735d 2066 6f72 2073 2069  2] == s] for s i
+000094b0: 6e20 7374 7265 6e67 7468 735d 0a20 2020  n strengths].   
+000094c0: 2020 2020 2069 6620 6e70 2e70 726f 6428       if np.prod(
+000094d0: 5b6d 6174 682e 6661 6374 6f72 6961 6c28  [math.factorial(
+000094e0: 6c65 6e28 6573 2929 2066 6f72 2065 7320  len(es)) for es 
+000094f0: 696e 2073 6f72 7465 645f 6564 6765 735d  in sorted_edges]
+00009500: 2920 3e20 3330 3030 3a20 0a20 2020 2020  ) > 3000: .     
+00009510: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00009520: 6e65 0a20 2020 2020 2020 2065 6c73 653a  ne.        else:
+00009530: 200a 2020 2020 2020 2020 2020 2020 7462   .            tb
+00009540: 7320 3d20 7072 6f64 7563 7428 2a5b 7065  s = product(*[pe
+00009550: 726d 7574 6174 696f 6e73 2865 6467 6573  rmutations(edges
+00009560: 2920 666f 7220 6564 6765 7320 696e 2073  ) for edges in s
+00009570: 6f72 7465 645f 6564 6765 735d 290a 2020  orted_edges]).  
+00009580: 2020 2020 2020 2020 2020 666f 7220 7462            for tb
+00009590: 2069 6e20 7462 733a 0a20 2020 2020 2020   in tbs:.       
+000095a0: 2020 2020 2020 2020 2065 6467 6573 203d           edges =
+000095b0: 2066 6c61 7474 656e 2874 6229 0a20 2020   flatten(tb).   
+000095c0: 2020 2020 2020 2020 2020 2020 2072 705f               rp_
+000095d0: 6465 6665 6174 203d 2053 504f 286c 656e  defeat = SPO(len
+000095e0: 2863 616e 6469 6461 7465 7329 290a 2020  (candidates)).  
+000095f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00009600: 7220 6530 2c65 312c 7320 696e 2065 6467  r e0,e1,s in edg
+00009610: 6573 3a20 0a20 2020 2020 2020 2020 2020  es: .           
+00009620: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00009630: 7270 5f64 6566 6561 742e 505b 6361 6e64  rp_defeat.P[cand
+00009640: 5f74 6f5f 6369 6478 5b65 315d 5d5b 6361  _to_cidx[e1]][ca
+00009650: 6e64 5f74 6f5f 6369 6478 5b65 305d 5d3a  nd_to_cidx[e0]]:
+00009660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009670: 2020 2020 2020 2020 2072 705f 6465 6665           rp_defe
+00009680: 6174 2e61 6464 2863 616e 645f 746f 5f63  at.add(cand_to_c
+00009690: 6964 785b 6530 5d2c 6361 6e64 5f74 6f5f  idx[e0],cand_to_
+000096a0: 6369 6478 5b65 315d 290a 2020 2020 2020  cidx[e1]).      
+000096b0: 2020 2020 2020 2020 2020 7769 6e6e 6572            winner
+000096c0: 732e 6170 7065 6e64 2863 6964 785f 746f  s.append(cidx_to
+000096d0: 5f63 616e 645b 7270 5f64 6566 6561 742e  _cand[rp_defeat.
+000096e0: 696e 6974 6961 6c5f 656c 656d 656e 7473  initial_elements
+000096f0: 2829 5b30 5d5d 290a 2020 2020 7265 7475  ()[0]]).    retu
+00009700: 726e 2073 6f72 7465 6428 6c69 7374 2873  rn sorted(list(s
+00009710: 6574 2877 696e 6e65 7273 2929 290a 0a64  et(winners)))..d
+00009720: 6566 2072 616e 6b65 645f 7061 6972 735f  ef ranked_pairs_
+00009730: 6465 6665 6174 7328 6564 6174 612c 2063  defeats(edata, c
+00009740: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+00009750: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+00009760: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
+00009770: 2020 2020 2222 220a 2020 2020 5265 7475      """.    Retu
+00009780: 726e 7320 7468 6520 5261 6e6b 6564 2050  rns the Ranked P
+00009790: 6169 7273 2064 6566 6561 7420 7265 6c61  airs defeat rela
+000097a0: 7469 6f6e 7320 7072 6f64 7563 6564 2062  tions produced b
+000097b0: 7920 7468 6520 5261 6e6b 6564 2050 6169  y the Ranked Pai
+000097c0: 7273 2061 6c67 6f72 6974 686d 2e20 0a0a  rs algorithm. ..
+000097d0: 2020 2020 2e2e 2069 6d70 6f72 7461 6e74      .. important
+000097e0: 3a3a 0a20 2020 2020 2020 2055 6e6c 696b  ::.        Unlik
+000097f0: 6520 7468 6520 6f74 6865 7220 6675 6e63  e the other func
+00009800: 7469 6f6e 7320 7468 6174 2072 6574 7572  tions that retur
+00009810: 6e20 6120 7369 6e67 6c65 2064 6566 6561  n a single defea
+00009820: 7420 7265 6c61 7469 6f6e 2c20 7468 6973  t relation, this
+00009830: 2072 6574 7572 6e73 2061 206c 6973 7420   returns a list 
+00009840: 6f66 2064 6566 6561 7420 7265 6c61 7469  of defeat relati
+00009850: 6f6e 732e 200a 2020 2020 2020 2020 0a20  ons. .        . 
+00009860: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00009870: 2065 6461 7461 2028 5072 6f66 696c 652c   edata (Profile,
+00009880: 2050 726f 6669 6c65 5769 7468 5469 6573   ProfileWithTies
+00009890: 2c20 4d61 7267 696e 4772 6170 6829 3a20  , MarginGraph): 
+000098a0: 416e 7920 656c 6563 7469 6f6e 2064 6174  Any election dat
+000098b0: 6120 7468 6174 2068 6173 2061 2060 6d61  a that has a `ma
+000098c0: 7267 696e 6020 6d65 7468 6f64 2e20 0a20  rgin` method. . 
+000098d0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+000098e0: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
+000098f0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
+00009900: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
+00009910: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
+00009920: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
+00009930: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
+00009940: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
+00009950: 6e64 7360 600a 2020 2020 2020 2020 7374  nds``.        st
+00009960: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+00009970: 2866 756e 6374 696f 6e2c 206f 7074 696f  (function, optio
+00009980: 6e61 6c29 3a20 5468 6520 7374 7265 6e67  nal): The streng
+00009990: 7468 2066 756e 6374 696f 6e20 746f 2062  th function to b
+000099a0: 6520 7573 6564 2074 6f20 6361 6c63 756c  e used to calcul
+000099b0: 6174 6520 7468 6520 7374 7265 6e67 7468  ate the strength
+000099c0: 206f 6620 6120 7061 7468 2e20 2020 5468   of a path.   Th
+000099d0: 6520 6465 6661 756c 7420 6973 2074 6865  e default is the
+000099e0: 206d 6172 6769 6e20 6d65 7468 6f64 206f   margin method o
+000099f0: 6620 6060 6564 6174 6160 602e 2020 2054  f ``edata``.   T
+00009a00: 6869 7320 6f6e 6c79 206d 6174 7465 7273  his only matters
+00009a10: 2077 6865 6e20 7468 6520 6261 6c6c 6f74   when the ballot
+00009a20: 7320 6172 6520 6e6f 7420 6c69 6e65 6172  s are not linear
+00009a30: 206f 7264 6572 732e 200a 0a20 2020 2052   orders. ..    R
+00009a40: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+00009a50: 2041 206e 6574 776f 726b 7820 4469 4772   A networkx DiGr
+00009a60: 6170 6820 7265 7072 6573 656e 7469 6e67  aph representing
+00009a70: 2074 6865 2052 616e 6b65 6420 5061 6972   the Ranked Pair
+00009a80: 7320 6465 6665 6174 2072 656c 6174 696f  s defeat relatio
+00009a90: 6e2e 200a 0a20 2020 202e 2e20 7365 6561  n. ..    .. seea
+00009aa0: 6c73 6f3a 3a0a 0a20 2020 2020 2020 203a  lso::..        :
+00009ab0: 6d65 7468 3a60 7072 6566 5f76 6f74 696e  meth:`pref_votin
+00009ac0: 672e 6d61 7267 696e 5f62 6173 6564 5f6d  g.margin_based_m
+00009ad0: 6574 686f 6473 2e72 616e 6b65 645f 7061  ethods.ranked_pa
+00009ae0: 6972 7360 2c20 3a6d 6574 683a 6070 7265  irs`, :meth:`pre
+00009af0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+00009b00: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
+00009b10: 6e6b 6564 5f70 6169 7273 5f77 6974 685f  nked_pairs_with_
+00009b20: 7465 7374 600a 0a20 2020 203a 4578 616d  test`..    :Exam
+00009b30: 706c 653a 200a 0a20 2020 202e 2e20 706c  ple: ..    .. pl
+00009b40: 6f74 3a3a 2020 6d61 7267 696e 5f67 7261  ot::  margin_gra
+00009b50: 7068 735f 6578 616d 706c 6573 2f6d 675f  phs_examples/mg_
+00009b60: 6578 5f72 705f 6465 6665 6174 732e 7079  ex_rp_defeats.py
+00009b70: 0a20 2020 2020 2020 203a 636f 6e74 6578  .        :contex
+00009b80: 743a 2072 6573 6574 2020 0a20 2020 2020  t: reset  .     
+00009b90: 2020 203a 696e 636c 7564 652d 736f 7572     :include-sour
+00009ba0: 6365 3a20 5472 7565 0a0a 2020 2020 2e2e  ce: True..    ..
+00009bb0: 2065 7865 635f 636f 6465 3a3a 0a0a 0a20   exec_code::... 
+00009bc0: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+00009bd0: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
+00009be0: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
+00009bf0: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
+00009c00: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
+00009c10: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+00009c20: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+00009c30: 7320 696d 706f 7274 2072 616e 6b65 645f  s import ranked_
+00009c40: 7061 6972 735f 6465 6665 6174 730a 0a20  pairs_defeats.. 
+00009c50: 2020 2020 2020 206d 6720 3d20 4d61 7267         mg = Marg
+00009c60: 696e 4772 6170 6828 5b30 2c20 312c 2032  inGraph([0, 1, 2
+00009c70: 2c20 335d 2c20 5b28 302c 2031 2c20 3130  , 3], [(0, 1, 10
+00009c80: 292c 2028 302c 2032 2c20 3229 2c20 2831  ), (0, 2, 2), (1
+00009c90: 2c20 332c 2034 292c 2028 322c 2031 2c20  , 3, 4), (2, 1, 
+00009ca0: 3629 2c20 2832 2c20 332c 2038 292c 2028  6), (2, 3, 8), (
+00009cb0: 332c 2030 2c20 3429 5d29 0a20 2020 2020  3, 0, 4)]).     
+00009cc0: 2020 2072 705f 6465 6665 6174 7320 3d20     rp_defeats = 
+00009cd0: 7261 6e6b 6564 5f70 6169 7273 5f64 6566  ranked_pairs_def
+00009ce0: 6561 7473 286d 6729 0a0a 2020 2020 2020  eats(mg)..      
+00009cf0: 2020 666f 7220 7270 6420 696e 2072 705f    for rpd in rp_
+00009d00: 6465 6665 6174 733a 200a 2020 2020 2020  defeats: .      
+00009d10: 2020 2020 2020 7072 696e 7428 7270 642e        print(rpd.
+00009d20: 6564 6765 7329 0a0a 2020 2020 2222 220a  edges)..    """.
+00009d30: 2020 2020 0a20 2020 2063 616e 6469 6461      .    candida
+00009d40: 7465 7320 3d20 6564 6174 612e 6361 6e64  tes = edata.cand
+00009d50: 6964 6174 6573 2069 6620 6375 7272 5f63  idates if curr_c
+00009d60: 616e 6473 2069 7320 4e6f 6e65 2065 6c73  ands is None els
+00009d70: 6520 6375 7272 5f63 616e 6473 2020 2020  e curr_cands    
+00009d80: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+00009d90: 6e63 7469 6f6e 203d 2065 6461 7461 2e6d  nction = edata.m
+00009da0: 6172 6769 6e20 6966 2073 7472 656e 6774  argin if strengt
+00009db0: 685f 6675 6e63 7469 6f6e 2069 7320 4e6f  h_function is No
+00009dc0: 6e65 2065 6c73 6520 7374 7265 6e67 7468  ne else strength
+00009dd0: 5f66 756e 6374 696f 6e20 2020 200a 0a20  _function    .. 
+00009de0: 2020 2077 5f65 6467 6573 203d 205b 2863     w_edges = [(c
+00009df0: 312c 2063 322c 2073 7472 656e 6774 685f  1, c2, strength_
+00009e00: 6675 6e63 7469 6f6e 2863 312c 2063 3229  function(c1, c2)
+00009e10: 2920 666f 7220 6331 2069 6e20 6361 6e64  ) for c1 in cand
+00009e20: 6964 6174 6573 2066 6f72 2063 3220 696e  idates for c2 in
+00009e30: 2063 616e 6469 6461 7465 7320 6966 2063   candidates if c
+00009e40: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+00009e50: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+00009e60: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+00009e70: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+00009e80: 2063 3229 295d 0a20 2020 2077 696e 6e65   c2))].    winne
+00009e90: 7273 203d 206c 6973 7428 2920 2020 2020  rs = list()     
+00009ea0: 2020 2020 2020 200a 2020 2020 7374 7265         .    stre
+00009eb0: 6e67 7468 7320 3d20 736f 7274 6564 286c  ngths = sorted(l
+00009ec0: 6973 7428 7365 7428 5b65 5b32 5d20 666f  ist(set([e[2] fo
+00009ed0: 7220 6520 696e 2077 5f65 6467 6573 5d29  r e in w_edges])
+00009ee0: 292c 2072 6576 6572 7365 3d54 7275 6529  ), reverse=True)
+00009ef0: 0a20 2020 2073 6f72 7465 645f 6564 6765  .    sorted_edge
+00009f00: 7320 3d20 5b5b 6520 666f 7220 6520 696e  s = [[e for e in
+00009f10: 2077 5f65 6467 6573 2069 6620 655b 325d   w_edges if e[2]
+00009f20: 203d 3d20 735d 2066 6f72 2073 2069 6e20   == s] for s in 
+00009f30: 7374 7265 6e67 7468 735d 0a20 2020 2074  strengths].    t
+00009f40: 6273 203d 2070 726f 6475 6374 282a 5b70  bs = product(*[p
+00009f50: 6572 6d75 7461 7469 6f6e 7328 6564 6765  ermutations(edge
+00009f60: 7329 2066 6f72 2065 6467 6573 2069 6e20  s) for edges in 
+00009f70: 736f 7274 6564 5f65 6467 6573 5d29 0a20  sorted_edges]). 
+00009f80: 2020 2072 705f 6465 6665 6174 7320 3d20     rp_defeats = 
+00009f90: 6c69 7374 2829 0a20 2020 2066 6f72 2074  list().    for t
+00009fa0: 6220 696e 2074 6273 3a0a 2020 2020 2020  b in tbs:.      
+00009fb0: 2020 6564 6765 7320 3d20 666c 6174 7465    edges = flatte
+00009fc0: 6e28 7462 290a 2020 2020 2020 2020 7270  n(tb).        rp
+00009fd0: 5f64 6566 6561 7420 3d20 6e78 2e44 6947  _defeat = nx.DiG
+00009fe0: 7261 7068 2829 200a 2020 2020 2020 2020  raph() .        
+00009ff0: 666f 7220 6520 696e 2065 6467 6573 3a20  for e in edges: 
+0000a000: 0a20 2020 2020 2020 2020 2020 2072 705f  .            rp_
+0000a010: 6465 6665 6174 2e61 6464 5f65 6467 6528  defeat.add_edge(
+0000a020: 655b 305d 2c20 655b 315d 2c20 7765 6967  e[0], e[1], weig
+0000a030: 6874 3d65 5b32 5d29 0a20 2020 2020 2020  ht=e[2]).       
+0000a040: 2020 2020 2069 6620 646f 6573 5f63 7265       if does_cre
+0000a050: 6174 655f 6379 636c 6528 7270 5f64 6566  ate_cycle(rp_def
+0000a060: 6561 742c 2065 293a 0a20 2020 2020 2020  eat, e):.       
+0000a070: 2020 2020 2020 2020 2072 705f 6465 6665           rp_defe
+0000a080: 6174 2e72 656d 6f76 655f 6564 6765 2865  at.remove_edge(e
+0000a090: 5b30 5d2c 2065 5b31 5d29 0a20 2020 2020  [0], e[1]).     
+0000a0a0: 2020 2072 705f 6465 6665 6174 732e 6170     rp_defeats.ap
+0000a0b0: 7065 6e64 2872 705f 6465 6665 6174 290a  pend(rp_defeat).
+0000a0c0: 2020 2020 2020 2020 7769 6e6e 6572 732e          winners.
+0000a0d0: 6170 7065 6e64 286d 6178 696d 616c 5f65  append(maximal_e
+0000a0e0: 6c65 6d65 6e74 7328 7270 5f64 6566 6561  lements(rp_defea
+0000a0f0: 7429 5b30 5d29 0a20 2020 2072 6574 7572  t)[0]).    retur
+0000a100: 6e20 7270 5f64 6566 6561 7473 0a0a 4076  n rp_defeats..@v
+0000a110: 6d28 6e61 6d65 3d22 5261 6e6b 6564 2050  m(name="Ranked P
+0000a120: 6169 7273 2054 4222 2c0a 2020 2020 696e  airs TB",.    in
+0000a130: 7075 745f 7479 7065 733d 5b45 6c65 6374  put_types=[Elect
+0000a140: 696f 6e54 7970 6573 2e50 524f 4649 4c45  ionTypes.PROFILE
+0000a150: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+0000a160: 5052 4f46 494c 455f 5749 5448 5f54 4945  PROFILE_WITH_TIE
+0000a170: 532c 2045 6c65 6374 696f 6e54 7970 6573  S, ElectionTypes
+0000a180: 2e4d 4152 4749 4e5f 4752 4150 485d 290a  .MARGIN_GRAPH]).
+0000a190: 6465 6620 7261 6e6b 6564 5f70 6169 7273  def ranked_pairs
+0000a1a0: 5f74 6228 0a20 2020 2065 6461 7461 2c20  _tb(.    edata, 
+0000a1b0: 0a20 2020 2063 7572 725f 6361 6e64 7320  .    curr_cands 
+0000a1c0: 3d20 4e6f 6e65 2c20 0a20 2020 2074 6965  = None, .    tie
+0000a1d0: 5f62 7265 616b 6572 203d 204e 6f6e 652c  _breaker = None,
+0000a1e0: 200a 2020 2020 7374 7265 6e67 7468 5f66   .    strength_f
+0000a1f0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+0000a200: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+0000a210: 5261 6e6b 6564 2050 6169 7273 2077 6974  Ranked Pairs wit
+0000a220: 6820 6120 6669 7865 6420 6c69 6e65 6172  h a fixed linear
+0000a230: 206f 7264 6572 206f 6e20 7468 6520 6361   order on the ca
+0000a240: 6e64 6964 6174 6573 2074 6f20 6272 6561  ndidates to brea
+0000a250: 6b20 616e 7920 7469 6573 2069 6e20 7468  k any ties in th
+0000a260: 6520 6d61 7267 696e 732e 2020 200a 2020  e margins.   .  
+0000a270: 2020 5369 6e63 6520 7468 6520 7469 655f    Since the tie_
+0000a280: 6272 6561 6b65 7220 6973 2061 206c 696e  breaker is a lin
+0000a290: 6561 7220 6f72 6465 722c 2074 6869 7320  ear order, this 
+0000a2a0: 6d65 7468 6f64 2069 7320 7265 736f 6c75  method is resolu
+0000a2b0: 7465 2e20 2020 0a0a 2020 2020 4172 6773  te.   ..    Args
+0000a2c0: 3a0a 2020 2020 2020 2020 6564 6174 6120  :.        edata 
+0000a2d0: 2850 726f 6669 6c65 2c20 5072 6f66 696c  (Profile, Profil
+0000a2e0: 6557 6974 6854 6965 732c 204d 6172 6769  eWithTies, Margi
+0000a2f0: 6e47 7261 7068 293a 2041 6e79 2065 6c65  nGraph): Any ele
+0000a300: 6374 696f 6e20 6461 7461 2074 6861 7420  ction data that 
+0000a310: 6861 7320 6120 606d 6172 6769 6e60 206d  has a `margin` m
+0000a320: 6574 686f 642e 200a 2020 2020 2020 2020  ethod. .        
+0000a330: 6375 7272 5f63 616e 6473 2028 4c69 7374  curr_cands (List
+0000a340: 5b69 6e74 5d2c 206f 7074 696f 6e61 6c29  [int], optional)
+0000a350: 3a20 4966 2073 6574 2c20 7468 656e 2066  : If set, then f
+0000a360: 696e 6420 7468 6520 7769 6e6e 6572 7320  ind the winners 
+0000a370: 666f 7220 7468 6520 7072 6f66 696c 6520  for the profile 
+0000a380: 7265 7374 7269 6374 6564 2074 6f20 7468  restricted to th
+0000a390: 6520 6361 6e64 6964 6174 6573 2069 6e20  e candidates in 
+0000a3a0: 6060 6375 7272 5f63 616e 6473 6060 0a20  ``curr_cands``. 
+0000a3b0: 2020 2020 2020 2073 7472 656e 6774 685f         strength_
+0000a3c0: 6675 6e63 7469 6f6e 2028 6675 6e63 7469  function (functi
+0000a3d0: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2054  on, optional): T
+0000a3e0: 6865 2073 7472 656e 6774 6820 6675 6e63  he strength func
+0000a3f0: 7469 6f6e 2074 6f20 6265 2075 7365 6420  tion to be used 
+0000a400: 746f 2063 616c 6375 6c61 7465 2074 6865  to calculate the
+0000a410: 2073 7472 656e 6774 6820 6f66 2061 2070   strength of a p
+0000a420: 6174 682e 2020 2054 6865 2064 6566 6175  ath.   The defau
+0000a430: 6c74 2069 7320 7468 6520 6d61 7267 696e  lt is the margin
+0000a440: 206d 6574 686f 6420 6f66 2060 6065 6461   method of ``eda
+0000a450: 7461 6060 2e20 2020 5468 6973 206f 6e6c  ta``.   This onl
+0000a460: 7920 6d61 7474 6572 7320 7768 656e 2074  y matters when t
+0000a470: 6865 2062 616c 6c6f 7473 2061 7265 206e  he ballots are n
+0000a480: 6f74 206c 696e 6561 7220 6f72 6465 7273  ot linear orders
+0000a490: 2e20 0a0a 2020 2020 5265 7475 726e 733a  . ..    Returns:
+0000a4a0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+0000a4b0: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+0000a4c0: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
+0000a4d0: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+0000a4e0: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+0000a4f0: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+0000a500: 6564 5f6d 6574 686f 6473 2e72 616e 6b65  ed_methods.ranke
+0000a510: 645f 7061 6972 7360 2c20 3a6d 6574 683a  d_pairs`, :meth:
+0000a520: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+0000a530: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000a540: 732e 7261 6e6b 6564 5f70 6169 7273 5f77  s.ranked_pairs_w
+0000a550: 6974 685f 7465 7374 600a 0a20 2020 202e  ith_test`..    .
+0000a560: 2e20 6578 6563 5f63 6f64 653a 3a0a 0a20  . exec_code::.. 
+0000a570: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+0000a580: 5f76 6f74 696e 672e 7072 6f66 696c 6573  _voting.profiles
+0000a590: 2069 6d70 6f72 7420 5072 6f66 696c 650a   import Profile.
+0000a5a0: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
+0000a5b0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+0000a5c0: 6261 7365 645f 6d65 7468 6f64 7320 696d  based_methods im
+0000a5d0: 706f 7274 2072 616e 6b65 645f 7061 6972  port ranked_pair
+0000a5e0: 735f 7462 2c20 7261 6e6b 6564 5f70 6169  s_tb, ranked_pai
+0000a5f0: 7273 5f7a 740a 0a20 2020 2020 2020 2070  rs_zt..        p
+0000a600: 726f 6620 3d20 5072 6f66 696c 6528 5b5b  rof = Profile([[
+0000a610: 322c 2033 2c20 312c 2030 5d2c 205b 302c  2, 3, 1, 0], [0,
+0000a620: 2033 2c20 312c 2032 5d2c 205b 312c 2033   3, 1, 2], [1, 3
+0000a630: 2c20 322c 2030 5d2c 205b 322c 2031 2c20  , 2, 0], [2, 1, 
+0000a640: 332c 2030 5d5d 2c20 5b31 2c20 312c 2031  3, 0]], [1, 1, 1
+0000a650: 2c20 315d 290a 0a20 2020 2020 2020 2070  , 1])..        p
+0000a660: 726f 662e 6469 7370 6c61 7928 290a 0a20  rof.display().. 
+0000a670: 2020 2020 2020 2072 616e 6b65 645f 7061         ranked_pa
+0000a680: 6972 735f 7462 2e64 6973 706c 6179 2870  irs_tb.display(p
+0000a690: 726f 6629 0a20 2020 2020 2020 2072 616e  rof).        ran
+0000a6a0: 6b65 645f 7061 6972 735f 7462 2e64 6973  ked_pairs_tb.dis
+0000a6b0: 706c 6179 2870 726f 662c 2074 6965 5f62  play(prof, tie_b
+0000a6c0: 7265 616b 6572 203d 205b 332c 2032 2c20  reaker = [3, 2, 
+0000a6d0: 312c 2030 5d29 0a20 2020 2020 2020 2072  1, 0]).        r
+0000a6e0: 616e 6b65 645f 7061 6972 735f 7a74 2e64  anked_pairs_zt.d
+0000a6f0: 6973 706c 6179 2870 726f 6629 0a0a 2020  isplay(prof)..  
+0000a700: 2020 2222 220a 0a20 2020 2063 616e 6469    """..    candi
+0000a710: 6461 7465 7320 3d20 6564 6174 612e 6361  dates = edata.ca
+0000a720: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+0000a730: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+0000a740: 6c73 6520 6375 7272 5f63 616e 6473 2020  lse curr_cands  
+0000a750: 2020 0a20 2020 2063 6964 785f 746f 5f63    .    cidx_to_c
+0000a760: 616e 6420 3d20 7b63 6964 783a 2063 2066  and = {cidx: c f
+0000a770: 6f72 2063 6964 782c 2063 2069 6e20 656e  or cidx, c in en
+0000a780: 756d 6572 6174 6528 6361 6e64 6964 6174  umerate(candidat
+0000a790: 6573 297d 2020 0a20 2020 2063 616e 645f  es)}  .    cand_
+0000a7a0: 746f 5f63 6964 7820 3d20 7b63 3a20 6369  to_cidx = {c: ci
+0000a7b0: 6478 2066 6f72 2063 6964 782c 2063 2069  dx for cidx, c i
+0000a7c0: 6e20 656e 756d 6572 6174 6528 6361 6e64  n enumerate(cand
+0000a7d0: 6964 6174 6573 297d 2020 0a0a 2020 2020  idates)}  ..    
+0000a7e0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000a7f0: 6e20 3d20 6564 6174 612e 6d61 7267 696e  n = edata.margin
+0000a800: 2069 6620 7374 7265 6e67 7468 5f66 756e   if strength_fun
+0000a810: 6374 696f 6e20 6973 204e 6f6e 6520 656c  ction is None el
+0000a820: 7365 2073 7472 656e 6774 685f 6675 6e63  se strength_func
+0000a830: 7469 6f6e 0a20 2020 200a 2020 2020 7462  tion.    .    tb
+0000a840: 5f72 616e 6b69 6e67 203d 2074 6965 5f62  _ranking = tie_b
+0000a850: 7265 616b 6572 2069 6620 7469 655f 6272  reaker if tie_br
+0000a860: 6561 6b65 7220 6973 206e 6f74 204e 6f6e  eaker is not Non
+0000a870: 6520 656c 7365 2073 6f72 7465 6428 6c69  e else sorted(li
+0000a880: 7374 2863 616e 6469 6461 7465 7329 290a  st(candidates)).
+0000a890: 0a20 2020 2063 7720 3d20 6564 6174 612e  .    cw = edata.
+0000a8a0: 636f 6e64 6f72 6365 745f 7769 6e6e 6572  condorcet_winner
+0000a8b0: 2863 7572 725f 6361 6e64 733d 6375 7272  (curr_cands=curr
+0000a8c0: 5f63 616e 6473 290a 2020 2020 2320 5261  _cands).    # Ra
+0000a8d0: 6e6b 6564 2050 6169 7273 2069 7320 436f  nked Pairs is Co
+0000a8e0: 6e64 6f72 6365 7420 636f 6e73 6973 7465  ndorcet consiste
+0000a8f0: 6e74 2c20 736f 2073 696d 706c 7920 7265  nt, so simply re
+0000a900: 7475 726e 2074 6865 2043 6f6e 646f 7263  turn the Condorc
+0000a910: 6574 2077 696e 6e65 7220 6966 2065 7869  et winner if exi
+0000a920: 7374 730a 2020 2020 6966 2063 7720 6973  sts.    if cw is
+0000a930: 206e 6f74 204e 6f6e 653a 200a 2020 2020   not None: .    
+0000a940: 2020 2020 7769 6e6e 6572 7320 3d20 5b63      winners = [c
+0000a950: 775d 0a20 2020 2065 6c73 653a 0a20 2020  w].    else:.   
+0000a960: 2020 2020 2077 5f65 6467 6573 203d 205b       w_edges = [
+0000a970: 2863 312c 2063 322c 2073 7472 656e 6774  (c1, c2, strengt
+0000a980: 685f 6675 6e63 7469 6f6e 2863 312c 2063  h_function(c1, c
+0000a990: 3229 2920 666f 7220 6331 2069 6e20 6361  2)) for c1 in ca
+0000a9a0: 6e64 6964 6174 6573 2066 6f72 2063 3220  ndidates for c2 
+0000a9b0: 696e 2063 616e 6469 6461 7465 7320 0a20  in candidates . 
+0000a9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a9d0: 2020 6966 2063 3120 213d 2063 3220 616e    if c1 != c2 an
+0000a9e0: 6420 2865 6461 7461 2e6d 616a 6f72 6974  d (edata.majorit
+0000a9f0: 795f 7072 6566 6572 7328 6331 2c20 6332  y_prefers(c1, c2
+0000aa00: 2920 6f72 2065 6461 7461 2e69 735f 7469  ) or edata.is_ti
+0000aa10: 6564 2863 312c 2063 3229 295d 0a20 2020  ed(c1, c2))].   
+0000aa20: 2020 2020 2077 696e 6e65 7273 203d 206c       winners = l
+0000aa30: 6973 7428 2920 2020 2020 2020 2020 2020  ist()           
+0000aa40: 200a 2020 2020 2020 2020 7374 7265 6e67   .        streng
+0000aa50: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
+0000aa60: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
+0000aa70: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
+0000aa80: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
+0000aa90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+0000aaa0: 7270 5f64 6566 6561 7420 3d20 5350 4f28  rp_defeat = SPO(
+0000aab0: 6c65 6e28 6361 6e64 6964 6174 6573 2929  len(candidates))
+0000aac0: 0a0a 2020 2020 2020 2020 666f 7220 7320  ..        for s 
+0000aad0: 696e 2073 7472 656e 6774 6873 3a20 0a20  in strengths: . 
+0000aae0: 2020 2020 2020 2020 2020 2065 6467 6573             edges
+0000aaf0: 203d 205b 6520 666f 7220 6520 696e 2077   = [e for e in w
+0000ab00: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+0000ab10: 3d20 735d 0a20 2020 2020 2020 2020 2020  = s].           
+0000ab20: 200a 2020 2020 2020 2020 2020 2020 2320   .            # 
+0000ab30: 6272 6561 6b20 7469 6573 2075 7369 6e67  break ties using
+0000ab40: 2074 6865 206c 6578 6963 6f67 7261 7068   the lexicograph
+0000ab50: 6963 206f 7264 6572 696e 6720 6f6e 2074  ic ordering on t
+0000ab60: 7570 6c65 7320 6769 7665 6e20 7462 5f72  uples given tb_r
+0000ab70: 616e 6b69 6e67 0a20 2020 2020 2020 2020  anking.         
+0000ab80: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+0000ab90: 3d20 736f 7274 6564 2865 6467 6573 2c20  = sorted(edges, 
+0000aba0: 6b65 7920 3d20 6c61 6d62 6461 2065 3a20  key = lambda e: 
+0000abb0: 2874 625f 7261 6e6b 696e 672e 696e 6465  (tb_ranking.inde
+0000abc0: 7828 655b 305d 292c 2074 625f 7261 6e6b  x(e[0]), tb_rank
+0000abd0: 696e 672e 696e 6465 7828 655b 315d 2929  ing.index(e[1]))
+0000abe0: 2c20 7265 7665 7273 653d 4661 6c73 6529  , reverse=False)
+0000abf0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000ac00: 2065 302c 6531 2c73 2069 6e20 6564 6765   e0,e1,s in edge
+0000ac10: 733a 200a 2020 2020 2020 2020 2020 2020  s: .            
+0000ac20: 2020 2020 6966 206e 6f74 2072 705f 6465      if not rp_de
+0000ac30: 6665 6174 2e50 5b63 616e 645f 746f 5f63  feat.P[cand_to_c
+0000ac40: 6964 785b 6531 5d5d 5b63 616e 645f 746f  idx[e1]][cand_to
+0000ac50: 5f63 6964 785b 6530 5d5d 3a0a 2020 2020  _cidx[e0]]:.    
+0000ac60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac70: 7270 5f64 6566 6561 742e 6164 6428 6361  rp_defeat.add(ca
+0000ac80: 6e64 5f74 6f5f 6369 6478 5b65 305d 2c63  nd_to_cidx[e0],c
+0000ac90: 616e 645f 746f 5f63 6964 785b 6531 5d29  and_to_cidx[e1])
+0000aca0: 0a20 2020 2020 2020 2020 2020 2077 696e  .            win
+0000acb0: 6e65 7273 2e61 7070 656e 6428 6369 6478  ners.append(cidx
+0000acc0: 5f74 6f5f 6361 6e64 5b72 705f 6465 6665  _to_cand[rp_defe
+0000acd0: 6174 2e69 6e69 7469 616c 5f65 6c65 6d65  at.initial_eleme
+0000ace0: 6e74 7328 295b 305d 5d29 0a0a 2020 2020  nts()[0]])..    
+0000acf0: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
+0000ad00: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
+0000ad10: 290a 0a40 766d 286e 616d 653d 2252 616e  )..@vm(name="Ran
+0000ad20: 6b65 6420 5061 6972 7320 5a54 222c 0a20  ked Pairs ZT",. 
+0000ad30: 2020 2069 6e70 7574 5f74 7970 6573 3d5b     input_types=[
+0000ad40: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
+0000ad50: 4f46 494c 455d 290a 6465 6620 7261 6e6b  OFILE]).def rank
+0000ad60: 6564 5f70 6169 7273 5f7a 7428 0a20 2020  ed_pairs_zt(.   
+0000ad70: 2070 726f 6669 6c65 2c20 0a20 2020 2063   profile, .    c
+0000ad80: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+0000ad90: 2c20 0a20 2020 2073 7472 656e 6774 685f  , .    strength_
+0000ada0: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+0000adb0: 3a20 2020 0a20 2020 2022 2222 5261 6e6b  :   .    """Rank
+0000adc0: 6564 2070 6169 7273 2077 6865 7265 2061  ed pairs where a
+0000add0: 2066 6978 6564 2076 6f74 6572 2062 7265   fixed voter bre
+0000ade0: 616b 7320 616e 7920 7469 6573 2069 6e20  aks any ties in 
+0000adf0: 7468 6520 6d61 7267 696e 732e 2020 4974  the margins.  It
+0000ae00: 2069 7320 616c 7761 7973 2074 6865 2076   is always the v
+0000ae10: 6f74 6572 2069 6e20 706f 7369 7469 6f6e  oter in position
+0000ae20: 2030 2074 6861 7420 6272 6561 6b73 2074   0 that breaks t
+0000ae30: 6865 2074 6965 732e 2020 5369 6e63 6520  he ties.  Since 
+0000ae40: 766f 7465 7273 2068 6176 6520 7374 7269  voters have stri
+0000ae50: 6374 2070 7265 6665 7265 6e63 6573 2c20  ct preferences, 
+0000ae60: 7468 6973 206d 6574 686f 6420 6973 2072  this method is r
+0000ae70: 6573 6f6c 7574 652e 2020 5468 6973 2069  esolute.  This i
+0000ae80: 7320 6b6e 6f77 6e20 6173 2052 616e 6b65  s known as Ranke
+0000ae90: 6420 5061 6972 7320 5a54 2c20 666f 7220  d Pairs ZT, for 
+0000aea0: 5a61 7669 7374 2054 6964 656d 616e 2e0a  Zavist Tideman..
+0000aeb0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+0000aec0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
+0000aed0: 6529 3a20 4120 7072 6f66 696c 6520 6f66  e): A profile of
+0000aee0: 206c 696e 6561 7220 6f72 6465 7273 0a20   linear orders. 
+0000aef0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
+0000af00: 7320 284c 6973 745b 696e 745d 2c20 6f70  s (List[int], op
+0000af10: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
+0000af20: 2074 6865 6e20 6669 6e64 2074 6865 2077   then find the w
+0000af30: 696e 6e65 7273 2066 6f72 2074 6865 2070  inners for the p
+0000af40: 726f 6669 6c65 2072 6573 7472 6963 7465  rofile restricte
+0000af50: 6420 746f 2074 6865 2063 616e 6469 6461  d to the candida
+0000af60: 7465 7320 696e 2060 6063 7572 725f 6361  tes in ``curr_ca
+0000af70: 6e64 7360 600a 0a20 2020 2052 6574 7572  nds``..    Retur
+0000af80: 6e73 3a20 0a20 2020 2020 2020 2041 2073  ns: .        A s
+0000af90: 6f72 7465 6420 6c69 7374 206f 6620 6361  orted list of ca
+0000afa0: 6e64 6964 6174 6573 2e20 0a0a 2020 2020  ndidates. ..    
+0000afb0: 2e2e 2073 6565 616c 736f 3a3a 0a0a 2020  .. seealso::..  
+0000afc0: 2020 2020 2020 3a6d 6574 683a 6070 7265        :meth:`pre
+0000afd0: 665f 766f 7469 6e67 2e6d 6172 6769 6e5f  f_voting.margin_
+0000afe0: 6261 7365 645f 6d65 7468 6f64 732e 7261  based_methods.ra
+0000aff0: 6e6b 6564 5f70 6169 7273 602c 203a 6d65  nked_pairs`, :me
+0000b000: 7468 3a60 7072 6566 5f76 6f74 696e 672e  th:`pref_voting.
+0000b010: 6d61 7267 696e 5f62 6173 6564 5f6d 6574  margin_based_met
+0000b020: 686f 6473 2e72 616e 6b65 645f 7061 6972  hods.ranked_pair
+0000b030: 735f 7769 7468 5f74 6573 7460 0a0a 2020  s_with_test`..  
+0000b040: 2020 2e2e 2065 7865 635f 636f 6465 3a3a    .. exec_code::
+0000b050: 0a0a 2020 2020 2020 2020 6672 6f6d 2070  ..        from p
+0000b060: 7265 665f 766f 7469 6e67 2e70 726f 6669  ref_voting.profi
+0000b070: 6c65 7320 696d 706f 7274 2050 726f 6669  les import Profi
+0000b080: 6c65 0a20 2020 2020 2020 2066 726f 6d20  le.        from 
+0000b090: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
+0000b0a0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
+0000b0b0: 2069 6d70 6f72 7420 7261 6e6b 6564 5f70   import ranked_p
+0000b0c0: 6169 7273 5f74 622c 2072 616e 6b65 645f  airs_tb, ranked_
+0000b0d0: 7061 6972 735f 7a74 0a0a 2020 2020 2020  pairs_zt..      
+0000b0e0: 2020 7072 6f66 203d 2050 726f 6669 6c65    prof = Profile
+0000b0f0: 285b 5b32 2c20 332c 2031 2c20 305d 2c20  ([[2, 3, 1, 0], 
+0000b100: 5b30 2c20 332c 2031 2c20 325d 2c20 5b31  [0, 3, 1, 2], [1
+0000b110: 2c20 332c 2032 2c20 305d 2c20 5b32 2c20  , 3, 2, 0], [2, 
+0000b120: 312c 2033 2c20 305d 5d2c 205b 312c 2031  1, 3, 0]], [1, 1
+0000b130: 2c20 312c 2031 5d29 0a0a 2020 2020 2020  , 1, 1])..      
+0000b140: 2020 7072 6f66 2e64 6973 706c 6179 2829    prof.display()
+0000b150: 0a0a 2020 2020 2020 2020 7261 6e6b 6564  ..        ranked
+0000b160: 5f70 6169 7273 5f74 622e 6469 7370 6c61  _pairs_tb.displa
+0000b170: 7928 7072 6f66 290a 2020 2020 2020 2020  y(prof).        
+0000b180: 7261 6e6b 6564 5f70 6169 7273 5f74 622e  ranked_pairs_tb.
+0000b190: 6469 7370 6c61 7928 7072 6f66 2c20 7469  display(prof, ti
+0000b1a0: 655f 6272 6561 6b65 7220 3d20 5b33 2c20  e_breaker = [3, 
+0000b1b0: 322c 2031 2c20 305d 290a 2020 2020 2020  2, 1, 0]).      
+0000b1c0: 2020 7261 6e6b 6564 5f70 6169 7273 5f7a    ranked_pairs_z
+0000b1d0: 742e 6469 7370 6c61 7928 7072 6f66 290a  t.display(prof).
+0000b1e0: 0a20 2020 200a 2020 2020 2222 220a 2020  .    .    """.  
+0000b1f0: 2020 6361 6e64 6964 6174 6573 203d 2070    candidates = p
+0000b200: 726f 6669 6c65 2e63 616e 6469 6461 7465  rofile.candidate
+0000b210: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
+0000b220: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
+0000b230: 725f 6361 6e64 7320 2020 200a 2020 2020  r_cands    .    
+0000b240: 0a20 2020 2023 2074 6865 2074 6965 2d62  .    # the tie-b
+0000b250: 7265 616b 6572 2069 7320 616c 7761 7973  reaker is always
+0000b260: 2074 6865 2066 6972 7374 2076 6f74 6572   the first voter
+0000b270: 2e20 0a20 2020 2074 625f 7261 6e6b 696e  . .    tb_rankin
+0000b280: 6720 3d20 7475 706c 6528 5b63 2066 6f72  g = tuple([c for
+0000b290: 2063 2069 6e20 6c69 7374 2870 726f 6669   c in list(profi
+0000b2a0: 6c65 2e5f 7261 6e6b 696e 6773 5b30 5d29  le._rankings[0])
+0000b2b0: 2069 6620 6320 696e 2063 616e 6469 6461   if c in candida
+0000b2c0: 7465 735d 290a 2020 2020 0a20 2020 2072  tes]).    .    r
+0000b2d0: 6574 7572 6e20 7261 6e6b 6564 5f70 6169  eturn ranked_pai
+0000b2e0: 7273 5f74 6228 7072 6f66 696c 652c 2063  rs_tb(profile, c
+0000b2f0: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000b300: 5f63 616e 6473 2c20 7469 655f 6272 6561  _cands, tie_brea
+0000b310: 6b65 7220 3d20 7462 5f72 616e 6b69 6e67  ker = tb_ranking
+0000b320: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+0000b330: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
+0000b340: 756e 6374 696f 6e29 0a0a 4076 6d28 6e61  unction)..@vm(na
+0000b350: 6d65 3d22 5269 7665 7222 2c0a 2020 2020  me="River",.    
+0000b360: 696e 7075 745f 7479 7065 733d 5b45 6c65  input_types=[Ele
+0000b370: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
+0000b380: 4c45 2c20 456c 6563 7469 6f6e 5479 7065  LE, ElectionType
+0000b390: 732e 5052 4f46 494c 455f 5749 5448 5f54  s.PROFILE_WITH_T
+0000b3a0: 4945 532c 2045 6c65 6374 696f 6e54 7970  IES, ElectionTyp
+0000b3b0: 6573 2e4d 4152 4749 4e5f 4752 4150 485d  es.MARGIN_GRAPH]
+0000b3c0: 290a 6465 6620 7269 7665 7228 6564 6174  ).def river(edat
+0000b3d0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
+0000b3e0: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
+0000b3f0: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
+0000b400: 2020 200a 2020 2020 2222 220a 2020 2020     .    """.    
+0000b410: 4f72 6465 7220 7468 6520 6564 6765 7320  Order the edges 
+0000b420: 696e 2074 6865 2077 6561 6b20 6d61 7267  in the weak marg
+0000b430: 696e 2067 7261 7068 2066 726f 6d20 6c61  in graph from la
+0000b440: 7267 6573 7420 746f 2073 6d61 6c6c 6573  rgest to smalles
+0000b450: 7420 616e 6420 6c6f 636b 2074 6865 6d20  t and lock them 
+0000b460: 696e 2069 6e20 7468 6174 206f 7264 6572  in in that order
+0000b470: 2c20 736b 6970 7069 6e67 2065 6467 6573  , skipping edges
+0000b480: 2074 6861 7420 6372 6561 7465 2061 2063   that create a c
+0000b490: 7963 6c65 202a 616e 6420 6564 6765 7320  ycle *and edges 
+0000b4a0: 696e 2077 6869 6368 2074 6865 7265 2069  in which there i
+0000b4b0: 7320 616c 7265 6164 7920 616e 2065 6467  s already an edg
+0000b4c0: 6520 706f 696e 7469 6e67 2074 6f20 7468  e pointing to th
+0000b4d0: 6520 7461 7267 6574 2a2e 2020 4272 6561  e target*.  Brea
+0000b4e0: 6b20 7469 6573 2075 7369 6e67 2061 2074  k ties using a t
+0000b4f0: 6965 2d62 7265 616b 696e 6720 206c 696e  ie-breaking  lin
+0000b500: 6561 7220 6f72 6465 7269 6e67 206f 7665  ear ordering ove
+0000b510: 7220 7468 6520 6564 6765 732e 2020 4120  r the edges.  A 
+0000b520: 6361 6e64 6964 6174 6520 6973 2061 2052  candidate is a R
+0000b530: 6976 6572 2077 696e 6e65 7220 6966 2069  iver winner if i
+0000b540: 7420 7769 6e73 2061 6363 6f72 6469 6e67  t wins according
+0000b550: 2074 6f20 736f 6d65 2074 6965 2d62 7265   to some tie-bre
+0000b560: 616b 696e 6720 7275 6c65 2e20 5365 6520  aking rule. See 
+0000b570: 6874 7470 733a 2f2f 656c 6563 746f 7769  https://electowi
+0000b580: 6b69 2e6f 7267 2f77 696b 692f 5269 7665  ki.org/wiki/Rive
+0000b590: 722e 0a0a 2020 2020 4172 6773 3a0a 2020  r...    Args:.  
+0000b5a0: 2020 2020 2020 6564 6174 6120 2850 726f        edata (Pro
+0000b5b0: 6669 6c65 2c20 5072 6f66 696c 6557 6974  file, ProfileWit
+0000b5c0: 6854 6965 732c 204d 6172 6769 6e47 7261  hTies, MarginGra
+0000b5d0: 7068 293a 2041 6e79 2065 6c65 6374 696f  ph): Any electio
+0000b5e0: 6e20 6461 7461 2074 6861 7420 6861 7320  n data that has 
+0000b5f0: 6120 606d 6172 6769 6e60 206d 6574 686f  a `margin` metho
+0000b600: 642e 200a 2020 2020 2020 2020 6375 7272  d. .        curr
+0000b610: 5f63 616e 6473 2028 4c69 7374 5b69 6e74  _cands (List[int
+0000b620: 5d2c 206f 7074 696f 6e61 6c29 3a20 4966  ], optional): If
+0000b630: 2073 6574 2c20 7468 656e 2066 696e 6420   set, then find 
+0000b640: 7468 6520 7769 6e6e 6572 7320 666f 7220  the winners for 
+0000b650: 7468 6520 7072 6f66 696c 6520 7265 7374  the profile rest
+0000b660: 7269 6374 6564 2074 6f20 7468 6520 6361  ricted to the ca
+0000b670: 6e64 6964 6174 6573 2069 6e20 6060 6375  ndidates in ``cu
+0000b680: 7272 5f63 616e 6473 6060 0a20 2020 2020  rr_cands``.     
+0000b690: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000b6a0: 7469 6f6e 2028 6675 6e63 7469 6f6e 2c20  tion (function, 
+0000b6b0: 6f70 7469 6f6e 616c 293a 2054 6865 2073  optional): The s
+0000b6c0: 7472 656e 6774 6820 6675 6e63 7469 6f6e  trength function
+0000b6d0: 2074 6f20 6265 2075 7365 6420 746f 2063   to be used to c
+0000b6e0: 616c 6375 6c61 7465 2074 6865 2073 7472  alculate the str
+0000b6f0: 656e 6774 6820 6f66 2061 2070 6174 682e  ength of a path.
+0000b700: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+0000b710: 7320 7468 6520 6d61 7267 696e 206d 6574  s the margin met
+0000b720: 686f 6420 6f66 2060 6065 6461 7461 6060  hod of ``edata``
+0000b730: 2e20 2020 5468 6973 206f 6e6c 7920 6d61  .   This only ma
+0000b740: 7474 6572 7320 7768 656e 2074 6865 2062  tters when the b
+0000b750: 616c 6c6f 7473 2061 7265 206e 6f74 206c  allots are not l
+0000b760: 696e 6561 7220 6f72 6465 7273 2e20 0a0a  inear orders. ..
+0000b770: 2020 2020 5265 7475 726e 733a 200a 2020      Returns: .  
+0000b780: 2020 2020 2020 4120 736f 7274 6564 206c        A sorted l
+0000b790: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+0000b7a0: 732e 200a 0a20 2020 203a 4578 616d 706c  s. ..    :Exampl
+0000b7b0: 653a 200a 0a20 2020 202e 2e20 6578 6563  e: ..    .. exec
+0000b7c0: 5f63 6f64 653a 3a20 0a0a 2020 2020 2020  _code:: ..      
+0000b7d0: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
+0000b7e0: 6e67 2e77 6569 6768 7465 645f 6d61 6a6f  ng.weighted_majo
+0000b7f0: 7269 7479 5f67 7261 7068 7320 696d 706f  rity_graphs impo
+0000b800: 7274 204d 6172 6769 6e47 7261 7068 0a20  rt MarginGraph. 
+0000b810: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+0000b820: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+0000b830: 6173 6564 5f6d 6574 686f 6473 2069 6d70  ased_methods imp
+0000b840: 6f72 7420 7269 7665 722c 2072 616e 6b65  ort river, ranke
+0000b850: 645f 7061 6972 730a 2020 2020 2020 2020  d_pairs.        
+0000b860: 0a20 2020 2020 2020 206d 6720 3d20 4d61  .        mg = Ma
+0000b870: 7267 696e 4772 6170 6828 5b30 2c20 312c  rginGraph([0, 1,
+0000b880: 2032 2c20 335d 2c20 5b28 302c 2032 2c20   2, 3], [(0, 2, 
+0000b890: 3229 2c20 2830 2c20 332c 2038 292c 2028  2), (0, 3, 8), (
+0000b8a0: 312c 2030 2c20 3132 292c 2028 322c 2033  1, 0, 12), (2, 3
+0000b8b0: 2c20 3132 292c 2028 332c 2031 2c20 3629  , 12), (3, 1, 6)
+0000b8c0: 5d29 0a0a 2020 2020 2020 2020 7261 6e6b  ])..        rank
+0000b8d0: 6564 5f70 6169 7273 2e64 6973 706c 6179  ed_pairs.display
+0000b8e0: 286d 6729 0a20 2020 2020 2020 2072 6976  (mg).        riv
+0000b8f0: 6572 2e64 6973 706c 6179 286d 6729 0a0a  er.display(mg)..
+0000b900: 2020 2020 2222 220a 2020 2020 6361 6e64      """.    cand
+0000b910: 6964 6174 6573 203d 2065 6461 7461 2e63  idates = edata.c
+0000b920: 616e 6469 6461 7465 7320 6966 2063 7572  andidates if cur
+0000b930: 725f 6361 6e64 7320 6973 204e 6f6e 6520  r_cands is None 
+0000b940: 656c 7365 2063 7572 725f 6361 6e64 7320  else curr_cands 
+0000b950: 2020 200a 2020 2020 6369 6478 5f74 6f5f     .    cidx_to_
+0000b960: 6361 6e64 203d 207b 6369 6478 3a20 6320  cand = {cidx: c 
+0000b970: 666f 7220 6369 6478 2c20 6320 696e 2065  for cidx, c in e
+0000b980: 6e75 6d65 7261 7465 2863 616e 6469 6461  numerate(candida
+0000b990: 7465 7329 7d20 200a 2020 2020 6361 6e64  tes)}  .    cand
+0000b9a0: 5f74 6f5f 6369 6478 203d 207b 633a 2063  _to_cidx = {c: c
+0000b9b0: 6964 7820 666f 7220 6369 6478 2c20 6320  idx for cidx, c 
+0000b9c0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+0000b9d0: 6469 6461 7465 7329 7d20 200a 0a20 2020  didates)}  ..   
+0000b9e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000b9f0: 6f6e 203d 2065 6461 7461 2e6d 6172 6769  on = edata.margi
+0000ba00: 6e20 6966 2073 7472 656e 6774 685f 6675  n if strength_fu
+0000ba10: 6e63 7469 6f6e 2069 7320 4e6f 6e65 2065  nction is None e
+0000ba20: 6c73 6520 7374 7265 6e67 7468 5f66 756e  lse strength_fun
+0000ba30: 6374 696f 6e20 2020 200a 0a20 2020 2063  ction    ..    c
+0000ba40: 7720 3d20 6564 6174 612e 636f 6e64 6f72  w = edata.condor
+0000ba50: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+0000ba60: 6361 6e64 733d 6375 7272 5f63 616e 6473  cands=curr_cands
+0000ba70: 290a 2020 2020 2320 5261 6e6b 6564 2050  ).    # Ranked P
+0000ba80: 6169 7273 2069 7320 436f 6e64 6f72 6365  airs is Condorce
+0000ba90: 7420 636f 6e73 6973 7465 6e74 2c20 736f  t consistent, so
+0000baa0: 2073 696d 706c 7920 7265 7475 726e 2074   simply return t
+0000bab0: 6865 2043 6f6e 646f 7263 6574 2077 696e  he Condorcet win
+0000bac0: 6e65 7220 6966 2065 7869 7374 730a 2020  ner if exists.  
+0000bad0: 2020 6966 2063 7720 6973 206e 6f74 204e    if cw is not N
+0000bae0: 6f6e 653a 200a 2020 2020 2020 2020 7769  one: .        wi
+0000baf0: 6e6e 6572 7320 3d20 5b63 775d 0a20 2020  nners = [cw].   
+0000bb00: 2065 6c73 653a 0a20 2020 2020 2020 2077   else:.        w
+0000bb10: 5f65 6467 6573 203d 205b 2863 312c 2063  _edges = [(c1, c
+0000bb20: 322c 2073 7472 656e 6774 685f 6675 6e63  2, strength_func
+0000bb30: 7469 6f6e 2863 312c 2063 3229 2920 666f  tion(c1, c2)) fo
+0000bb40: 7220 6331 2069 6e20 6361 6e64 6964 6174  r c1 in candidat
+0000bb50: 6573 2066 6f72 2063 3220 696e 2063 616e  es for c2 in can
+0000bb60: 6469 6461 7465 7320 0a20 2020 2020 2020  didates .       
+0000bb70: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+0000bb80: 3120 213d 2063 3220 616e 6420 2865 6461  1 != c2 and (eda
+0000bb90: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
+0000bba0: 6572 7328 6331 2c20 6332 2920 6f72 2065  ers(c1, c2) or e
+0000bbb0: 6461 7461 2e69 735f 7469 6564 2863 312c  data.is_tied(c1,
+0000bbc0: 2063 3229 295d 0a20 2020 2020 2020 2077   c2))].        w
+0000bbd0: 696e 6e65 7273 203d 206c 6973 7428 2920  inners = list() 
+0000bbe0: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+0000bbf0: 2020 2020 7374 7265 6e67 7468 7320 3d20      strengths = 
+0000bc00: 736f 7274 6564 286c 6973 7428 7365 7428  sorted(list(set(
+0000bc10: 5b65 5b32 5d20 666f 7220 6520 696e 2077  [e[2] for e in w
+0000bc20: 5f65 6467 6573 5d29 292c 2072 6576 6572  _edges])), rever
+0000bc30: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
+0000bc40: 2073 6f72 7465 645f 6564 6765 7320 3d20   sorted_edges = 
+0000bc50: 5b5b 6520 666f 7220 6520 696e 2077 5f65  [[e for e in w_e
+0000bc60: 6467 6573 2069 6620 655b 325d 203d 3d20  dges if e[2] == 
+0000bc70: 735d 2066 6f72 2073 2069 6e20 7374 7265  s] for s in stre
+0000bc80: 6e67 7468 735d 0a20 2020 2020 2020 2074  ngths].        t
+0000bc90: 6273 203d 2070 726f 6475 6374 282a 5b70  bs = product(*[p
+0000bca0: 6572 6d75 7461 7469 6f6e 7328 6564 6765  ermutations(edge
+0000bcb0: 7329 2066 6f72 2065 6467 6573 2069 6e20  s) for edges in 
+0000bcc0: 736f 7274 6564 5f65 6467 6573 5d29 0a20  sorted_edges]). 
+0000bcd0: 2020 2020 2020 2066 6f72 2074 6220 696e         for tb in
+0000bce0: 2074 6273 3a0a 2020 2020 2020 2020 2020   tbs:.          
+0000bcf0: 2020 6564 6765 7320 3d20 666c 6174 7465    edges = flatte
+0000bd00: 6e28 7462 290a 2020 2020 2020 2020 2020  n(tb).          
+0000bd10: 2020 7276 5f64 6566 6561 7420 3d20 5350    rv_defeat = SP
+0000bd20: 4f28 6c65 6e28 6361 6e64 6964 6174 6573  O(len(candidates
+0000bd30: 2929 0a20 2020 2020 2020 2020 2020 2066  )).            f
+0000bd40: 6f72 2065 302c 6531 2c73 2069 6e20 6564  or e0,e1,s in ed
+0000bd50: 6765 733a 200a 2020 2020 2020 2020 2020  ges: .          
+0000bd60: 2020 2020 2020 6966 206e 6f74 2072 765f        if not rv_
+0000bd70: 6465 6665 6174 2e50 5b63 616e 645f 746f  defeat.P[cand_to
+0000bd80: 5f63 6964 785b 6531 5d5d 5b63 616e 645f  _cidx[e1]][cand_
+0000bd90: 746f 5f63 6964 785b 6530 5d5d 2061 6e64  to_cidx[e0]] and
+0000bda0: 206c 656e 2872 765f 6465 6665 6174 2e70   len(rv_defeat.p
+0000bdb0: 7265 6473 5b63 616e 645f 746f 5f63 6964  reds[cand_to_cid
+0000bdc0: 785b 6531 5d5d 2920 3d3d 2030 3a0a 2020  x[e1]]) == 0:.  
+0000bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bde0: 2020 7276 5f64 6566 6561 742e 6164 6428    rv_defeat.add(
+0000bdf0: 6361 6e64 5f74 6f5f 6369 6478 5b65 305d  cand_to_cidx[e0]
+0000be00: 2c63 616e 645f 746f 5f63 6964 785b 6531  ,cand_to_cidx[e1
+0000be10: 5d29 0a20 2020 2020 2020 2020 2020 2077  ]).            w
+0000be20: 696e 6e65 7273 2e61 7070 656e 6428 6369  inners.append(ci
+0000be30: 6478 5f74 6f5f 6361 6e64 5b72 765f 6465  dx_to_cand[rv_de
+0000be40: 6665 6174 2e69 6e69 7469 616c 5f65 6c65  feat.initial_ele
+0000be50: 6d65 6e74 7328 295b 305d 5d29 0a0a 2020  ments()[0]])..  
+0000be60: 2020 7265 7475 726e 2073 6f72 7465 6428    return sorted(
+0000be70: 6c69 7374 2873 6574 2877 696e 6e65 7273  list(set(winners
+0000be80: 2929 290a 0a64 6566 2072 6976 6572 5f64  )))..def river_d
+0000be90: 6566 6561 7473 2865 6461 7461 2c20 6375  efeats(edata, cu
+0000bea0: 7272 5f63 616e 6473 203d 204e 6f6e 652c  rr_cands = None,
+0000beb0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000bec0: 6f6e 203d 204e 6f6e 6529 3a0a 2020 2020  on = None):.    
+0000bed0: 2222 220a 2020 2020 5265 7475 726e 7320  """.    Returns 
+0000bee0: 7468 6520 5269 7665 7220 6465 6665 6174  the River defeat
+0000bef0: 2072 656c 6174 696f 6e73 2070 726f 6475   relations produ
+0000bf00: 6365 6420 6279 2074 6865 2052 6976 6572  ced by the River
+0000bf10: 2061 6c67 6f72 6974 686d 2e0a 0a20 2020   algorithm...   
+0000bf20: 202e 2e20 696d 706f 7274 616e 743a 3a0a   .. important::.
+0000bf30: 2020 2020 2020 2020 556e 6c69 6b65 2074          Unlike t
+0000bf40: 6865 206f 7468 6572 2066 756e 6374 696f  he other functio
+0000bf50: 6e73 2074 6861 7420 7265 7475 726e 2061  ns that return a
+0000bf60: 2073 696e 676c 6520 6465 6665 6174 2072   single defeat r
+0000bf70: 656c 6174 696f 6e2c 2074 6869 7320 7265  elation, this re
+0000bf80: 7475 726e 7320 6120 6c69 7374 206f 6620  turns a list of 
+0000bf90: 6465 6665 6174 2072 656c 6174 696f 6e73  defeat relations
+0000bfa0: 2e20 0a20 2020 2020 2020 200a 2020 2020  . .        .    
+0000bfb0: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000bfc0: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000bfd0: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000bfe0: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000bff0: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000c000: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000c010: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000c020: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000c030: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000c040: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000c050: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000c060: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000c070: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000c080: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000c090: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000c0a0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000c0b0: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000c0c0: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000c0d0: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000c0e0: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000c0f0: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000c100: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000c110: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000c120: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000c130: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000c140: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000c150: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000c160: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000c170: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000c180: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000c190: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000c1a0: 6e65 7477 6f72 6b78 2044 6947 7261 7068  networkx DiGraph
+0000c1b0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+0000c1c0: 6520 5269 7665 7220 6465 6665 6174 2072  e River defeat r
+0000c1d0: 656c 6174 696f 6e2e 200a 2020 2020 2222  elation. .    ""
+0000c1e0: 220a 0a20 2020 2063 616e 6469 6461 7465  "..    candidate
+0000c1f0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+0000c200: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+0000c210: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+0000c220: 6375 7272 5f63 616e 6473 2020 2020 0a20  curr_cands    . 
+0000c230: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000c240: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000c250: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000c260: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000c270: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000c280: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
+0000c290: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+0000c2a0: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+0000c2b0: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+0000c2c0: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+0000c2d0: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+0000c2e0: 616e 6469 6461 7465 7320 6966 2063 3120  andidates if c1 
+0000c2f0: 213d 2063 3220 616e 6420 2865 6461 7461  != c2 and (edata
+0000c300: 2e6d 616a 6f72 6974 795f 7072 6566 6572  .majority_prefer
+0000c310: 7328 6331 2c20 6332 2920 6f72 2065 6461  s(c1, c2) or eda
+0000c320: 7461 2e69 735f 7469 6564 2863 312c 2063  ta.is_tied(c1, c
+0000c330: 3229 295d 0a0a 2020 2020 7374 7265 6e67  2))]..    streng
+0000c340: 7468 7320 3d20 736f 7274 6564 286c 6973  ths = sorted(lis
+0000c350: 7428 7365 7428 5b65 5b32 5d20 666f 7220  t(set([e[2] for 
+0000c360: 6520 696e 2077 5f65 6467 6573 5d29 292c  e in w_edges])),
+0000c370: 2072 6576 6572 7365 3d54 7275 6529 0a20   reverse=True). 
+0000c380: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+0000c390: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
+0000c3a0: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+0000c3b0: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
+0000c3c0: 7265 6e67 7468 735d 0a20 2020 2074 6273  rengths].    tbs
+0000c3d0: 203d 2070 726f 6475 6374 282a 5b70 6572   = product(*[per
+0000c3e0: 6d75 7461 7469 6f6e 7328 6564 6765 7329  mutations(edges)
+0000c3f0: 2066 6f72 2065 6467 6573 2069 6e20 736f   for edges in so
+0000c400: 7274 6564 5f65 6467 6573 5d29 0a0a 2020  rted_edges])..  
+0000c410: 2020 7269 7665 725f 6465 6665 6174 7320    river_defeats 
+0000c420: 3d20 6c69 7374 2829 0a20 2020 2066 6f72  = list().    for
+0000c430: 2074 6220 696e 2074 6273 3a0a 2020 2020   tb in tbs:.    
+0000c440: 2020 2020 6564 6765 7320 3d20 666c 6174      edges = flat
+0000c450: 7465 6e28 7462 290a 2020 2020 2020 2020  ten(tb).        
+0000c460: 7269 7665 725f 6465 6665 6174 203d 206e  river_defeat = n
+0000c470: 782e 4469 4772 6170 6828 2920 0a20 2020  x.DiGraph() .   
+0000c480: 2020 2020 2066 6f72 2065 2069 6e20 6564       for e in ed
+0000c490: 6765 733a 200a 2020 2020 2020 2020 2020  ges: .          
+0000c4a0: 2020 6966 2065 5b31 5d20 6e6f 7420 696e    if e[1] not in
+0000c4b0: 2072 6976 6572 5f64 6566 6561 742e 6e6f   river_defeat.no
+0000c4c0: 6465 7320 6f72 206c 656e 286c 6973 7428  des or len(list(
+0000c4d0: 7269 7665 725f 6465 6665 6174 2e69 6e5f  river_defeat.in_
+0000c4e0: 6564 6765 7328 655b 315d 2929 2920 3d3d  edges(e[1]))) ==
+0000c4f0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+0000c500: 2020 2020 7269 7665 725f 6465 6665 6174      river_defeat
+0000c510: 2e61 6464 5f65 6467 6528 655b 305d 2c20  .add_edge(e[0], 
+0000c520: 655b 315d 2c20 7765 6967 6874 3d65 5b32  e[1], weight=e[2
+0000c530: 5d29 0a20 2020 2020 2020 2020 2020 2020  ]).             
+0000c540: 2020 2069 6620 646f 6573 5f63 7265 6174     if does_creat
+0000c550: 655f 6379 636c 6528 7269 7665 725f 6465  e_cycle(river_de
+0000c560: 6665 6174 2c20 6529 3a0a 2020 2020 2020  feat, e):.      
+0000c570: 2020 2020 2020 2020 2020 2020 2020 7269                ri
+0000c580: 7665 725f 6465 6665 6174 2e72 656d 6f76  ver_defeat.remov
+0000c590: 655f 6564 6765 2865 5b30 5d2c 2065 5b31  e_edge(e[0], e[1
+0000c5a0: 5d29 0a20 2020 2020 2020 2020 2020 200a  ]).            .
+0000c5b0: 2020 2020 2020 2020 7269 7665 725f 6465          river_de
+0000c5c0: 6665 6174 732e 6170 7065 6e64 2872 6976  feats.append(riv
+0000c5d0: 6572 5f64 6566 6561 7429 0a0a 2020 2020  er_defeat)..    
+0000c5e0: 7265 7475 726e 2072 6976 6572 5f64 6566  return river_def
+0000c5f0: 6561 7473 0a0a 4076 6d28 6e61 6d65 3d22  eats..@vm(name="
+0000c600: 5269 7665 7222 2c0a 2020 2020 736b 6970  River",.    skip
+0000c610: 5f72 6567 6973 7472 6174 696f 6e3d 5472  _registration=Tr
+0000c620: 7565 290a 6465 6620 7269 7665 725f 7769  ue).def river_wi
+0000c630: 7468 5f74 6573 7428 6564 6174 612c 2063  th_test(edata, c
+0000c640: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+0000c650: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+0000c660: 696f 6e20 3d20 4e6f 6e65 293a 2020 200a  ion = None):   .
+0000c670: 2020 2020 2222 2246 696e 6420 7468 6520      """Find the 
+0000c680: 5269 7665 7220 7769 6e6e 6572 7320 7769  River winners wi
+0000c690: 7468 2061 2074 6573 7420 746f 2064 6574  th a test to det
+0000c6a0: 6572 6d69 6e65 6420 6966 2069 7420 7769  ermined if it wi
+0000c6b0: 6c6c 2074 616b 6520 746f 6f20 6c6f 6e67  ll take too long
+0000c6c0: 2074 6f20 636f 6d70 7574 6520 7468 6520   to compute the 
+0000c6d0: 5269 7665 7220 7769 6e6e 6572 732e 2049  River winners. I
+0000c6e0: 6620 7468 6520 6361 6c63 756c 6174 696f  f the calculatio
+0000c6f0: 6e20 6f66 2074 6865 2077 696e 6e65 7273  n of the winners
+0000c700: 2077 696c 6c20 7461 6b65 2074 6f6f 206c   will take too l
+0000c710: 6f6e 672c 2072 6574 7572 6e20 4e6f 6e65  ong, return None
+0000c720: 2e20 0a20 2020 2020 2020 200a 2020 2020  . .        .    
+0000c730: 2e2e 2069 6d70 6f72 7461 6e74 3a3a 0a20  .. important::. 
+0000c740: 2020 2020 2020 2054 6869 7320 766f 7469         This voti
+0000c750: 6e67 206d 6574 686f 6420 7468 6174 206d  ng method that m
+0000c760: 6967 6874 2072 6574 7572 6e20 4e6f 6e65  ight return None
+0000c770: 2072 6174 6865 7220 7468 616e 2061 206c   rather than a l
+0000c780: 6973 7420 6f66 2063 616e 6469 6461 7465  ist of candidate
+0000c790: 732e 2020 0a0a 2020 2020 4172 6773 3a0a  s.  ..    Args:.
+0000c7a0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000c7b0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000c7c0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000c7d0: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000c7e0: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000c7f0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000c800: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000c810: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000c820: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000c830: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000c840: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000c850: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000c860: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000c870: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000c880: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000c890: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000c8a0: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+0000c8b0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000c8c0: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+0000c8d0: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+0000c8e0: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+0000c8f0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+0000c900: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+0000c910: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+0000c920: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+0000c930: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+0000c940: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+0000c950: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+0000c960: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+0000c970: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
+0000c980: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
+0000c990: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
+0000c9a0: 7465 732e 200a 0a20 2020 202e 2e20 7365  tes. ..    .. se
+0000c9b0: 6561 6c73 6f3a 3a0a 0a20 2020 2020 2020  ealso::..       
+0000c9c0: 203a 6d65 7468 3a60 7072 6566 5f76 6f74   :meth:`pref_vot
+0000c9d0: 696e 672e 6d61 7267 696e 5f62 6173 6564  ing.margin_based
+0000c9e0: 5f6d 6574 686f 6473 2e72 616e 6b65 645f  _methods.ranked_
+0000c9f0: 7061 6972 735f 7769 7468 5f74 6573 7460  pairs_with_test`
+0000ca00: 2c20 3a6d 6574 683a 6070 7265 665f 766f  , :meth:`pref_vo
+0000ca10: 7469 6e67 2e6d 6172 6769 6e5f 6261 7365  ting.margin_base
+0000ca20: 645f 6d65 7468 6f64 732e 7269 7665 7260  d_methods.river`
+0000ca30: 0a0a 2020 2020 2222 220a 2020 2020 6361  ..    """.    ca
+0000ca40: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
+0000ca50: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000ca60: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000ca70: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000ca80: 7320 2020 200a 2020 2020 6369 6478 5f74  s    .    cidx_t
+0000ca90: 6f5f 6361 6e64 203d 207b 6369 6478 3a20  o_cand = {cidx: 
+0000caa0: 6320 666f 7220 6369 6478 2c20 6320 696e  c for cidx, c in
+0000cab0: 2065 6e75 6d65 7261 7465 2863 616e 6469   enumerate(candi
+0000cac0: 6461 7465 7329 7d20 200a 2020 2020 6361  dates)}  .    ca
+0000cad0: 6e64 5f74 6f5f 6369 6478 203d 207b 633a  nd_to_cidx = {c:
+0000cae0: 2063 6964 7820 666f 7220 6369 6478 2c20   cidx for cidx, 
+0000caf0: 6320 696e 2065 6e75 6d65 7261 7465 2863  c in enumerate(c
+0000cb00: 616e 6469 6461 7465 7329 7d20 200a 0a20  andidates)}  .. 
+0000cb10: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+0000cb20: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+0000cb30: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+0000cb40: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+0000cb50: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+0000cb60: 756e 6374 696f 6e20 2020 200a 0a20 2020  unction    ..   
+0000cb70: 2063 7720 3d20 6564 6174 612e 636f 6e64   cw = edata.cond
+0000cb80: 6f72 6365 745f 7769 6e6e 6572 2863 7572  orcet_winner(cur
+0000cb90: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
+0000cba0: 6473 290a 2020 2020 2320 5261 6e6b 6564  ds).    # Ranked
+0000cbb0: 2050 6169 7273 2069 7320 436f 6e64 6f72   Pairs is Condor
+0000cbc0: 6365 7420 636f 6e73 6973 7465 6e74 2c20  cet consistent, 
+0000cbd0: 736f 2073 696d 706c 7920 7265 7475 726e  so simply return
+0000cbe0: 2074 6865 2043 6f6e 646f 7263 6574 2077   the Condorcet w
+0000cbf0: 696e 6e65 7220 6966 2065 7869 7374 730a  inner if exists.
+0000cc00: 2020 2020 6966 2063 7720 6973 206e 6f74      if cw is not
+0000cc10: 204e 6f6e 653a 200a 2020 2020 2020 2020   None: .        
+0000cc20: 7769 6e6e 6572 7320 3d20 5b63 775d 0a20  winners = [cw]. 
+0000cc30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000cc40: 2077 5f65 6467 6573 203d 205b 2863 312c   w_edges = [(c1,
+0000cc50: 2063 322c 2073 7472 656e 6774 685f 6675   c2, strength_fu
+0000cc60: 6e63 7469 6f6e 2863 312c 2063 3229 2920  nction(c1, c2)) 
+0000cc70: 666f 7220 6331 2069 6e20 6361 6e64 6964  for c1 in candid
+0000cc80: 6174 6573 2066 6f72 2063 3220 696e 2063  ates for c2 in c
+0000cc90: 616e 6469 6461 7465 7320 0a20 2020 2020  andidates .     
+0000cca0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000ccb0: 2063 3120 213d 2063 3220 616e 6420 2865   c1 != c2 and (e
+0000ccc0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
+0000ccd0: 6566 6572 7328 6331 2c20 6332 2920 6f72  efers(c1, c2) or
+0000cce0: 2065 6461 7461 2e69 735f 7469 6564 2863   edata.is_tied(c
+0000ccf0: 312c 2063 3229 295d 0a20 2020 2020 2020  1, c2))].       
+0000cd00: 2077 696e 6e65 7273 203d 206c 6973 7428   winners = list(
+0000cd10: 2920 2020 2020 2020 2020 2020 200a 2020  )            .  
+0000cd20: 2020 2020 2020 7374 7265 6e67 7468 7320        strengths 
+0000cd30: 3d20 736f 7274 6564 286c 6973 7428 7365  = sorted(list(se
+0000cd40: 7428 5b65 5b32 5d20 666f 7220 6520 696e  t([e[2] for e in
+0000cd50: 2077 5f65 6467 6573 5d29 292c 2072 6576   w_edges])), rev
+0000cd60: 6572 7365 3d54 7275 6529 0a20 2020 2020  erse=True).     
+0000cd70: 2020 2073 6f72 7465 645f 6564 6765 7320     sorted_edges 
+0000cd80: 3d20 5b5b 6520 666f 7220 6520 696e 2077  = [[e for e in w
+0000cd90: 5f65 6467 6573 2069 6620 655b 325d 203d  _edges if e[2] =
+0000cda0: 3d20 735d 2066 6f72 2073 2069 6e20 7374  = s] for s in st
+0000cdb0: 7265 6e67 7468 735d 0a20 2020 2020 2020  rengths].       
+0000cdc0: 2069 6620 6e70 2e70 726f 6428 5b6d 6174   if np.prod([mat
+0000cdd0: 682e 6661 6374 6f72 6961 6c28 6c65 6e28  h.factorial(len(
+0000cde0: 6573 2929 2066 6f72 2065 7320 696e 2073  es)) for es in s
+0000cdf0: 6f72 7465 645f 6564 6765 735d 2920 3e20  orted_edges]) > 
+0000ce00: 3330 3030 3a20 0a20 2020 2020 2020 2020  3000: .         
+0000ce10: 2020 2072 6574 7572 6e20 4e6f 6e65 0a20     return None. 
+0000ce20: 2020 2020 2020 2065 6c73 653a 200a 2020         else: .  
+0000ce30: 2020 2020 2020 2020 2020 7462 7320 3d20            tbs = 
+0000ce40: 7072 6f64 7563 7428 2a5b 7065 726d 7574  product(*[permut
+0000ce50: 6174 696f 6e73 2865 6467 6573 2920 666f  ations(edges) fo
+0000ce60: 7220 6564 6765 7320 696e 2073 6f72 7465  r edges in sorte
+0000ce70: 645f 6564 6765 735d 290a 2020 2020 2020  d_edges]).      
+0000ce80: 2020 2020 2020 666f 7220 7462 2069 6e20        for tb in 
+0000ce90: 7462 733a 0a20 2020 2020 2020 2020 2020  tbs:.           
+0000cea0: 2020 2020 2065 6467 6573 203d 2066 6c61       edges = fla
+0000ceb0: 7474 656e 2874 6229 0a20 2020 2020 2020  tten(tb).       
+0000cec0: 2020 2020 2020 2020 2072 765f 6465 6665           rv_defe
+0000ced0: 6174 203d 2053 504f 286c 656e 2863 616e  at = SPO(len(can
+0000cee0: 6469 6461 7465 7329 290a 2020 2020 2020  didates)).      
+0000cef0: 2020 2020 2020 2020 2020 666f 7220 6530            for e0
+0000cf00: 2c65 312c 7320 696e 2065 6467 6573 3a20  ,e1,s in edges: 
+0000cf10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cf20: 2020 2020 2069 6620 6e6f 7420 7276 5f64       if not rv_d
+0000cf30: 6566 6561 742e 505b 6361 6e64 5f74 6f5f  efeat.P[cand_to_
+0000cf40: 6369 6478 5b65 315d 5d5b 6361 6e64 5f74  cidx[e1]][cand_t
+0000cf50: 6f5f 6369 6478 5b65 305d 5d20 616e 6420  o_cidx[e0]] and 
+0000cf60: 6c65 6e28 7276 5f64 6566 6561 742e 7072  len(rv_defeat.pr
+0000cf70: 6564 735b 6361 6e64 5f74 6f5f 6369 6478  eds[cand_to_cidx
+0000cf80: 5b65 315d 5d29 203d 3d20 303a 0a20 2020  [e1]]) == 0:.   
+0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfa0: 2020 2020 2072 765f 6465 6665 6174 2e61       rv_defeat.a
+0000cfb0: 6464 2863 616e 645f 746f 5f63 6964 785b  dd(cand_to_cidx[
+0000cfc0: 6530 5d2c 6361 6e64 5f74 6f5f 6369 6478  e0],cand_to_cidx
+0000cfd0: 5b65 315d 290a 2020 2020 2020 2020 2020  [e1]).          
+0000cfe0: 2020 2020 2020 7769 6e6e 6572 732e 6170        winners.ap
+0000cff0: 7065 6e64 2863 6964 785f 746f 5f63 616e  pend(cidx_to_can
+0000d000: 645b 7276 5f64 6566 6561 742e 696e 6974  d[rv_defeat.init
+0000d010: 6961 6c5f 656c 656d 656e 7473 2829 5b30  ial_elements()[0
+0000d020: 5d5d 290a 2020 2020 7265 7475 726e 2073  ]]).    return s
+0000d030: 6f72 7465 6428 6c69 7374 2873 6574 2877  orted(list(set(w
+0000d040: 696e 6e65 7273 2929 290a 0a40 766d 286e  inners)))..@vm(n
+0000d050: 616d 653d 2252 6976 6572 2054 4222 2c0a  ame="River TB",.
+0000d060: 2020 2020 696e 7075 745f 7479 7065 733d      input_types=
+0000d070: 5b45 6c65 6374 696f 6e54 7970 6573 2e50  [ElectionTypes.P
+0000d080: 524f 4649 4c45 2c20 456c 6563 7469 6f6e  ROFILE, Election
+0000d090: 5479 7065 732e 5052 4f46 494c 455f 5749  Types.PROFILE_WI
+0000d0a0: 5448 5f54 4945 532c 2045 6c65 6374 696f  TH_TIES, Electio
+0000d0b0: 6e54 7970 6573 2e4d 4152 4749 4e5f 4752  nTypes.MARGIN_GR
+0000d0c0: 4150 485d 290a 6465 6620 7269 7665 725f  APH]).def river_
+0000d0d0: 7462 2865 6461 7461 2c20 6375 7272 5f63  tb(edata, curr_c
+0000d0e0: 616e 6473 203d 204e 6f6e 652c 2074 6965  ands = None, tie
+0000d0f0: 5f62 7265 616b 6572 203d 204e 6f6e 652c  _breaker = None,
+0000d100: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000d110: 6f6e 203d 204e 6f6e 6529 3a20 2020 0a20  on = None):   . 
+0000d120: 2020 2022 2222 0a20 2020 2052 6976 6572     """.    River
+0000d130: 2077 6974 6820 6120 6669 7865 6420 6c69   with a fixed li
+0000d140: 6e65 6172 206f 7264 6572 206f 6e20 7468  near order on th
+0000d150: 6520 6361 6e64 6964 6174 6573 2074 6f20  e candidates to 
+0000d160: 6272 6561 6b20 616e 7920 7469 6573 2069  break any ties i
+0000d170: 6e20 7468 6520 6d61 7267 696e 732e 2020  n the margins.  
+0000d180: 5369 6e63 6520 7468 6520 7469 655f 6272  Since the tie_br
+0000d190: 6561 6b65 7220 6973 2061 206c 696e 6561  eaker is a linea
+0000d1a0: 7220 6f72 6465 722c 2074 6869 7320 6d65  r order, this me
+0000d1b0: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
+0000d1c0: 2e20 2020 0a0a 2020 2020 4172 6773 3a0a  .   ..    Args:.
+0000d1d0: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000d1e0: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000d1f0: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000d200: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000d210: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000d220: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000d230: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000d240: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000d250: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000d260: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000d270: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000d280: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000d290: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000d2a0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000d2b0: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000d2c0: 2020 2020 2074 6965 5f62 7265 616b 6572       tie_breaker
+0000d2d0: 2028 4c69 7374 5b69 6e74 5d2c 206f 7074   (List[int], opt
+0000d2e0: 696f 6e61 6c29 3a20 4120 6c69 6e65 6172  ional): A linear
+0000d2f0: 206f 7264 6572 206f 6e20 7468 6520 6361   order on the ca
+0000d300: 6e64 6964 6174 6573 2e20 2049 6620 6e6f  ndidates.  If no
+0000d310: 7420 7365 742c 2074 6865 6e20 7468 6520  t set, then the 
+0000d320: 6361 6e64 6964 6174 6573 2061 7265 2073  candidates are s
+0000d330: 6f72 7465 6420 696e 2061 7363 656e 6469  orted in ascendi
+0000d340: 6e67 206f 7264 6572 2e0a 2020 2020 2020  ng order..      
+0000d350: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
+0000d360: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
+0000d370: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
+0000d380: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
+0000d390: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
+0000d3a0: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
+0000d3b0: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
+0000d3c0: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
+0000d3d0: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
+0000d3e0: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
+0000d3f0: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
+0000d400: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
+0000d410: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
+0000d420: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
+0000d430: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
+0000d440: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
+0000d450: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
+0000d460: 2e20 0a0a 2020 2020 2222 220a 2020 2020  . ..    """.    
+0000d470: 6361 6e64 6964 6174 6573 203d 2065 6461  candidates = eda
+0000d480: 7461 2e63 616e 6469 6461 7465 7320 6966  ta.candidates if
+0000d490: 2063 7572 725f 6361 6e64 7320 6973 204e   curr_cands is N
+0000d4a0: 6f6e 6520 656c 7365 2063 7572 725f 6361  one else curr_ca
+0000d4b0: 6e64 7320 2020 200a 2020 2020 6369 6478  nds    .    cidx
+0000d4c0: 5f74 6f5f 6361 6e64 203d 207b 6369 6478  _to_cand = {cidx
+0000d4d0: 3a20 6320 666f 7220 6369 6478 2c20 6320  : c for cidx, c 
+0000d4e0: 696e 2065 6e75 6d65 7261 7465 2863 616e  in enumerate(can
+0000d4f0: 6469 6461 7465 7329 7d20 200a 2020 2020  didates)}  .    
+0000d500: 6361 6e64 5f74 6f5f 6369 6478 203d 207b  cand_to_cidx = {
+0000d510: 633a 2063 6964 7820 666f 7220 6369 6478  c: cidx for cidx
+0000d520: 2c20 6320 696e 2065 6e75 6d65 7261 7465  , c in enumerate
+0000d530: 2863 616e 6469 6461 7465 7329 7d20 200a  (candidates)}  .
+0000d540: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000d550: 6374 696f 6e20 3d20 6564 6174 612e 6d61  ction = edata.ma
+0000d560: 7267 696e 2069 6620 7374 7265 6e67 7468  rgin if strength
+0000d570: 5f66 756e 6374 696f 6e20 6973 204e 6f6e  _function is Non
+0000d580: 6520 656c 7365 2073 7472 656e 6774 685f  e else strength_
+0000d590: 6675 6e63 7469 6f6e 2020 2020 0a0a 2020  function    ..  
+0000d5a0: 2020 7462 5f72 616e 6b69 6e67 203d 2074    tb_ranking = t
+0000d5b0: 6965 5f62 7265 616b 6572 2069 6620 7469  ie_breaker if ti
+0000d5c0: 655f 6272 6561 6b65 7220 6973 206e 6f74  e_breaker is not
+0000d5d0: 204e 6f6e 6520 656c 7365 2073 6f72 7465   None else sorte
+0000d5e0: 6428 6c69 7374 2863 616e 6469 6461 7465  d(list(candidate
+0000d5f0: 7329 290a 0a20 2020 2063 7720 3d20 6564  s))..    cw = ed
+0000d600: 6174 612e 636f 6e64 6f72 6365 745f 7769  ata.condorcet_wi
+0000d610: 6e6e 6572 2863 7572 725f 6361 6e64 733d  nner(curr_cands=
+0000d620: 6375 7272 5f63 616e 6473 290a 2020 2020  curr_cands).    
+0000d630: 2320 5269 7665 7220 6973 2043 6f6e 646f  # River is Condo
+0000d640: 7263 6574 2063 6f6e 7369 7374 656e 742c  rcet consistent,
+0000d650: 2073 6f20 7369 6d70 6c79 2072 6574 7572   so simply retur
+0000d660: 6e20 7468 6520 436f 6e64 6f72 6365 7420  n the Condorcet 
+0000d670: 7769 6e6e 6572 2069 6620 6578 6973 7473  winner if exists
+0000d680: 0a20 2020 2069 6620 6377 2069 7320 6e6f  .    if cw is no
+0000d690: 7420 4e6f 6e65 3a20 0a20 2020 2020 2020  t None: .       
+0000d6a0: 2077 696e 6e65 7273 203d 205b 6377 5d0a   winners = [cw].
+0000d6b0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d6c0: 2020 775f 6564 6765 7320 3d20 5b28 6331    w_edges = [(c1
+0000d6d0: 2c20 6332 2c20 7374 7265 6e67 7468 5f66  , c2, strength_f
+0000d6e0: 756e 6374 696f 6e28 6331 2c20 6332 2929  unction(c1, c2))
+0000d6f0: 2066 6f72 2063 3120 696e 2063 616e 6469   for c1 in candi
+0000d700: 6461 7465 7320 666f 7220 6332 2069 6e20  dates for c2 in 
+0000d710: 6361 6e64 6964 6174 6573 2069 6620 6331  candidates if c1
+0000d720: 2021 3d20 6332 2061 6e64 2028 6564 6174   != c2 and (edat
+0000d730: 612e 6d61 6a6f 7269 7479 5f70 7265 6665  a.majority_prefe
+0000d740: 7273 2863 312c 2063 3229 206f 7220 6564  rs(c1, c2) or ed
+0000d750: 6174 612e 6973 5f74 6965 6428 6331 2c20  ata.is_tied(c1, 
+0000d760: 6332 2929 5d0a 2020 2020 2020 2020 7769  c2))].        wi
+0000d770: 6e6e 6572 7320 3d20 6c69 7374 2829 2020  nners = list()  
+0000d780: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+0000d790: 6873 203d 2073 6f72 7465 6428 6c69 7374  hs = sorted(list
+0000d7a0: 2873 6574 285b 655b 325d 2066 6f72 2065  (set([e[2] for e
+0000d7b0: 2069 6e20 775f 6564 6765 735d 2929 2c20   in w_edges])), 
+0000d7c0: 7265 7665 7273 653d 5472 7565 290a 0a20  reverse=True).. 
+0000d7d0: 2020 2020 2020 2072 765f 6465 6665 6174         rv_defeat
+0000d7e0: 203d 2053 504f 286c 656e 2863 616e 6469   = SPO(len(candi
+0000d7f0: 6461 7465 7329 290a 0a20 2020 2020 2020  dates))..       
+0000d800: 2066 6f72 2073 2069 6e20 7374 7265 6e67   for s in streng
+0000d810: 7468 733a 200a 2020 2020 2020 2020 2020  ths: .          
+0000d820: 2020 6564 6765 7320 3d20 5b65 2066 6f72    edges = [e for
+0000d830: 2065 2069 6e20 775f 6564 6765 7320 6966   e in w_edges if
+0000d840: 2065 5b32 5d20 3d3d 2073 5d0a 2020 2020   e[2] == s].    
+0000d850: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+0000d860: 2020 2020 2023 2062 7265 616b 2074 6965       # break tie
+0000d870: 7320 7573 696e 6720 7468 6520 6c65 7869  s using the lexi
+0000d880: 636f 6772 6170 6869 6320 6f72 6465 7269  cographic orderi
+0000d890: 6e67 206f 6e20 7475 706c 6573 2067 6976  ng on tuples giv
+0000d8a0: 656e 2074 625f 7261 6e6b 696e 670a 2020  en tb_ranking.  
+0000d8b0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000d8c0: 5f65 6467 6573 203d 2073 6f72 7465 6428  _edges = sorted(
+0000d8d0: 6564 6765 732c 206b 6579 203d 206c 616d  edges, key = lam
+0000d8e0: 6264 6120 653a 2028 7462 5f72 616e 6b69  bda e: (tb_ranki
+0000d8f0: 6e67 2e69 6e64 6578 2865 5b30 5d29 2c20  ng.index(e[0]), 
+0000d900: 7462 5f72 616e 6b69 6e67 2e69 6e64 6578  tb_ranking.index
+0000d910: 2865 5b31 5d29 292c 2072 6576 6572 7365  (e[1])), reverse
+0000d920: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
+0000d930: 2020 2020 666f 7220 6530 2c65 312c 7320      for e0,e1,s 
+0000d940: 696e 2073 6f72 7465 645f 6564 6765 733a  in sorted_edges:
+0000d950: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000d960: 2020 6966 206e 6f74 2072 765f 6465 6665    if not rv_defe
+0000d970: 6174 2e50 5b63 616e 645f 746f 5f63 6964  at.P[cand_to_cid
+0000d980: 785b 6531 5d5d 5b63 616e 645f 746f 5f63  x[e1]][cand_to_c
+0000d990: 6964 785b 6530 5d5d 2061 6e64 206c 656e  idx[e0]] and len
+0000d9a0: 2872 765f 6465 6665 6174 2e70 7265 6473  (rv_defeat.preds
+0000d9b0: 5b63 616e 645f 746f 5f63 6964 785b 6531  [cand_to_cidx[e1
+0000d9c0: 5d5d 2920 3d3d 2030 3a0a 2020 2020 2020  ]]) == 0:.      
+0000d9d0: 2020 2020 2020 2020 2020 2020 2020 7276                rv
+0000d9e0: 5f64 6566 6561 742e 6164 6428 6361 6e64  _defeat.add(cand
+0000d9f0: 5f74 6f5f 6369 6478 5b65 305d 2c63 616e  _to_cidx[e0],can
+0000da00: 645f 746f 5f63 6964 785b 6531 5d29 0a20  d_to_cidx[e1]). 
+0000da10: 2020 2020 2020 2020 2020 2077 696e 6e65             winne
+0000da20: 7273 2e61 7070 656e 6428 6369 6478 5f74  rs.append(cidx_t
+0000da30: 6f5f 6361 6e64 5b72 765f 6465 6665 6174  o_cand[rv_defeat
+0000da40: 2e69 6e69 7469 616c 5f65 6c65 6d65 6e74  .initial_element
+0000da50: 7328 295b 305d 5d29 0a20 2020 2072 6574  s()[0]]).    ret
+0000da60: 7572 6e20 736f 7274 6564 286c 6973 7428  urn sorted(list(
+0000da70: 7365 7428 7769 6e6e 6572 7329 2929 0a0a  set(winners)))..
+0000da80: 4076 6d28 6e61 6d65 3d22 5269 7665 7220  @vm(name="River 
+0000da90: 5a54 222c 0a20 2020 2069 6e70 7574 5f74  ZT",.    input_t
+0000daa0: 7970 6573 3d5b 456c 6563 7469 6f6e 5479  ypes=[ElectionTy
+0000dab0: 7065 732e 5052 4f46 494c 455d 290a 6465  pes.PROFILE]).de
+0000dac0: 6620 7269 7665 725f 7a74 2870 726f 6669  f river_zt(profi
+0000dad0: 6c65 2c20 6375 7272 5f63 616e 6473 203d  le, curr_cands =
+0000dae0: 204e 6f6e 652c 2073 7472 656e 6774 685f   None, strength_
+0000daf0: 6675 6e63 7469 6f6e 203d 204e 6f6e 6529  function = None)
+0000db00: 3a20 2020 0a20 2020 2022 2222 5269 7665  :   .    """Rive
+0000db10: 7220 7768 6572 6520 6120 6669 7865 6420  r where a fixed 
+0000db20: 766f 7465 7220 6272 6561 6b73 2061 6e79  voter breaks any
+0000db30: 2074 6965 7320 696e 2074 6865 206d 6172   ties in the mar
+0000db40: 6769 6e73 2e20 2049 7420 6973 2061 6c77  gins.  It is alw
+0000db50: 6179 7320 7468 6520 766f 7465 7220 696e  ays the voter in
+0000db60: 2070 6f73 6974 696f 6e20 3020 7468 6174   position 0 that
+0000db70: 2062 7265 616b 7320 7468 6520 7469 6573   breaks the ties
+0000db80: 2e20 2053 696e 6365 2076 6f74 6572 7320  .  Since voters 
+0000db90: 6861 7665 2073 7472 6963 7420 7072 6566  have strict pref
+0000dba0: 6572 656e 6365 732c 2074 6869 7320 6d65  erences, this me
+0000dbb0: 7468 6f64 2069 7320 7265 736f 6c75 7465  thod is resolute
+0000dbc0: 2e20 200a 0a20 2020 2041 7267 733a 0a20  .  ..    Args:. 
+0000dbd0: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+0000dbe0: 6f66 696c 6529 3a20 4120 7072 6f66 696c  ofile): A profil
+0000dbf0: 6520 6f66 206c 696e 6561 7220 6f72 6465  e of linear orde
+0000dc00: 7273 0a20 2020 2020 2020 2063 7572 725f  rs.        curr_
+0000dc10: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+0000dc20: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+0000dc30: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+0000dc40: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+0000dc50: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+0000dc60: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+0000dc70: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+0000dc80: 725f 6361 6e64 7360 600a 0a20 2020 2052  r_cands``..    R
+0000dc90: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+0000dca0: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
+0000dcb0: 6620 6361 6e64 6964 6174 6573 2e20 0a0a  f candidates. ..
+0000dcc0: 2020 2020 2e2e 2073 6565 616c 736f 3a3a      .. seealso::
+0000dcd0: 0a0a 2020 2020 2020 2020 3a6d 6574 683a  ..        :meth:
+0000dce0: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+0000dcf0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000dd00: 732e 7269 7665 7260 2c20 3a6d 6574 683a  s.river`, :meth:
+0000dd10: 6070 7265 665f 766f 7469 6e67 2e6d 6172  `pref_voting.mar
+0000dd20: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000dd30: 732e 7269 7665 725f 7769 7468 5f74 6573  s.river_with_tes
+0000dd40: 7460 2c20 3a6d 6574 683a 6070 7265 665f  t`, :meth:`pref_
+0000dd50: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+0000dd60: 7365 645f 6d65 7468 6f64 732e 7261 6e6b  sed_methods.rank
+0000dd70: 6564 5f70 6169 7273 600a 0a20 2020 200a  ed_pairs`..    .
+0000dd80: 2020 2020 2222 220a 2020 2020 6361 6e64      """.    cand
+0000dd90: 6964 6174 6573 203d 2070 726f 6669 6c65  idates = profile
+0000dda0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+0000ddb0: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+0000ddc0: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+0000ddd0: 7320 2020 200a 2020 2020 0a20 2020 2023  s    .    .    #
+0000dde0: 2074 6865 2074 6965 2d62 7265 616b 6572   the tie-breaker
+0000ddf0: 2069 7320 616c 7761 7973 2074 6865 2066   is always the f
+0000de00: 6972 7374 2076 6f74 6572 2e20 0a20 2020  irst voter. .   
+0000de10: 2074 625f 7261 6e6b 696e 6720 3d20 7475   tb_ranking = tu
+0000de20: 706c 6528 5b63 2066 6f72 2063 2069 6e20  ple([c for c in 
+0000de30: 6c69 7374 2870 726f 6669 6c65 2e5f 7261  list(profile._ra
+0000de40: 6e6b 696e 6773 5b30 5d29 2069 6620 6320  nkings[0]) if c 
+0000de50: 696e 2063 616e 6469 6461 7465 735d 290a  in candidates]).
+0000de60: 2020 2020 0a20 2020 2072 6574 7572 6e20      .    return 
+0000de70: 7269 7665 725f 7462 2870 726f 6669 6c65  river_tb(profile
+0000de80: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
+0000de90: 7572 725f 6361 6e64 732c 2074 6965 5f62  urr_cands, tie_b
+0000dea0: 7265 616b 6572 203d 2074 625f 7261 6e6b  reaker = tb_rank
+0000deb0: 696e 672c 2073 7472 656e 6774 685f 6675  ing, strength_fu
+0000dec0: 6e63 7469 6f6e 203d 2073 7472 656e 6774  nction = strengt
+0000ded0: 685f 6675 6e63 7469 6f6e 290a 2020 2020  h_function).    
+0000dee0: 0a0a 2320 5369 6d70 6c65 2053 7461 626c  ..# Simple Stabl
+0000def0: 6520 566f 7469 6e67 200a 6465 6620 5f73  e Voting .def _s
+0000df00: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
+0000df10: 696e 6728 6375 7272 5f63 616e 6473 2c20  ing(curr_cands, 
+0000df20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000df30: 2020 2020 2020 2020 2020 2073 6f72 7465             sorte
+0000df40: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
+0000df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df60: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000df70: 6572 7329 3a0a 2020 2020 2727 270a 2020  ers):.    '''.  
+0000df80: 2020 4465 7465 726d 696e 6520 7468 6520    Determine the 
+0000df90: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000dfa0: 7469 6e67 2077 696e 6e65 7273 2077 6869  ting winners whi
+0000dfb0: 6c65 206b 6565 7069 6e67 2074 7261 636b  le keeping track
+0000dfc0: 200a 2020 2020 6f66 2074 6865 2077 696e   .    of the win
+0000dfd0: 6e65 7273 2069 6e20 616e 7920 7375 6270  ners in any subp
+0000dfe0: 726f 6669 6c65 7320 6368 6563 6b65 6420  rofiles checked 
+0000dff0: 6475 7269 6e67 2063 6f6d 7075 7461 7469  during computati
+0000e000: 6f6e 2e20 0a20 2020 2027 2727 0a20 2020  on. .    '''.   
+0000e010: 200a 2020 2020 7376 5f77 696e 6e65 7273   .    sv_winners
+0000e020: 203d 206c 6973 7428 290a 2020 2020 2020   = list().      
+0000e030: 2020 0a20 2020 2069 6620 6c65 6e28 6375    .    if len(cu
+0000e040: 7272 5f63 616e 6473 2920 3d3d 2031 3a20  rr_cands) == 1: 
+0000e050: 0a20 2020 2020 2020 206d 656d 5f73 765f  .        mem_sv_
+0000e060: 7769 6e6e 6572 735b 7475 706c 6528 6375  winners[tuple(cu
+0000e070: 7272 5f63 616e 6473 295d 203d 2063 7572  rr_cands)] = cur
+0000e080: 725f 6361 6e64 730a 2020 2020 2020 2020  r_cands.        
+0000e090: 7265 7475 726e 2063 7572 725f 6361 6e64  return curr_cand
+0000e0a0: 732c 206d 656d 5f73 765f 7769 6e6e 6572  s, mem_sv_winner
+0000e0b0: 730a 2020 2020 0a20 2020 206d 6172 6769  s.    .    margi
+0000e0c0: 6e5f 7769 746e 6573 7369 6e67 5f77 696e  n_witnessing_win
+0000e0d0: 203d 202d 6d61 7468 2e69 6e66 0a0a 2020   = -math.inf..  
+0000e0e0: 2020 666f 7220 612c 2062 2c20 7320 696e    for a, b, s in
+0000e0f0: 2073 6f72 7465 645f 6d61 7463 6865 733a   sorted_matches:
+0000e100: 0a20 2020 2020 2020 2069 6620 7320 3c20  .        if s < 
+0000e110: 6d61 7267 696e 5f77 6974 6e65 7373 696e  margin_witnessin
+0000e120: 675f 7769 6e3a 200a 2020 2020 2020 2020  g_win: .        
+0000e130: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+0000e140: 2020 6966 2061 206e 6f74 2069 6e20 7376    if a not in sv
+0000e150: 5f77 696e 6e65 7273 3a20 0a20 2020 2020  _winners: .     
+0000e160: 2020 2020 2020 2063 616e 6473 5f6d 696e         cands_min
+0000e170: 7573 5f62 203d 205b 6320 666f 7220 6320  us_b = [c for c 
+0000e180: 696e 2063 7572 725f 6361 6e64 7320 6966  in curr_cands if
+0000e190: 2063 2021 3d20 625d 0a20 2020 2020 2020   c != b].       
+0000e1a0: 2020 2020 2063 616e 6473 5f6d 696e 7573       cands_minus
+0000e1b0: 5f62 5f6b 6579 203d 2074 7570 6c65 2873  _b_key = tuple(s
+0000e1c0: 6f72 7465 6428 6361 6e64 735f 6d69 6e75  orted(cands_minu
+0000e1d0: 735f 6229 290a 2020 2020 2020 2020 2020  s_b)).          
+0000e1e0: 2020 6966 2063 616e 6473 5f6d 696e 7573    if cands_minus
+0000e1f0: 5f62 5f6b 6579 206e 6f74 2069 6e20 6d65  _b_key not in me
+0000e200: 6d5f 7376 5f77 696e 6e65 7273 2e6b 6579  m_sv_winners.key
+0000e210: 7328 293a 200a 2020 2020 2020 2020 2020  s(): .          
+0000e220: 2020 2020 2020 7773 2c20 6d65 6d5f 7376        ws, mem_sv
+0000e230: 5f77 696e 6e65 7273 203d 205f 7369 6d70  _winners = _simp
+0000e240: 6c65 5f73 7461 626c 655f 766f 7469 6e67  le_stable_voting
+0000e250: 2863 7572 725f 6361 6e64 7320 3d20 6361  (curr_cands = ca
+0000e260: 6e64 735f 6d69 6e75 735f 622c 0a20 2020  nds_minus_b,.   
+0000e270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e2a0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
+0000e2b0: 6174 6368 6573 203d 205b 2861 2c20 632c  atches = [(a, c,
+0000e2c0: 2073 2920 666f 7220 612c 2063 2c20 7320   s) for a, c, s 
+0000e2d0: 696e 2073 6f72 7465 645f 6d61 7463 6865  in sorted_matche
+0000e2e0: 7320 6966 2061 2021 3d20 6220 616e 6420  s if a != b and 
+0000e2f0: 6320 213d 2062 5d2c 0a20 2020 2020 2020  c != b],.       
+0000e300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e330: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
+0000e340: 7273 203d 206d 656d 5f73 765f 7769 6e6e  rs = mem_sv_winn
+0000e350: 6572 7329 0a20 2020 2020 2020 2020 2020  ers).           
+0000e360: 2020 2020 206d 656d 5f73 765f 7769 6e6e       mem_sv_winn
+0000e370: 6572 735b 6361 6e64 735f 6d69 6e75 735f  ers[cands_minus_
+0000e380: 625f 6b65 795d 203d 2077 730a 2020 2020  b_key] = ws.    
+0000e390: 2020 2020 2020 2020 656c 7365 3a20 0a20          else: . 
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000e3b0: 7320 3d20 6d65 6d5f 7376 5f77 696e 6e65  s = mem_sv_winne
+0000e3c0: 7273 5b63 616e 6473 5f6d 696e 7573 5f62  rs[cands_minus_b
+0000e3d0: 5f6b 6579 5d0a 2020 2020 2020 2020 2020  _key].          
+0000e3e0: 2020 6966 2061 2069 6e20 7773 3a0a 2020    if a in ws:.  
+0000e3f0: 2020 2020 2020 2020 2020 2020 2020 7376                sv
+0000e400: 5f77 696e 6e65 7273 2e61 7070 656e 6428  _winners.append(
+0000e410: 6129 0a20 2020 2020 2020 2020 2020 2020  a).             
+0000e420: 2020 206d 6172 6769 6e5f 7769 746e 6573     margin_witnes
+0000e430: 7369 6e67 5f77 696e 203d 2073 0a0a 2020  sing_win = s..  
+0000e440: 2020 7265 7475 726e 2073 765f 7769 6e6e    return sv_winn
+0000e450: 6572 732c 206d 656d 5f73 765f 7769 6e6e  ers, mem_sv_winn
+0000e460: 6572 730a 2020 2020 0a0a 4076 6d28 6e61  ers.    ..@vm(na
+0000e470: 6d65 203d 2022 5369 6d70 6c65 2053 7461  me = "Simple Sta
+0000e480: 626c 6520 566f 7469 6e67 2229 0a64 6566  ble Voting").def
+0000e490: 205f 7369 6d70 6c65 5f73 7461 626c 655f   _simple_stable_
+0000e4a0: 766f 7469 6e67 5f77 6974 685f 636f 6e64  voting_with_cond
+0000e4b0: 6f72 6365 745f 6368 6563 6b28 0a20 2020  orcet_check(.   
+0000e4c0: 2065 6461 7461 2c20 0a20 2020 2063 7572   edata, .    cur
+0000e4d0: 725f 6361 6e64 7320 3d20 4e6f 6e65 2c20  r_cands = None, 
+0000e4e0: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+0000e4f0: 6e63 7469 6f6e 203d 204e 6f6e 6529 3a20  nction = None): 
+0000e500: 0a20 2020 2022 2222 5369 6d70 6c65 2053  .    """Simple S
+0000e510: 7461 626c 6520 566f 7469 6e67 2069 7320  table Voting is 
+0000e520: 436f 6e64 6f72 6365 7420 636f 6e73 6973  Condorcet consis
+0000e530: 7465 6e74 2e20 2020 4974 2069 7320 6661  tent.   It is fa
+0000e540: 7374 6572 2074 6f20 736b 6970 2065 7865  ster to skip exe
+0000e550: 6375 7469 6e67 2074 6865 2072 6563 7572  cuting the recur
+0000e560: 7369 7665 2061 6c67 6f72 6974 686d 2077  sive algorithm w
+0000e570: 6865 6e20 7468 6572 6520 6973 2061 2043  hen there is a C
+0000e580: 6f6e 646f 7263 6574 2077 696e 6e65 7246  ondorcet winnerF
+0000e590: 6972 7374 2063 6865 636b 2069 6620 7468  irst check if th
+0000e5a0: 6572 6520 6973 2061 2043 6f6e 646f 7263  ere is a Condorc
+0000e5b0: 6574 2077 696e 6e65 722e 2020 4966 2073  et winner.  If s
+0000e5c0: 6f2c 2072 6574 7572 6e20 7468 6520 436f  o, return the Co
+0000e5d0: 6e64 6f72 6365 7420 7769 6e6e 6572 2c20  ndorcet winner, 
+0000e5e0: 6f74 6865 7277 6973 6520 6669 6e64 2074  otherwise find t
+0000e5f0: 6865 2053 696d 706c 6520 5374 6162 6c65  he Simple Stable
+0000e600: 2056 6f74 696e 6720 7769 6e6e 6572 2075   Voting winner u
+0000e610: 7369 6e67 205f 7369 6d70 6c65 5f73 7461  sing _simple_sta
+0000e620: 626c 655f 766f 7469 6e67 0a0a 2020 2020  ble_voting..    
+0000e630: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
+0000e640: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
+0000e650: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
+0000e660: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
+0000e670: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
+0000e680: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
+0000e690: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
+0000e6a0: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
+0000e6b0: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
+0000e6c0: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
+0000e6d0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
+0000e6e0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
+0000e6f0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
+0000e700: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
+0000e710: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
+0000e720: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
+0000e730: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
+0000e740: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
+0000e750: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
+0000e760: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
+0000e770: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
+0000e780: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
+0000e790: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
+0000e7a0: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
+0000e7b0: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
+0000e7c0: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
+0000e7d0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
+0000e7e0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
+0000e7f0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
+0000e800: 6465 7273 2e20 0a0a 2020 2020 5265 7475  ders. ..    Retu
+0000e810: 726e 733a 200a 2020 2020 2020 2020 4120  rns: .        A 
+0000e820: 736f 7274 6564 206c 6973 7420 6f66 2063  sorted list of c
+0000e830: 616e 6469 6461 7465 732e 200a 0a20 2020  andidates. ..   
+0000e840: 2022 2222 0a20 2020 200a 2020 2020 6377   """.    .    cw
+0000e850: 203d 2065 6461 7461 2e63 6f6e 646f 7263   = edata.condorc
+0000e860: 6574 5f77 696e 6e65 7228 6375 7272 5f63  et_winner(curr_c
+0000e870: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+0000e880: 7329 0a20 2020 2069 6620 6377 2069 7320  s).    if cw is 
+0000e890: 6e6f 7420 4e6f 6e65 3a20 0a20 2020 2020  not None: .     
+0000e8a0: 2020 2072 6574 7572 6e20 5b63 775d 0a20     return [cw]. 
+0000e8b0: 2020 2065 6c73 653a 200a 2020 2020 2020     else: .      
+0000e8c0: 2020 6375 7272 5f63 616e 6473 203d 2065    curr_cands = e
+0000e8d0: 6461 7461 2e63 616e 6469 6461 7465 7320  data.candidates 
+0000e8e0: 6966 2063 7572 725f 6361 6e64 7320 6973  if curr_cands is
+0000e8f0: 204e 6f6e 6520 656c 7365 2063 7572 725f   None else curr_
+0000e900: 6361 6e64 730a 2020 2020 2020 2020 7374  cands.        st
+0000e910: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
+0000e920: 3d20 6564 6174 612e 6d61 7267 696e 2069  = edata.margin i
+0000e930: 6620 7374 7265 6e67 7468 5f66 756e 6374  f strength_funct
+0000e940: 696f 6e20 6973 204e 6f6e 6520 656c 7365  ion is None else
+0000e950: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000e960: 6f6e 2020 0a0a 2020 2020 2020 2020 6d61  on  ..        ma
+0000e970: 7463 6865 7320 3d20 5b28 612c 2062 2c20  tches = [(a, b, 
+0000e980: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+0000e990: 6e28 612c 2062 2929 2066 6f72 2061 2069  n(a, b)) for a i
+0000e9a0: 6e20 6375 7272 5f63 616e 6473 2066 6f72  n curr_cands for
+0000e9b0: 2062 2069 6e20 6375 7272 5f63 616e 6473   b in curr_cands
+0000e9c0: 2069 6620 6120 213d 2062 5d0a 2020 2020   if a != b].    
+0000e9d0: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
+0000e9e0: 6573 203d 2073 6f72 7465 6428 6d61 7463  es = sorted(matc
+0000e9f0: 6865 732c 2072 6576 6572 7365 3d54 7275  hes, reverse=Tru
+0000ea00: 652c 206b 6579 3d6c 616d 6264 6120 6d5f  e, key=lambda m_
+0000ea10: 775f 7765 6967 6874 3a20 6d5f 775f 7765  w_weight: m_w_we
+0000ea20: 6967 6874 5b32 5d29 0a20 2020 200a 2020  ight[2]).    .  
+0000ea30: 2020 2020 2020 7265 7475 726e 2073 6f72        return sor
+0000ea40: 7465 6428 5f73 696d 706c 655f 7374 6162  ted(_simple_stab
+0000ea50: 6c65 5f76 6f74 696e 6728 6375 7272 5f63  le_voting(curr_c
+0000ea60: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+0000ea70: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
+0000ea80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eaa0: 736f 7274 6564 5f6d 6174 6368 6573 203d  sorted_matches =
+0000eab0: 2073 6f72 7465 645f 6d61 7463 6865 732c   sorted_matches,
+0000eac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eae0: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000eaf0: 5f73 765f 7769 6e6e 6572 7320 3d20 7b7d  _sv_winners = {}
+0000eb00: 295b 305d 290a 0a0a 6465 6620 5f73 696d  )[0])...def _sim
+0000eb10: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000eb20: 675f 6261 7369 6328 6564 6174 612c 2063  g_basic(edata, c
+0000eb30: 7572 725f 6361 6e64 7320 3d20 4e6f 6e65  urr_cands = None
+0000eb40: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
+0000eb50: 696f 6e20 3d20 4e6f 6e65 293a 200a 2020  ion = None): .  
+0000eb60: 2020 2222 2249 6d70 6c65 6d65 6e74 6174    """Implementat
+0000eb70: 696f 6e20 6f66 2053 696d 706c 6520 5374  ion of Simple St
+0000eb80: 6162 6c65 2056 6f74 696e 6720 6672 6f6d  able Voting from
+0000eb90: 2068 7474 7073 3a2f 2f61 7278 6976 2e6f   https://arxiv.o
+0000eba0: 7267 2f61 6273 2f32 3130 382e 3030 3534  rg/abs/2108.0054
+0000ebb0: 322e 200a 0a20 2020 2041 7267 733a 0a20  2. ..    Args:. 
+0000ebc0: 2020 2020 2020 2065 6461 7461 2028 5072         edata (Pr
+0000ebd0: 6f66 696c 652c 2050 726f 6669 6c65 5769  ofile, ProfileWi
+0000ebe0: 7468 5469 6573 2c20 4d61 7267 696e 4772  thTies, MarginGr
+0000ebf0: 6170 6829 3a20 416e 7920 656c 6563 7469  aph): Any electi
+0000ec00: 6f6e 2064 6174 6120 7468 6174 2068 6173  on data that has
+0000ec10: 2061 2060 6d61 7267 696e 6020 6d65 7468   a `margin` meth
+0000ec20: 6f64 2e20 0a20 2020 2020 2020 2063 7572  od. .        cur
+0000ec30: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+0000ec40: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+0000ec50: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+0000ec60: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+0000ec70: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+0000ec80: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+0000ec90: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+0000eca0: 7572 725f 6361 6e64 7360 600a 2020 2020  urr_cands``.    
+0000ecb0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000ecc0: 6374 696f 6e20 2866 756e 6374 696f 6e2c  ction (function,
+0000ecd0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+0000ece0: 7374 7265 6e67 7468 2066 756e 6374 696f  strength functio
+0000ecf0: 6e20 746f 2062 6520 7573 6564 2074 6f20  n to be used to 
+0000ed00: 6361 6c63 756c 6174 6520 7468 6520 7374  calculate the st
+0000ed10: 7265 6e67 7468 206f 6620 6120 7061 7468  rength of a path
+0000ed20: 2e20 2020 5468 6520 6465 6661 756c 7420  .   The default 
+0000ed30: 6973 2074 6865 206d 6172 6769 6e20 6d65  is the margin me
+0000ed40: 7468 6f64 206f 6620 6060 6564 6174 6160  thod of ``edata`
+0000ed50: 602e 2020 2054 6869 7320 6f6e 6c79 206d  `.   This only m
+0000ed60: 6174 7465 7273 2077 6865 6e20 7468 6520  atters when the 
+0000ed70: 6261 6c6c 6f74 7320 6172 6520 6e6f 7420  ballots are not 
+0000ed80: 6c69 6e65 6172 206f 7264 6572 732e 200a  linear orders. .
+0000ed90: 0a20 2020 2052 6574 7572 6e73 3a20 0a20  .    Returns: . 
+0000eda0: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+0000edb0: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+0000edc0: 6573 2e20 0a0a 2020 2020 2222 220a 2020  es. ..    """.  
+0000edd0: 2020 0a20 2020 2063 7572 725f 6361 6e64    .    curr_cand
+0000ede0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
+0000edf0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
+0000ee00: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
+0000ee10: 6375 7272 5f63 616e 6473 0a20 2020 2073  curr_cands.    s
 0000ee20: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
-0000ee30: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
-0000ee40: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
-0000ee50: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
-0000ee60: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
-0000ee70: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
-0000ee80: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
-0000ee90: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
-0000eea0: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
-0000eeb0: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
-0000eec0: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
-0000eed0: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
-0000eee0: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
-0000eef0: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
-0000ef00: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
-0000ef10: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-0000ef20: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
-0000ef30: 0a20 2020 2022 2222 0a20 2020 200a 2020  .    """.    .  
-0000ef40: 2020 6377 203d 2065 6461 7461 2e63 6f6e    cw = edata.con
-0000ef50: 646f 7263 6574 5f77 696e 6e65 7228 6375  dorcet_winner(cu
-0000ef60: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
-0000ef70: 6361 6e64 7329 0a20 2020 2069 6620 6377  cands).    if cw
-0000ef80: 2069 7320 6e6f 7420 4e6f 6e65 3a20 0a20   is not None: . 
-0000ef90: 2020 2020 2020 2072 6574 7572 6e20 5b63         return [c
-0000efa0: 775d 0a20 2020 2065 6c73 653a 200a 2020  w].    else: .  
-0000efb0: 2020 2020 2020 6375 7272 5f63 616e 6473        curr_cands
-0000efc0: 203d 2065 6461 7461 2e63 616e 6469 6461   = edata.candida
-0000efd0: 7465 7320 6966 2063 7572 725f 6361 6e64  tes if curr_cand
-0000efe0: 7320 6973 204e 6f6e 6520 656c 7365 2063  s is None else c
-0000eff0: 7572 725f 6361 6e64 730a 2020 2020 2020  urr_cands.      
-0000f000: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-0000f010: 696f 6e20 3d20 6564 6174 612e 6d61 7267  ion = edata.marg
-0000f020: 696e 2069 6620 7374 7265 6e67 7468 5f66  in if strength_f
-0000f030: 756e 6374 696f 6e20 6973 204e 6f6e 6520  unction is None 
-0000f040: 656c 7365 2073 7472 656e 6774 685f 6675  else strength_fu
-0000f050: 6e63 7469 6f6e 2020 0a0a 2020 2020 2020  nction  ..      
-0000f060: 2020 6d61 7463 6865 7320 3d20 5b28 612c    matches = [(a,
-0000f070: 2062 2c20 7374 7265 6e67 7468 5f66 756e   b, strength_fun
-0000f080: 6374 696f 6e28 612c 2062 2929 2066 6f72  ction(a, b)) for
-0000f090: 2061 2069 6e20 6375 7272 5f63 616e 6473   a in curr_cands
-0000f0a0: 2066 6f72 2062 2069 6e20 6375 7272 5f63   for b in curr_c
-0000f0b0: 616e 6473 2069 6620 6120 213d 2062 5d0a  ands if a != b].
-0000f0c0: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
-0000f0d0: 6174 6368 6573 203d 2073 6f72 7465 6428  atches = sorted(
-0000f0e0: 6d61 7463 6865 732c 2072 6576 6572 7365  matches, reverse
-0000f0f0: 3d54 7275 652c 206b 6579 3d6c 616d 6264  =True, key=lambd
-0000f100: 6120 6d5f 775f 7765 6967 6874 3a20 6d5f  a m_w_weight: m_
-0000f110: 775f 7765 6967 6874 5b32 5d29 0a20 2020  w_weight[2]).   
-0000f120: 200a 2020 2020 2020 2020 7265 7475 726e   .        return
-0000f130: 2073 6f72 7465 6428 5f73 696d 706c 655f   sorted(_simple_
-0000f140: 7374 6162 6c65 5f76 6f74 696e 6728 6375  stable_voting(cu
-0000f150: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
-0000f160: 6361 6e64 732c 200a 2020 2020 2020 2020  cands, .        
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f190: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
-0000f1a0: 6573 203d 2073 6f72 7465 645f 6d61 7463  es = sorted_matc
-0000f1b0: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
-0000f1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f1e0: 206d 656d 5f73 765f 7769 6e6e 6572 7320   mem_sv_winners 
-0000f1f0: 3d20 7b7d 295b 305d 290a 0a0a 6465 6620  = {})[0])...def 
-0000f200: 5f73 696d 706c 655f 7374 6162 6c65 5f76  _simple_stable_v
-0000f210: 6f74 696e 675f 6261 7369 6328 6564 6174  oting_basic(edat
-0000f220: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-0000f230: 4e6f 6e65 2c20 7374 7265 6e67 7468 5f66  None, strength_f
-0000f240: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-0000f250: 200a 2020 2020 2222 2249 6d70 6c65 6d65   .    """Impleme
-0000f260: 6e74 6174 696f 6e20 6f66 2053 696d 706c  ntation of Simpl
-0000f270: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
-0000f280: 6672 6f6d 2068 7474 7073 3a2f 2f61 7278  from https://arx
-0000f290: 6976 2e6f 7267 2f61 6273 2f32 3130 382e  iv.org/abs/2108.
-0000f2a0: 3030 3534 322e 200a 0a20 2020 2041 7267  00542. ..    Arg
-0000f2b0: 733a 0a20 2020 2020 2020 2065 6461 7461  s:.        edata
-0000f2c0: 2028 5072 6f66 696c 652c 2050 726f 6669   (Profile, Profi
-0000f2d0: 6c65 5769 7468 5469 6573 2c20 4d61 7267  leWithTies, Marg
-0000f2e0: 696e 4772 6170 6829 3a20 416e 7920 656c  inGraph): Any el
-0000f2f0: 6563 7469 6f6e 2064 6174 6120 7468 6174  ection data that
-0000f300: 2068 6173 2061 2060 6d61 7267 696e 6020   has a `margin` 
-0000f310: 6d65 7468 6f64 2e20 0a20 2020 2020 2020  method. .       
-0000f320: 2063 7572 725f 6361 6e64 7320 284c 6973   curr_cands (Lis
-0000f330: 745b 696e 745d 2c20 6f70 7469 6f6e 616c  t[int], optional
-0000f340: 293a 2049 6620 7365 742c 2074 6865 6e20  ): If set, then 
-0000f350: 6669 6e64 2074 6865 2077 696e 6e65 7273  find the winners
-0000f360: 2066 6f72 2074 6865 2070 726f 6669 6c65   for the profile
-0000f370: 2072 6573 7472 6963 7465 6420 746f 2074   restricted to t
-0000f380: 6865 2063 616e 6469 6461 7465 7320 696e  he candidates in
-0000f390: 2060 6063 7572 725f 6361 6e64 7360 600a   ``curr_cands``.
-0000f3a0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
-0000f3b0: 5f66 756e 6374 696f 6e20 2866 756e 6374  _function (funct
-0000f3c0: 696f 6e2c 206f 7074 696f 6e61 6c29 3a20  ion, optional): 
-0000f3d0: 5468 6520 7374 7265 6e67 7468 2066 756e  The strength fun
-0000f3e0: 6374 696f 6e20 746f 2062 6520 7573 6564  ction to be used
-0000f3f0: 2074 6f20 6361 6c63 756c 6174 6520 7468   to calculate th
-0000f400: 6520 7374 7265 6e67 7468 206f 6620 6120  e strength of a 
-0000f410: 7061 7468 2e20 2020 5468 6520 6465 6661  path.   The defa
-0000f420: 756c 7420 6973 2074 6865 206d 6172 6769  ult is the margi
-0000f430: 6e20 6d65 7468 6f64 206f 6620 6060 6564  n method of ``ed
-0000f440: 6174 6160 602e 2020 2054 6869 7320 6f6e  ata``.   This on
-0000f450: 6c79 206d 6174 7465 7273 2077 6865 6e20  ly matters when 
-0000f460: 7468 6520 6261 6c6c 6f74 7320 6172 6520  the ballots are 
-0000f470: 6e6f 7420 6c69 6e65 6172 206f 7264 6572  not linear order
-0000f480: 732e 200a 0a20 2020 2052 6574 7572 6e73  s. ..    Returns
-0000f490: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-0000f4a0: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-0000f4b0: 6964 6174 6573 2e20 0a0a 2020 2020 2222  idates. ..    ""
-0000f4c0: 220a 2020 2020 0a20 2020 2063 7572 725f  ".    .    curr_
-0000f4d0: 6361 6e64 7320 3d20 6564 6174 612e 6361  cands = edata.ca
-0000f4e0: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
-0000f4f0: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
-0000f500: 6c73 6520 6375 7272 5f63 616e 6473 0a20  lse curr_cands. 
-0000f510: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-0000f520: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-0000f530: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-0000f540: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-0000f550: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-0000f560: 756e 6374 696f 6e20 200a 0a20 2020 206d  unction  ..    m
-0000f570: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
-0000f580: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-0000f590: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
-0000f5a0: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
-0000f5b0: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
-0000f5c0: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
-0000f5d0: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
-0000f5e0: 3d20 736f 7274 6564 286d 6174 6368 6573  = sorted(matches
-0000f5f0: 2c20 7265 7665 7273 653d 5472 7565 2c20  , reverse=True, 
-0000f600: 6b65 793d 6c61 6d62 6461 206d 5f77 5f77  key=lambda m_w_w
-0000f610: 6569 6768 743a 206d 5f77 5f77 6569 6768  eight: m_w_weigh
-0000f620: 745b 325d 290a 2020 2020 0a20 2020 2072  t[2]).    .    r
-0000f630: 6574 7572 6e20 736f 7274 6564 285f 7369  eturn sorted(_si
-0000f640: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
-0000f650: 6e67 2863 7572 725f 6361 6e64 7320 3d20  ng(curr_cands = 
-0000f660: 6375 7272 5f63 616e 6473 2c20 0a20 2020  curr_cands, .   
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f690: 2020 2020 2073 6f72 7465 645f 6d61 7463       sorted_matc
-0000f6a0: 6865 7320 3d20 736f 7274 6564 5f6d 6174  hes = sorted_mat
-0000f6b0: 6368 6573 2c0a 2020 2020 2020 2020 2020  ches,.          
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0000f6e0: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
-0000f6f0: 7d29 5b30 5d29 0a0a 7373 765f 7072 6f70  })[0])..ssv_prop
-0000f700: 6572 7469 6573 203d 2056 6f74 696e 674d  erties = VotingM
-0000f710: 6574 686f 6450 726f 7065 7274 6965 7328  ethodProperties(
-0000f720: 0a20 2020 2063 6f6e 646f 7263 6574 5f77  .    condorcet_w
-0000f730: 696e 6e65 723d 5472 7565 2c20 0a20 2020  inner=True, .   
-0000f740: 2063 6f6e 646f 7263 6574 5f6c 6f73 6572   condorcet_loser
-0000f750: 3d54 7275 652c 0a20 2020 2070 6172 6574  =True,.    paret
-0000f760: 6f5f 646f 6d69 6e61 6e63 653d 5472 7565  o_dominance=True
-0000f770: 2c0a 2020 2020 706f 7369 7469 7665 5f69  ,.    positive_i
-0000f780: 6e76 6f6c 7665 6d65 6e74 3d46 616c 7365  nvolvement=False
-0000f790: 2c20 0a20 2020 2029 0a40 766d 286e 616d  , .    ).@vm(nam
-0000f7a0: 6520 3d20 2253 696d 706c 6520 5374 6162  e = "Simple Stab
-0000f7b0: 6c65 2056 6f74 696e 6722 2c0a 2020 2020  le Voting",.    
-0000f7c0: 7072 6f70 6572 7469 6573 203d 2073 7376  properties = ssv
-0000f7d0: 5f70 726f 7065 7274 6965 732c 0a20 2020  _properties,.   
-0000f7e0: 2069 6e70 7574 5f74 7970 6573 203d 205b   input_types = [
-0000f7f0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-0000f800: 4f46 494c 452c 2045 6c65 6374 696f 6e54  OFILE, ElectionT
-0000f810: 7970 6573 2e50 524f 4649 4c45 5f57 4954  ypes.PROFILE_WIT
-0000f820: 485f 5449 4553 2c20 456c 6563 7469 6f6e  H_TIES, Election
-0000f830: 5479 7065 732e 4d41 5247 494e 5f47 5241  Types.MARGIN_GRA
-0000f840: 5048 5d29 0a64 6566 2073 696d 706c 655f  PH]).def simple_
-0000f850: 7374 6162 6c65 5f76 6f74 696e 6728 0a20  stable_voting(. 
-0000f860: 2020 2065 6461 7461 2c20 0a20 2020 2063     edata, .    c
-0000f870: 7572 725f 6361 6e64 733d 4e6f 6e65 2c20  urr_cands=None, 
-0000f880: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
-0000f890: 6e63 7469 6f6e 3d4e 6f6e 652c 0a20 2020  nction=None,.   
-0000f8a0: 2061 6c67 6f72 6974 686d 203d 2027 6261   algorithm = 'ba
-0000f8b0: 7369 6327 293a 200a 0a20 2020 2022 2222  sic'): ..    """
-0000f8c0: 496d 706c 656d 656e 7461 7469 6f6e 206f  Implementation o
-0000f8d0: 6620 5369 6d70 6c65 2053 7461 626c 6520  f Simple Stable 
-0000f8e0: 566f 7469 6e67 2066 726f 6d20 6874 7470  Voting from http
-0000f8f0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-0000f900: 732f 3231 3038 2e30 3035 3432 2e20 0a0a  s/2108.00542. ..
-0000f910: 2020 2020 5369 6d70 6c65 2053 7461 626c      Simple Stabl
-0000f920: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
-0000f930: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
-0000f940: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
-0000f950: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
-0000f960: 312e 2049 6620 7468 6572 6520 6973 206f  1. If there is o
-0000f970: 6e6c 7920 6f6e 6520 6361 6e64 6964 6174  nly one candidat
-0000f980: 6520 696e 2074 6865 2070 726f 6669 6c65  e in the profile
-0000f990: 2c20 7468 656e 2074 6861 7420 6361 6e64  , then that cand
-0000f9a0: 6964 6174 6520 6973 2074 6865 2077 696e  idate is the win
-0000f9b0: 6e65 722e 200a 2020 2020 322e 204f 7264  ner. .    2. Ord
-0000f9c0: 6572 2074 6865 2070 6169 7273 203a 6d61  er the pairs :ma
-0000f9d0: 7468 3a60 2861 2c62 2960 206f 6620 6361  th:`(a,b)` of ca
-0000f9e0: 6e64 6964 6174 6573 2066 726f 6d20 6c61  ndidates from la
-0000f9f0: 7267 6573 7420 746f 2073 6d61 6c6c 6573  rgest to smalles
-0000fa00: 7420 7661 6c75 6520 6f66 2074 6865 206d  t value of the m
-0000fa10: 6172 6769 6e20 6f66 203a 6d61 7468 3a60  argin of :math:`
-0000fa20: 6160 206f 7665 7220 3a6d 6174 683a 6062  a` over :math:`b
-0000fa30: 602c 2061 6e64 2064 6563 6c61 7265 2061  `, and declare a
-0000fa40: 7320 5369 6d70 6c65 2053 7461 626c 6520  s Simple Stable 
-0000fa50: 566f 7469 6e67 2077 696e 6e65 7273 2074  Voting winners t
-0000fa60: 6865 2063 616e 6469 6461 7465 2873 2920  he candidate(s) 
-0000fa70: 3a6d 6174 683a 6061 6020 6672 6f6d 2074  :math:`a` from t
-0000fa80: 6865 2065 6172 6c69 6573 7420 7061 6972  he earliest pair
-0000fa90: 2873 2920 3a6d 6174 683a 6028 612c 6229  (s) :math:`(a,b)
-0000faa0: 6020 7375 6368 2074 6861 7420 3a6d 6174  ` such that :mat
-0000fab0: 683a 6061 6020 6973 2061 2053 696d 706c  h:`a` is a Simpl
-0000fac0: 6520 5374 6162 6c65 2056 6f74 696e 6720  e Stable Voting 
-0000fad0: 7769 6e6e 6572 2069 6e20 7468 6520 656c  winner in the el
-0000fae0: 6563 7469 6f6e 2077 6974 686f 7574 203a  ection without :
-0000faf0: 6d61 7468 3a60 6260 2e20 0a0a 2020 2020  math:`b`. ..    
-0000fb00: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-0000fb10: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-0000fb20: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-0000fb30: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-0000fb40: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-0000fb50: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-0000fb60: 6e60 206d 6574 686f 642e 200a 2020 2020  n` method. .    
-0000fb70: 2020 2020 6375 7272 5f63 616e 6473 2028      curr_cands (
-0000fb80: 4c69 7374 5b69 6e74 5d2c 206f 7074 696f  List[int], optio
-0000fb90: 6e61 6c29 3a20 4966 2073 6574 2c20 7468  nal): If set, th
-0000fba0: 656e 2066 696e 6420 7468 6520 7769 6e6e  en find the winn
-0000fbb0: 6572 7320 666f 7220 7468 6520 7072 6f66  ers for the prof
-0000fbc0: 696c 6520 7265 7374 7269 6374 6564 2074  ile restricted t
-0000fbd0: 6f20 7468 6520 6361 6e64 6964 6174 6573  o the candidates
-0000fbe0: 2069 6e20 6060 6375 7272 5f63 616e 6473   in ``curr_cands
-0000fbf0: 6060 0a20 2020 2020 2020 2073 7472 656e  ``.        stren
-0000fc00: 6774 685f 6675 6e63 7469 6f6e 2028 6675  gth_function (fu
-0000fc10: 6e63 7469 6f6e 2c20 6f70 7469 6f6e 616c  nction, optional
-0000fc20: 293a 2054 6865 2073 7472 656e 6774 6820  ): The strength 
-0000fc30: 6675 6e63 7469 6f6e 2074 6f20 6265 2075  function to be u
-0000fc40: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-0000fc50: 2074 6865 2073 7472 656e 6774 6820 6f66   the strength of
-0000fc60: 2061 2070 6174 682e 2020 2054 6865 2064   a path.   The d
-0000fc70: 6566 6175 6c74 2069 7320 7468 6520 6d61  efault is the ma
-0000fc80: 7267 696e 206d 6574 686f 6420 6f66 2060  rgin method of `
-0000fc90: 6065 6461 7461 6060 2e20 2020 5468 6973  `edata``.   This
-0000fca0: 206f 6e6c 7920 6d61 7474 6572 7320 7768   only matters wh
-0000fcb0: 656e 2074 6865 2062 616c 6c6f 7473 2061  en the ballots a
-0000fcc0: 7265 206e 6f74 206c 696e 6561 7220 6f72  re not linear or
-0000fcd0: 6465 7273 2e20 0a20 2020 2020 2020 2061  ders. .        a
-0000fce0: 6c67 6f72 6974 686d 2028 7374 722c 206f  lgorithm (str, o
-0000fcf0: 7074 696f 6e61 6c29 3a20 5370 6563 6966  ptional): Specif
-0000fd00: 7920 7768 6963 6820 616c 676f 7269 7468  y which algorith
-0000fd10: 6d20 746f 2075 7365 2e20 204f 7074 696f  m to use.  Optio
-0000fd20: 6e73 2061 7265 2027 6261 7369 6327 2028  ns are 'basic' (
-0000fd30: 7468 6520 6465 6661 756c 7429 2061 6e64  the default) and
-0000fd40: 2027 7769 7468 5f63 6f6e 646f 7263 6574   'with_condorcet
-0000fd50: 5f63 6865 636b 272e 0a0a 2020 2020 5265  _check'...    Re
-0000fd60: 7475 726e 733a 200a 2020 2020 2020 2020  turns: .        
-0000fd70: 4120 736f 7274 6564 206c 6973 7420 6f66  A sorted list of
-0000fd80: 2063 616e 6469 6461 7465 732e 200a 0a20   candidates. .. 
-0000fd90: 2020 202e 2e20 7365 6561 6c73 6f3a 3a0a     .. seealso::.
-0000fda0: 0a20 2020 2020 2020 203a 6d65 7468 3a60  .        :meth:`
-0000fdb0: 7072 6566 5f76 6f74 696e 672e 6d61 7267  pref_voting.marg
-0000fdc0: 696e 5f62 6173 6564 5f6d 6574 686f 6473  in_based_methods
-0000fdd0: 2e73 7461 626c 655f 766f 7469 6e67 600a  .stable_voting`.
-0000fde0: 0a20 2020 203a 4578 616d 706c 653a 200a  .    :Example: .
-0000fdf0: 0a20 2020 202e 2e20 6578 6563 5f63 6f64  .    .. exec_cod
-0000fe00: 653a 3a0a 0a20 2020 2020 2020 2066 726f  e::..        fro
-0000fe10: 6d20 7072 6566 5f76 6f74 696e 672e 7765  m pref_voting.we
-0000fe20: 6967 6874 6564 5f6d 616a 6f72 6974 795f  ighted_majority_
-0000fe30: 6772 6170 6873 2069 6d70 6f72 7420 4d61  graphs import Ma
-0000fe40: 7267 696e 4772 6170 680a 2020 2020 2020  rginGraph.      
-0000fe50: 2020 6672 6f6d 2070 7265 665f 766f 7469    from pref_voti
-0000fe60: 6e67 2e6d 6172 6769 6e5f 6261 7365 645f  ng.margin_based_
-0000fe70: 6d65 7468 6f64 7320 696d 706f 7274 2073  methods import s
-0000fe80: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000fe90: 696e 670a 0a20 2020 2020 2020 206d 6720  ing..        mg 
-0000fea0: 3d20 4d61 7267 696e 4772 6170 6828 5b30  = MarginGraph([0
-0000feb0: 2c20 312c 2032 2c20 335d 2c20 5b28 302c  , 1, 2, 3], [(0,
-0000fec0: 2033 2c20 3829 2c20 2831 2c20 302c 2031   3, 8), (1, 0, 1
-0000fed0: 3029 2c20 2832 2c20 302c 2034 292c 2028  0), (2, 0, 4), (
-0000fee0: 322c 2031 2c20 3829 2c20 2833 2c20 312c  2, 1, 8), (3, 1,
-0000fef0: 2038 295d 290a 0a20 2020 2020 2020 2073   8)])..        s
-0000ff00: 696d 706c 655f 7374 6162 6c65 5f76 6f74  imple_stable_vot
-0000ff10: 696e 672e 6469 7370 6c61 7928 6d67 290a  ing.display(mg).
-0000ff20: 2020 2020 2020 2020 7369 6d70 6c65 5f73          simple_s
-0000ff30: 7461 626c 655f 766f 7469 6e67 2e64 6973  table_voting.dis
-0000ff40: 706c 6179 286d 672c 2061 6c67 6f72 6974  play(mg, algorit
-0000ff50: 686d 3d27 6261 7369 6327 290a 2020 2020  hm='basic').    
-0000ff60: 2020 2020 7369 6d70 6c65 5f73 7461 626c      simple_stabl
-0000ff70: 655f 766f 7469 6e67 2e64 6973 706c 6179  e_voting.display
-0000ff80: 286d 672c 2061 6c67 6f72 6974 686d 3d27  (mg, algorithm='
-0000ff90: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
-0000ffa0: 6865 636b 2729 0a0a 2020 2020 2222 220a  heck')..    """.
-0000ffb0: 2020 2020 0a20 2020 2069 6620 616c 676f      .    if algo
-0000ffc0: 7269 7468 6d20 3d3d 2027 6261 7369 6327  rithm == 'basic'
-0000ffd0: 3a20 0a20 2020 2020 2020 2072 6574 7572  : .        retur
-0000ffe0: 6e20 5f73 696d 706c 655f 7374 6162 6c65  n _simple_stable
-0000fff0: 5f76 6f74 696e 675f 6261 7369 6328 6564  _voting_basic(ed
-00010000: 6174 612c 2063 7572 725f 6361 6e64 7320  ata, curr_cands 
-00010010: 3d20 6375 7272 5f63 616e 6473 2c20 7374  = curr_cands, st
-00010020: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00010030: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
-00010040: 696f 6e29 0a20 2020 2065 6c69 6620 616c  ion).    elif al
-00010050: 676f 7269 7468 6d20 3d3d 2027 7769 7468  gorithm == 'with
-00010060: 5f63 6f6e 646f 7263 6574 5f63 6865 636b  _condorcet_check
-00010070: 273a 0a20 2020 2020 2020 2072 6574 7572  ':.        retur
-00010080: 6e20 5f73 696d 706c 655f 7374 6162 6c65  n _simple_stable
-00010090: 5f76 6f74 696e 675f 7769 7468 5f63 6f6e  _voting_with_con
-000100a0: 646f 7263 6574 5f63 6865 636b 2865 6461  dorcet_check(eda
-000100b0: 7461 2c20 6375 7272 5f63 616e 6473 203d  ta, curr_cands =
-000100c0: 2063 7572 725f 6361 6e64 732c 2073 7472   curr_cands, str
-000100d0: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
-000100e0: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
-000100f0: 6f6e 290a 2020 2020 656c 7365 3a0a 2020  on).    else:.  
-00010100: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00010110: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
-00010120: 616c 676f 7269 7468 6d20 7370 6563 6966  algorithm specif
-00010130: 6965 642e 2229 0a20 2020 200a 0a64 6566  ied.").    ..def
-00010140: 205f 7374 6162 6c65 5f76 6f74 696e 6728   _stable_voting(
-00010150: 6564 6174 612c 200a 2020 2020 2020 2020  edata, .        
-00010160: 2020 2020 2020 2020 2020 2063 7572 725f             curr_
-00010170: 6361 6e64 732c 0a20 2020 2020 2020 2020  cands,.         
-00010180: 2020 2020 2020 2020 2020 7374 7265 6e67            streng
-00010190: 7468 5f66 756e 6374 696f 6e2c 0a20 2020  th_function,.   
-000101a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101b0: 736f 7274 6564 5f6d 6174 6368 6573 2c0a  sorted_matches,.
-000101c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000101d0: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
-000101e0: 7329 3a20 0a20 2020 2027 2727 0a20 2020  s): .    '''.   
-000101f0: 2044 6574 6572 6d69 6e65 2074 6865 2053   Determine the S
-00010200: 7461 626c 6520 566f 7469 6e67 2077 696e  table Voting win
-00010210: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00010220: 6669 6c65 2077 6869 6c65 206b 6565 7069  file while keepi
-00010230: 6e67 2074 7261 636b 206f 6620 7468 6520  ng track of the 
-00010240: 7769 6e6e 6572 7320 696e 2061 6e79 2073  winners in any s
-00010250: 7562 7072 6f66 696c 6573 2063 6865 636b  ubprofiles check
-00010260: 6564 2064 7572 696e 6720 636f 6d70 7574  ed during comput
-00010270: 6174 696f 6e2e 200a 2020 2020 2727 270a  ation. .    '''.
-00010280: 2020 2020 0a20 2020 2073 765f 7769 6e6e      .    sv_winn
-00010290: 6572 7320 3d20 6c69 7374 2829 0a20 2020  ers = list().   
-000102a0: 200a 2020 2020 756e 6465 6665 6174 6564   .    undefeated
-000102b0: 5f63 616e 6469 6461 7465 7320 3d20 7370  _candidates = sp
-000102c0: 6c69 745f 6379 636c 6528 6564 6174 612c  lit_cycle(edata,
-000102d0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-000102e0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-000102f0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-00010300: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-00010310: 0a0a 2020 2020 6966 206c 656e 2863 7572  ..    if len(cur
-00010320: 725f 6361 6e64 7329 203d 3d20 313a 200a  r_cands) == 1: .
-00010330: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
-00010340: 696e 6e65 7273 5b74 7570 6c65 2863 7572  inners[tuple(cur
-00010350: 725f 6361 6e64 7329 5d20 3d20 6375 7272  r_cands)] = curr
-00010360: 5f63 616e 6473 0a20 2020 2020 2020 2072  _cands.        r
-00010370: 6574 7572 6e20 6375 7272 5f63 616e 6473  eturn curr_cands
-00010380: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
-00010390: 0a20 2020 200a 2020 2020 6d61 7267 696e  .    .    margin
-000103a0: 5f77 6974 6e65 7373 696e 675f 7769 6e20  _witnessing_win 
-000103b0: 3d20 2d6d 6174 682e 696e 660a 0a20 2020  = -math.inf..   
-000103c0: 2066 6f72 2061 2c20 622c 2073 2069 6e20   for a, b, s in 
-000103d0: 736f 7274 6564 5f6d 6174 6368 6573 3a0a  sorted_matches:.
-000103e0: 2020 2020 2020 2020 6966 2073 203c 206d          if s < m
-000103f0: 6172 6769 6e5f 7769 746e 6573 7369 6e67  argin_witnessing
-00010400: 5f77 696e 3a20 0a20 2020 2020 2020 2020  _win: .         
-00010410: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00010420: 2069 6620 6120 696e 2075 6e64 6566 6561   if a in undefea
-00010430: 7465 645f 6361 6e64 6964 6174 6573 2061  ted_candidates a
-00010440: 6e64 2061 206e 6f74 2069 6e20 7376 5f77  nd a not in sv_w
-00010450: 696e 6e65 7273 3a20 0a20 2020 2020 2020  inners: .       
-00010460: 2020 2020 2063 616e 6473 5f6d 696e 7573       cands_minus
-00010470: 5f62 203d 205b 6320 666f 7220 6320 696e  _b = [c for c in
-00010480: 2063 7572 725f 6361 6e64 7320 6966 2063   curr_cands if c
-00010490: 2021 3d20 625d 0a20 2020 2020 2020 2020   != b].         
-000104a0: 2020 2063 616e 6473 5f6d 696e 7573 5f62     cands_minus_b
-000104b0: 5f6b 6579 203d 2074 7570 6c65 2873 6f72  _key = tuple(sor
-000104c0: 7465 6428 6361 6e64 735f 6d69 6e75 735f  ted(cands_minus_
-000104d0: 6229 290a 2020 2020 2020 2020 2020 2020  b)).            
-000104e0: 6966 2063 616e 6473 5f6d 696e 7573 5f62  if cands_minus_b
-000104f0: 5f6b 6579 206e 6f74 2069 6e20 6d65 6d5f  _key not in mem_
-00010500: 7376 5f77 696e 6e65 7273 2e6b 6579 7328  sv_winners.keys(
-00010510: 293a 200a 2020 2020 2020 2020 2020 2020  ): .            
-00010520: 2020 2020 7773 2c20 6d65 6d5f 7376 5f77      ws, mem_sv_w
-00010530: 696e 6e65 7273 203d 205f 7374 6162 6c65  inners = _stable
-00010540: 5f76 6f74 696e 6728 6564 6174 612c 0a20  _voting(edata,. 
-00010550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee30: 203d 2065 6461 7461 2e6d 6172 6769 6e20   = edata.margin 
+0000ee40: 6966 2073 7472 656e 6774 685f 6675 6e63  if strength_func
+0000ee50: 7469 6f6e 2069 7320 4e6f 6e65 2065 6c73  tion is None els
+0000ee60: 6520 7374 7265 6e67 7468 5f66 756e 6374  e strength_funct
+0000ee70: 696f 6e20 200a 0a20 2020 206d 6174 6368  ion  ..    match
+0000ee80: 6573 203d 205b 2861 2c20 622c 2073 7472  es = [(a, b, str
+0000ee90: 656e 6774 685f 6675 6e63 7469 6f6e 2861  ength_function(a
+0000eea0: 2c20 6229 2920 666f 7220 6120 696e 2063  , b)) for a in c
+0000eeb0: 7572 725f 6361 6e64 7320 666f 7220 6220  urr_cands for b 
+0000eec0: 696e 2063 7572 725f 6361 6e64 7320 6966  in curr_cands if
+0000eed0: 2061 2021 3d20 625d 0a20 2020 2073 6f72   a != b].    sor
+0000eee0: 7465 645f 6d61 7463 6865 7320 3d20 736f  ted_matches = so
+0000eef0: 7274 6564 286d 6174 6368 6573 2c20 7265  rted(matches, re
+0000ef00: 7665 7273 653d 5472 7565 2c20 6b65 793d  verse=True, key=
+0000ef10: 6c61 6d62 6461 206d 5f77 5f77 6569 6768  lambda m_w_weigh
+0000ef20: 743a 206d 5f77 5f77 6569 6768 745b 325d  t: m_w_weight[2]
+0000ef30: 290a 2020 2020 0a20 2020 2072 6574 7572  ).    .    retur
+0000ef40: 6e20 736f 7274 6564 285f 7369 6d70 6c65  n sorted(_simple
+0000ef50: 5f73 7461 626c 655f 766f 7469 6e67 2863  _stable_voting(c
+0000ef60: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000ef70: 5f63 616e 6473 2c20 0a20 2020 2020 2020  _cands, .       
+0000ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+0000efb0: 3d20 736f 7274 6564 5f6d 6174 6368 6573  = sorted_matches
+0000efc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000efd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efe0: 2020 2020 2020 2020 2020 6d65 6d5f 7376            mem_sv
+0000eff0: 5f77 696e 6e65 7273 203d 207b 7d29 5b30  _winners = {})[0
+0000f000: 5d29 0a0a 4076 6d28 6e61 6d65 203d 2022  ])..@vm(name = "
+0000f010: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
+0000f020: 7469 6e67 222c 0a20 2020 2069 6e70 7574  ting",.    input
+0000f030: 5f74 7970 6573 203d 205b 456c 6563 7469  _types = [Electi
+0000f040: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
+0000f050: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
+0000f060: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
+0000f070: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
+0000f080: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
+0000f090: 6566 2073 696d 706c 655f 7374 6162 6c65  ef simple_stable
+0000f0a0: 5f76 6f74 696e 6728 0a20 2020 2065 6461  _voting(.    eda
+0000f0b0: 7461 2c20 0a20 2020 2063 7572 725f 6361  ta, .    curr_ca
+0000f0c0: 6e64 733d 4e6f 6e65 2c20 0a20 2020 2073  nds=None, .    s
+0000f0d0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+0000f0e0: 3d4e 6f6e 652c 0a20 2020 2061 6c67 6f72  =None,.    algor
+0000f0f0: 6974 686d 203d 2027 6261 7369 6327 293a  ithm = 'basic'):
+0000f100: 200a 0a20 2020 2022 2222 496d 706c 656d   ..    """Implem
+0000f110: 656e 7461 7469 6f6e 206f 6620 5369 6d70  entation of Simp
+0000f120: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
+0000f130: 2066 726f 6d20 6874 7470 733a 2f2f 6172   from https://ar
+0000f140: 7869 762e 6f72 672f 6162 732f 3231 3038  xiv.org/abs/2108
+0000f150: 2e30 3035 3432 2e20 0a0a 2020 2020 5369  .00542. ..    Si
+0000f160: 6d70 6c65 2053 7461 626c 6520 566f 7469  mple Stable Voti
+0000f170: 6e67 2069 7320 6120 7265 6375 7273 6976  ng is a recursiv
+0000f180: 6520 766f 7469 6e67 206d 6574 686f 6420  e voting method 
+0000f190: 6465 6669 6e65 6420 6173 2066 6f6c 6c6f  defined as follo
+0000f1a0: 7773 3a20 0a0a 2020 2020 312e 2049 6620  ws: ..    1. If 
+0000f1b0: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
+0000f1c0: 6520 6361 6e64 6964 6174 6520 696e 2074  e candidate in t
+0000f1d0: 6865 2070 726f 6669 6c65 2c20 7468 656e  he profile, then
+0000f1e0: 2074 6861 7420 6361 6e64 6964 6174 6520   that candidate 
+0000f1f0: 6973 2074 6865 2077 696e 6e65 722e 200a  is the winner. .
+0000f200: 2020 2020 322e 204f 7264 6572 2074 6865      2. Order the
+0000f210: 2070 6169 7273 203a 6d61 7468 3a60 2861   pairs :math:`(a
+0000f220: 2c62 2960 206f 6620 6361 6e64 6964 6174  ,b)` of candidat
+0000f230: 6573 2066 726f 6d20 6c61 7267 6573 7420  es from largest 
+0000f240: 746f 2073 6d61 6c6c 6573 7420 7661 6c75  to smallest valu
+0000f250: 6520 6f66 2074 6865 206d 6172 6769 6e20  e of the margin 
+0000f260: 6f66 203a 6d61 7468 3a60 6160 206f 7665  of :math:`a` ove
+0000f270: 7220 3a6d 6174 683a 6062 602c 2061 6e64  r :math:`b`, and
+0000f280: 2064 6563 6c61 7265 2061 7320 5369 6d70   declare as Simp
+0000f290: 6c65 2053 7461 626c 6520 566f 7469 6e67  le Stable Voting
+0000f2a0: 2077 696e 6e65 7273 2074 6865 2063 616e   winners the can
+0000f2b0: 6469 6461 7465 2873 2920 3a6d 6174 683a  didate(s) :math:
+0000f2c0: 6061 6020 6672 6f6d 2074 6865 2065 6172  `a` from the ear
+0000f2d0: 6c69 6573 7420 7061 6972 2873 2920 3a6d  liest pair(s) :m
+0000f2e0: 6174 683a 6028 612c 6229 6020 7375 6368  ath:`(a,b)` such
+0000f2f0: 2074 6861 7420 3a6d 6174 683a 6061 6020   that :math:`a` 
+0000f300: 6973 2061 2053 696d 706c 6520 5374 6162  is a Simple Stab
+0000f310: 6c65 2056 6f74 696e 6720 7769 6e6e 6572  le Voting winner
+0000f320: 2069 6e20 7468 6520 656c 6563 7469 6f6e   in the election
+0000f330: 2077 6974 686f 7574 203a 6d61 7468 3a60   without :math:`
+0000f340: 6260 2e20 0a0a 2020 2020 4172 6773 3a0a  b`. ..    Args:.
+0000f350: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+0000f360: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+0000f370: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+0000f380: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+0000f390: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+0000f3a0: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+0000f3b0: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
+0000f3c0: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
+0000f3d0: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
+0000f3e0: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
+0000f3f0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
+0000f400: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
+0000f410: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
+0000f420: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
+0000f430: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
+0000f440: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
+0000f450: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
+0000f460: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+0000f470: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
+0000f480: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
+0000f490: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
+0000f4a0: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
+0000f4b0: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
+0000f4c0: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
+0000f4d0: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
+0000f4e0: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
+0000f4f0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
+0000f500: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
+0000f510: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
+0000f520: 0a20 2020 2020 2020 2061 6c67 6f72 6974  .        algorit
+0000f530: 686d 2028 7374 722c 206f 7074 696f 6e61  hm (str, optiona
+0000f540: 6c29 3a20 5370 6563 6966 7920 7768 6963  l): Specify whic
+0000f550: 6820 616c 676f 7269 7468 6d20 746f 2075  h algorithm to u
+0000f560: 7365 2e20 204f 7074 696f 6e73 2061 7265  se.  Options are
+0000f570: 2027 6261 7369 6327 2028 7468 6520 6465   'basic' (the de
+0000f580: 6661 756c 7429 2061 6e64 2027 7769 7468  fault) and 'with
+0000f590: 5f63 6f6e 646f 7263 6574 5f63 6865 636b  _condorcet_check
+0000f5a0: 272e 0a0a 2020 2020 5265 7475 726e 733a  '...    Returns:
+0000f5b0: 200a 2020 2020 2020 2020 4120 736f 7274   .        A sort
+0000f5c0: 6564 206c 6973 7420 6f66 2063 616e 6469  ed list of candi
+0000f5d0: 6461 7465 732e 200a 0a20 2020 202e 2e20  dates. ..    .. 
+0000f5e0: 7365 6561 6c73 6f3a 3a0a 0a20 2020 2020  seealso::..     
+0000f5f0: 2020 203a 6d65 7468 3a60 7072 6566 5f76     :meth:`pref_v
+0000f600: 6f74 696e 672e 6d61 7267 696e 5f62 6173  oting.margin_bas
+0000f610: 6564 5f6d 6574 686f 6473 2e73 7461 626c  ed_methods.stabl
+0000f620: 655f 766f 7469 6e67 600a 0a20 2020 203a  e_voting`..    :
+0000f630: 4578 616d 706c 653a 200a 0a20 2020 202e  Example: ..    .
+0000f640: 2e20 6578 6563 5f63 6f64 653a 3a0a 0a20  . exec_code::.. 
+0000f650: 2020 2020 2020 2066 726f 6d20 7072 6566         from pref
+0000f660: 5f76 6f74 696e 672e 7765 6967 6874 6564  _voting.weighted
+0000f670: 5f6d 616a 6f72 6974 795f 6772 6170 6873  _majority_graphs
+0000f680: 2069 6d70 6f72 7420 4d61 7267 696e 4772   import MarginGr
+0000f690: 6170 680a 2020 2020 2020 2020 6672 6f6d  aph.        from
+0000f6a0: 2070 7265 665f 766f 7469 6e67 2e6d 6172   pref_voting.mar
+0000f6b0: 6769 6e5f 6261 7365 645f 6d65 7468 6f64  gin_based_method
+0000f6c0: 7320 696d 706f 7274 2073 696d 706c 655f  s import simple_
+0000f6d0: 7374 6162 6c65 5f76 6f74 696e 670a 0a20  stable_voting.. 
+0000f6e0: 2020 2020 2020 206d 6720 3d20 4d61 7267         mg = Marg
+0000f6f0: 696e 4772 6170 6828 5b30 2c20 312c 2032  inGraph([0, 1, 2
+0000f700: 2c20 335d 2c20 5b28 302c 2033 2c20 3829  , 3], [(0, 3, 8)
+0000f710: 2c20 2831 2c20 302c 2031 3029 2c20 2832  , (1, 0, 10), (2
+0000f720: 2c20 302c 2034 292c 2028 322c 2031 2c20  , 0, 4), (2, 1, 
+0000f730: 3829 2c20 2833 2c20 312c 2038 295d 290a  8), (3, 1, 8)]).
+0000f740: 0a20 2020 2020 2020 2073 696d 706c 655f  .        simple_
+0000f750: 7374 6162 6c65 5f76 6f74 696e 672e 6469  stable_voting.di
+0000f760: 7370 6c61 7928 6d67 290a 2020 2020 2020  splay(mg).      
+0000f770: 2020 7369 6d70 6c65 5f73 7461 626c 655f    simple_stable_
+0000f780: 766f 7469 6e67 2e64 6973 706c 6179 286d  voting.display(m
+0000f790: 672c 2061 6c67 6f72 6974 686d 3d27 6261  g, algorithm='ba
+0000f7a0: 7369 6327 290a 2020 2020 2020 2020 7369  sic').        si
+0000f7b0: 6d70 6c65 5f73 7461 626c 655f 766f 7469  mple_stable_voti
+0000f7c0: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
+0000f7d0: 6c67 6f72 6974 686d 3d27 7769 7468 5f63  lgorithm='with_c
+0000f7e0: 6f6e 646f 7263 6574 5f63 6865 636b 2729  ondorcet_check')
+0000f7f0: 0a0a 2020 2020 2222 220a 2020 2020 0a20  ..    """.    . 
+0000f800: 2020 2069 6620 616c 676f 7269 7468 6d20     if algorithm 
+0000f810: 3d3d 2027 6261 7369 6327 3a20 0a20 2020  == 'basic': .   
+0000f820: 2020 2020 2072 6574 7572 6e20 5f73 696d       return _sim
+0000f830: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000f840: 675f 6261 7369 6328 6564 6174 612c 2063  g_basic(edata, c
+0000f850: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+0000f860: 5f63 616e 6473 2c20 7374 7265 6e67 7468  _cands, strength
+0000f870: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
+0000f880: 6e67 7468 5f66 756e 6374 696f 6e29 0a20  ngth_function). 
+0000f890: 2020 2065 6c69 6620 616c 676f 7269 7468     elif algorith
+0000f8a0: 6d20 3d3d 2027 7769 7468 5f63 6f6e 646f  m == 'with_condo
+0000f8b0: 7263 6574 5f63 6865 636b 273a 0a20 2020  rcet_check':.   
+0000f8c0: 2020 2020 2072 6574 7572 6e20 5f73 696d       return _sim
+0000f8d0: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+0000f8e0: 675f 7769 7468 5f63 6f6e 646f 7263 6574  g_with_condorcet
+0000f8f0: 5f63 6865 636b 2865 6461 7461 2c20 6375  _check(edata, cu
+0000f900: 7272 5f63 616e 6473 203d 2063 7572 725f  rr_cands = curr_
+0000f910: 6361 6e64 732c 2073 7472 656e 6774 685f  cands, strength_
+0000f920: 6675 6e63 7469 6f6e 203d 2073 7472 656e  function = stren
+0000f930: 6774 685f 6675 6e63 7469 6f6e 290a 2020  gth_function).  
+0000f940: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000f950: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+0000f960: 2822 496e 7661 6c69 6420 616c 676f 7269  ("Invalid algori
+0000f970: 7468 6d20 7370 6563 6966 6965 642e 2229  thm specified.")
+0000f980: 0a20 2020 200a 0a64 6566 205f 7374 6162  .    ..def _stab
+0000f990: 6c65 5f76 6f74 696e 6728 6564 6174 612c  le_voting(edata,
+0000f9a0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000f9b0: 2020 2020 2063 7572 725f 6361 6e64 732c       curr_cands,
+0000f9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f9d0: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
+0000f9e0: 6374 696f 6e2c 0a20 2020 2020 2020 2020  ction,.         
+0000f9f0: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
+0000fa00: 5f6d 6174 6368 6573 2c0a 2020 2020 2020  _matches,.      
+0000fa10: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000fa20: 5f73 765f 7769 6e6e 6572 7329 3a20 0a20  _sv_winners): . 
+0000fa30: 2020 2027 2727 0a20 2020 2044 6574 6572     '''.    Deter
+0000fa40: 6d69 6e65 2074 6865 2053 7461 626c 6520  mine the Stable 
+0000fa50: 566f 7469 6e67 2077 696e 6e65 7273 2066  Voting winners f
+0000fa60: 6f72 2074 6865 2070 726f 6669 6c65 2077  or the profile w
+0000fa70: 6869 6c65 206b 6565 7069 6e67 2074 7261  hile keeping tra
+0000fa80: 636b 206f 6620 7468 6520 7769 6e6e 6572  ck of the winner
+0000fa90: 7320 696e 2061 6e79 2073 7562 7072 6f66  s in any subprof
+0000faa0: 696c 6573 2063 6865 636b 6564 2064 7572  iles checked dur
+0000fab0: 696e 6720 636f 6d70 7574 6174 696f 6e2e  ing computation.
+0000fac0: 200a 2020 2020 2727 270a 2020 2020 0a20   .    '''.    . 
+0000fad0: 2020 2073 765f 7769 6e6e 6572 7320 3d20     sv_winners = 
+0000fae0: 6c69 7374 2829 0a20 2020 200a 2020 2020  list().    .    
+0000faf0: 756e 6465 6665 6174 6564 5f63 616e 6469  undefeated_candi
+0000fb00: 6461 7465 7320 3d20 7370 6c69 745f 6379  dates = split_cy
+0000fb10: 636c 6528 6564 6174 612c 2063 7572 725f  cle(edata, curr_
+0000fb20: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+0000fb30: 6473 2c20 7374 7265 6e67 7468 5f66 756e  ds, strength_fun
+0000fb40: 6374 696f 6e20 3d20 7374 7265 6e67 7468  ction = strength
+0000fb50: 5f66 756e 6374 696f 6e29 0a0a 2020 2020  _function)..    
+0000fb60: 6966 206c 656e 2863 7572 725f 6361 6e64  if len(curr_cand
+0000fb70: 7329 203d 3d20 313a 200a 2020 2020 2020  s) == 1: .      
+0000fb80: 2020 6d65 6d5f 7376 5f77 696e 6e65 7273    mem_sv_winners
+0000fb90: 5b74 7570 6c65 2863 7572 725f 6361 6e64  [tuple(curr_cand
+0000fba0: 7329 5d20 3d20 6375 7272 5f63 616e 6473  s)] = curr_cands
+0000fbb0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fbc0: 6375 7272 5f63 616e 6473 2c20 6d65 6d5f  curr_cands, mem_
+0000fbd0: 7376 5f77 696e 6e65 7273 0a20 2020 200a  sv_winners.    .
+0000fbe0: 2020 2020 6d61 7267 696e 5f77 6974 6e65      margin_witne
+0000fbf0: 7373 696e 675f 7769 6e20 3d20 2d6d 6174  ssing_win = -mat
+0000fc00: 682e 696e 660a 0a20 2020 2066 6f72 2061  h.inf..    for a
+0000fc10: 2c20 622c 2073 2069 6e20 736f 7274 6564  , b, s in sorted
+0000fc20: 5f6d 6174 6368 6573 3a0a 2020 2020 2020  _matches:.      
+0000fc30: 2020 6966 2073 203c 206d 6172 6769 6e5f    if s < margin_
+0000fc40: 7769 746e 6573 7369 6e67 5f77 696e 3a20  witnessing_win: 
+0000fc50: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
+0000fc60: 616b 0a20 2020 2020 2020 2069 6620 6120  ak.        if a 
+0000fc70: 696e 2075 6e64 6566 6561 7465 645f 6361  in undefeated_ca
+0000fc80: 6e64 6964 6174 6573 2061 6e64 2061 206e  ndidates and a n
+0000fc90: 6f74 2069 6e20 7376 5f77 696e 6e65 7273  ot in sv_winners
+0000fca0: 3a20 0a20 2020 2020 2020 2020 2020 2063  : .            c
+0000fcb0: 616e 6473 5f6d 696e 7573 5f62 203d 205b  ands_minus_b = [
+0000fcc0: 6320 666f 7220 6320 696e 2063 7572 725f  c for c in curr_
+0000fcd0: 6361 6e64 7320 6966 2063 2021 3d20 625d  cands if c != b]
+0000fce0: 0a20 2020 2020 2020 2020 2020 2063 616e  .            can
+0000fcf0: 6473 5f6d 696e 7573 5f62 5f6b 6579 203d  ds_minus_b_key =
+0000fd00: 2074 7570 6c65 2873 6f72 7465 6428 6361   tuple(sorted(ca
+0000fd10: 6e64 735f 6d69 6e75 735f 6229 290a 2020  nds_minus_b)).  
+0000fd20: 2020 2020 2020 2020 2020 6966 2063 616e            if can
+0000fd30: 6473 5f6d 696e 7573 5f62 5f6b 6579 206e  ds_minus_b_key n
+0000fd40: 6f74 2069 6e20 6d65 6d5f 7376 5f77 696e  ot in mem_sv_win
+0000fd50: 6e65 7273 2e6b 6579 7328 293a 200a 2020  ners.keys(): .  
+0000fd60: 2020 2020 2020 2020 2020 2020 2020 7773                ws
+0000fd70: 2c20 6d65 6d5f 7376 5f77 696e 6e65 7273  , mem_sv_winners
+0000fd80: 203d 205f 7374 6162 6c65 5f76 6f74 696e   = _stable_votin
+0000fd90: 6728 6564 6174 612c 0a20 2020 2020 2020  g(edata,.       
+0000fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fdc0: 2020 2020 2020 2020 2020 2020 2063 7572               cur
+0000fdd0: 725f 6361 6e64 7320 3d20 6361 6e64 735f  r_cands = cands_
+0000fde0: 6d69 6e75 735f 622c 0a20 2020 2020 2020  minus_b,.       
+0000fdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe10: 2020 2020 2020 2020 2020 2020 2073 7472               str
+0000fe20: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+0000fe30: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+0000fe40: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
+0000fe50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe70: 2020 2020 2020 2020 736f 7274 6564 5f6d          sorted_m
+0000fe80: 6174 6368 6573 203d 205b 2861 2c20 632c  atches = [(a, c,
+0000fe90: 2073 2920 666f 7220 612c 2063 2c20 7320   s) for a, c, s 
+0000fea0: 696e 2073 6f72 7465 645f 6d61 7463 6865  in sorted_matche
+0000feb0: 7320 6966 2061 2021 3d20 6220 616e 6420  s if a != b and 
+0000fec0: 6320 213d 2062 5d2c 0a20 2020 2020 2020  c != b],.       
+0000fed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fef0: 2020 2020 2020 2020 2020 2020 206d 656d               mem
+0000ff00: 5f73 765f 7769 6e6e 6572 7320 3d20 6d65  _sv_winners = me
+0000ff10: 6d5f 7376 5f77 696e 6e65 7273 290a 2020  m_sv_winners).  
+0000ff20: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000ff30: 6d5f 7376 5f77 696e 6e65 7273 5b63 616e  m_sv_winners[can
+0000ff40: 6473 5f6d 696e 7573 5f62 5f6b 6579 5d20  ds_minus_b_key] 
+0000ff50: 3d20 7773 0a20 2020 2020 2020 2020 2020  = ws.           
+0000ff60: 2065 6c73 653a 200a 2020 2020 2020 2020   else: .        
+0000ff70: 2020 2020 2020 2020 7773 203d 206d 656d          ws = mem
+0000ff80: 5f73 765f 7769 6e6e 6572 735b 6361 6e64  _sv_winners[cand
+0000ff90: 735f 6d69 6e75 735f 625f 6b65 795d 0a20  s_minus_b_key]. 
+0000ffa0: 2020 2020 2020 2020 2020 2069 6620 6120             if a 
+0000ffb0: 696e 2077 733a 0a20 2020 2020 2020 2020  in ws:.         
+0000ffc0: 2020 2020 2020 2073 765f 7769 6e6e 6572         sv_winner
+0000ffd0: 732e 6170 7065 6e64 2861 290a 2020 2020  s.append(a).    
+0000ffe0: 2020 2020 2020 2020 2020 2020 6d61 7267              marg
+0000fff0: 696e 5f77 6974 6e65 7373 696e 675f 7769  in_witnessing_wi
+00010000: 6e20 3d20 730a 2020 2020 2020 2020 2020  n = s.          
+00010010: 2020 2020 2020 0a20 2020 2072 6574 7572        .    retur
+00010020: 6e20 7376 5f77 696e 6e65 7273 2c20 6d65  n sv_winners, me
+00010030: 6d5f 7376 5f77 696e 6e65 7273 0a20 2020  m_sv_winners.   
+00010040: 2020 2020 200a 6465 6620 5f73 7461 626c       .def _stabl
+00010050: 655f 766f 7469 6e67 5f77 6974 685f 636f  e_voting_with_co
+00010060: 6e64 6f72 6365 745f 6368 6563 6b28 0a20  ndorcet_check(. 
+00010070: 2020 2065 6461 7461 2c20 0a20 2020 2063     edata, .    c
+00010080: 7572 725f 6361 6e64 733d 4e6f 6e65 2c20  urr_cands=None, 
+00010090: 0a20 2020 2073 7472 656e 6774 685f 6675  .    strength_fu
+000100a0: 6e63 7469 6f6e 3d4e 6f6e 6529 3a20 0a20  nction=None): . 
+000100b0: 2020 2022 2222 0a20 2020 2053 7461 626c     """.    Stabl
+000100c0: 6520 566f 7469 6e67 2069 7320 436f 6e64  e Voting is Cond
+000100d0: 6f72 6365 7420 636f 6e73 6973 7465 6e74  orcet consistent
+000100e0: 2e20 2020 4974 2069 7320 6661 7374 6572  .   It is faster
+000100f0: 2074 6f20 736b 6970 2065 7865 6375 7469   to skip executi
+00010100: 6e67 2074 6865 2072 6563 7572 7369 7665  ng the recursive
+00010110: 2061 6c67 6f72 6974 686d 2077 6865 6e20   algorithm when 
+00010120: 7468 6572 6520 6973 2061 2043 6f6e 646f  there is a Condo
+00010130: 7263 6574 2077 696e 6e65 722e 2020 0a0a  rcet winner.  ..
+00010140: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00010150: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
+00010160: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
+00010170: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
+00010180: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
+00010190: 7461 2074 6861 7420 6861 7320 6120 606d  ta that has a `m
+000101a0: 6172 6769 6e60 206d 6574 686f 642e 200a  argin` method. .
+000101b0: 2020 2020 2020 2020 6375 7272 5f63 616e          curr_can
+000101c0: 6473 2028 4c69 7374 5b69 6e74 5d2c 206f  ds (List[int], o
+000101d0: 7074 696f 6e61 6c29 3a20 4966 2073 6574  ptional): If set
+000101e0: 2c20 7468 656e 2066 696e 6420 7468 6520  , then find the 
+000101f0: 7769 6e6e 6572 7320 666f 7220 7468 6520  winners for the 
+00010200: 7072 6f66 696c 6520 7265 7374 7269 6374  profile restrict
+00010210: 6564 2074 6f20 7468 6520 6361 6e64 6964  ed to the candid
+00010220: 6174 6573 2069 6e20 6060 6375 7272 5f63  ates in ``curr_c
+00010230: 616e 6473 6060 0a20 2020 2020 2020 2073  ands``.        s
+00010240: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+00010250: 2028 6675 6e63 7469 6f6e 2c20 6f70 7469   (function, opti
+00010260: 6f6e 616c 293a 2054 6865 2073 7472 656e  onal): The stren
+00010270: 6774 6820 6675 6e63 7469 6f6e 2074 6f20  gth function to 
+00010280: 6265 2075 7365 6420 746f 2063 616c 6375  be used to calcu
+00010290: 6c61 7465 2074 6865 2073 7472 656e 6774  late the strengt
+000102a0: 6820 6f66 2061 2070 6174 682e 2020 2054  h of a path.   T
+000102b0: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
+000102c0: 6520 6d61 7267 696e 206d 6574 686f 6420  e margin method 
+000102d0: 6f66 2060 6065 6461 7461 6060 2e20 2020  of ``edata``.   
+000102e0: 5468 6973 206f 6e6c 7920 6d61 7474 6572  This only matter
+000102f0: 7320 7768 656e 2074 6865 2062 616c 6c6f  s when the ballo
+00010300: 7473 2061 7265 206e 6f74 206c 696e 6561  ts are not linea
+00010310: 7220 6f72 6465 7273 2e20 0a0a 2020 2020  r orders. ..    
+00010320: 5265 7475 726e 733a 200a 2020 2020 2020  Returns: .      
+00010330: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+00010340: 6f66 2063 616e 6469 6461 7465 732e 200a  of candidates. .
+00010350: 0a20 2020 2022 2222 0a20 2020 2063 7720  .    """.    cw 
+00010360: 3d20 6564 6174 612e 636f 6e64 6f72 6365  = edata.condorce
+00010370: 745f 7769 6e6e 6572 2863 7572 725f 6361  t_winner(curr_ca
+00010380: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
+00010390: 290a 2020 2020 6966 2063 7720 6973 206e  ).    if cw is n
+000103a0: 6f74 204e 6f6e 653a 200a 2020 2020 2020  ot None: .      
+000103b0: 2020 7265 7475 726e 205b 6377 5d0a 2020    return [cw].  
+000103c0: 2020 656c 7365 3a20 0a20 2020 2020 2020    else: .       
+000103d0: 2063 7572 725f 6361 6e64 7320 3d20 6564   curr_cands = ed
+000103e0: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
+000103f0: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
+00010400: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
+00010410: 616e 6473 0a20 2020 2020 2020 2073 7472  ands.        str
+00010420: 656e 6774 685f 6675 6e63 7469 6f6e 203d  ength_function =
+00010430: 2065 6461 7461 2e6d 6172 6769 6e20 6966   edata.margin if
+00010440: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00010450: 6f6e 2069 7320 4e6f 6e65 2065 6c73 6520  on is None else 
+00010460: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00010470: 6e20 200a 0a20 2020 2020 2020 206d 6174  n  ..        mat
+00010480: 6368 6573 203d 205b 2861 2c20 622c 2073  ches = [(a, b, s
+00010490: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+000104a0: 2861 2c20 6229 2920 666f 7220 6120 696e  (a, b)) for a in
+000104b0: 2063 7572 725f 6361 6e64 7320 666f 7220   curr_cands for 
+000104c0: 6220 696e 2063 7572 725f 6361 6e64 7320  b in curr_cands 
+000104d0: 6966 2061 2021 3d20 625d 0a20 2020 2020  if a != b].     
+000104e0: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
+000104f0: 7320 3d20 736f 7274 6564 286d 6174 6368  s = sorted(match
+00010500: 6573 2c20 7265 7665 7273 653d 5472 7565  es, reverse=True
+00010510: 2c20 6b65 793d 6c61 6d62 6461 206d 5f77  , key=lambda m_w
+00010520: 5f77 6569 6768 743a 206d 5f77 5f77 6569  _weight: m_w_wei
+00010530: 6768 745b 325d 290a 0a20 2020 2020 2020  ght[2])..       
+00010540: 2072 6574 7572 6e20 736f 7274 6564 285f   return sorted(_
+00010550: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
+00010560: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
 00010570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010580: 2020 2063 7572 725f 6361 6e64 7320 3d20     curr_cands = 
-00010590: 6361 6e64 735f 6d69 6e75 735f 622c 0a20  cands_minus_b,. 
-000105a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010580: 2020 2020 2020 2020 2020 6375 7272 5f63            curr_c
+00010590: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+000105a0: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
 000105b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105d0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-000105e0: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
-000105f0: 6675 6e63 7469 6f6e 2c0a 2020 2020 2020  function,.      
+000105c0: 2020 2020 2020 2020 7374 7265 6e67 7468          strength
+000105d0: 5f66 756e 6374 696f 6e20 3d20 7374 7265  _function = stre
+000105e0: 6e67 7468 5f66 756e 6374 696f 6e2c 0a20  ngth_function,. 
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00010600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010620: 2020 2020 2020 2020 2020 2020 2020 736f                so
-00010630: 7274 6564 5f6d 6174 6368 6573 203d 205b  rted_matches = [
-00010640: 2861 2c20 632c 2073 2920 666f 7220 612c  (a, c, s) for a,
-00010650: 2063 2c20 7320 696e 2073 6f72 7465 645f   c, s in sorted_
-00010660: 6d61 7463 6865 7320 6966 2061 2021 3d20  matches if a != 
-00010670: 6220 616e 6420 6320 213d 2062 5d2c 0a20  b and c != b],. 
-00010680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106b0: 2020 206d 656d 5f73 765f 7769 6e6e 6572     mem_sv_winner
-000106c0: 7320 3d20 6d65 6d5f 7376 5f77 696e 6e65  s = mem_sv_winne
-000106d0: 7273 290a 2020 2020 2020 2020 2020 2020  rs).            
-000106e0: 2020 2020 6d65 6d5f 7376 5f77 696e 6e65      mem_sv_winne
-000106f0: 7273 5b63 616e 6473 5f6d 696e 7573 5f62  rs[cands_minus_b
-00010700: 5f6b 6579 5d20 3d20 7773 0a20 2020 2020  _key] = ws.     
-00010710: 2020 2020 2020 2065 6c73 653a 200a 2020         else: .  
-00010720: 2020 2020 2020 2020 2020 2020 2020 7773                ws
-00010730: 203d 206d 656d 5f73 765f 7769 6e6e 6572   = mem_sv_winner
-00010740: 735b 6361 6e64 735f 6d69 6e75 735f 625f  s[cands_minus_b_
-00010750: 6b65 795d 0a20 2020 2020 2020 2020 2020  key].           
-00010760: 2069 6620 6120 696e 2077 733a 0a20 2020   if a in ws:.   
-00010770: 2020 2020 2020 2020 2020 2020 2073 765f               sv_
-00010780: 7769 6e6e 6572 732e 6170 7065 6e64 2861  winners.append(a
-00010790: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000107a0: 2020 6d61 7267 696e 5f77 6974 6e65 7373    margin_witness
-000107b0: 696e 675f 7769 6e20 3d20 730a 2020 2020  ing_win = s.    
-000107c0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-000107d0: 2072 6574 7572 6e20 7376 5f77 696e 6e65   return sv_winne
-000107e0: 7273 2c20 6d65 6d5f 7376 5f77 696e 6e65  rs, mem_sv_winne
-000107f0: 7273 0a20 2020 2020 2020 200a 6465 6620  rs.        .def 
-00010800: 5f73 7461 626c 655f 766f 7469 6e67 5f77  _stable_voting_w
-00010810: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
-00010820: 6563 6b28 0a20 2020 2065 6461 7461 2c20  eck(.    edata, 
-00010830: 0a20 2020 2063 7572 725f 6361 6e64 733d  .    curr_cands=
-00010840: 4e6f 6e65 2c20 0a20 2020 2073 7472 656e  None, .    stren
-00010850: 6774 685f 6675 6e63 7469 6f6e 3d4e 6f6e  gth_function=Non
-00010860: 6529 3a20 0a20 2020 2022 2222 0a20 2020  e): .    """.   
-00010870: 2053 7461 626c 6520 566f 7469 6e67 2069   Stable Voting i
-00010880: 7320 436f 6e64 6f72 6365 7420 636f 6e73  s Condorcet cons
-00010890: 6973 7465 6e74 2e20 2020 4974 2069 7320  istent.   It is 
-000108a0: 6661 7374 6572 2074 6f20 736b 6970 2065  faster to skip e
-000108b0: 7865 6375 7469 6e67 2074 6865 2072 6563  xecuting the rec
-000108c0: 7572 7369 7665 2061 6c67 6f72 6974 686d  ursive algorithm
-000108d0: 2077 6865 6e20 7468 6572 6520 6973 2061   when there is a
-000108e0: 2043 6f6e 646f 7263 6574 2077 696e 6e65   Condorcet winne
-000108f0: 722e 2020 0a0a 2020 2020 4172 6773 3a0a  r.  ..    Args:.
-00010900: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
-00010910: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
-00010920: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
-00010930: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
-00010940: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
-00010950: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
-00010960: 686f 642e 200a 2020 2020 2020 2020 6375  hod. .        cu
-00010970: 7272 5f63 616e 6473 2028 4c69 7374 5b69  rr_cands (List[i
-00010980: 6e74 5d2c 206f 7074 696f 6e61 6c29 3a20  nt], optional): 
-00010990: 4966 2073 6574 2c20 7468 656e 2066 696e  If set, then fin
-000109a0: 6420 7468 6520 7769 6e6e 6572 7320 666f  d the winners fo
-000109b0: 7220 7468 6520 7072 6f66 696c 6520 7265  r the profile re
-000109c0: 7374 7269 6374 6564 2074 6f20 7468 6520  stricted to the 
-000109d0: 6361 6e64 6964 6174 6573 2069 6e20 6060  candidates in ``
-000109e0: 6375 7272 5f63 616e 6473 6060 0a20 2020  curr_cands``.   
-000109f0: 2020 2020 2073 7472 656e 6774 685f 6675       strength_fu
-00010a00: 6e63 7469 6f6e 2028 6675 6e63 7469 6f6e  nction (function
-00010a10: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00010a20: 2073 7472 656e 6774 6820 6675 6e63 7469   strength functi
-00010a30: 6f6e 2074 6f20 6265 2075 7365 6420 746f  on to be used to
-00010a40: 2063 616c 6375 6c61 7465 2074 6865 2073   calculate the s
-00010a50: 7472 656e 6774 6820 6f66 2061 2070 6174  trength of a pat
-00010a60: 682e 2020 2054 6865 2064 6566 6175 6c74  h.   The default
-00010a70: 2069 7320 7468 6520 6d61 7267 696e 206d   is the margin m
-00010a80: 6574 686f 6420 6f66 2060 6065 6461 7461  ethod of ``edata
-00010a90: 6060 2e20 2020 5468 6973 206f 6e6c 7920  ``.   This only 
-00010aa0: 6d61 7474 6572 7320 7768 656e 2074 6865  matters when the
-00010ab0: 2062 616c 6c6f 7473 2061 7265 206e 6f74   ballots are not
-00010ac0: 206c 696e 6561 7220 6f72 6465 7273 2e20   linear orders. 
-00010ad0: 0a0a 2020 2020 5265 7475 726e 733a 200a  ..    Returns: .
-00010ae0: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-00010af0: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00010b00: 7465 732e 200a 0a20 2020 2022 2222 0a20  tes. ..    """. 
-00010b10: 2020 2063 7720 3d20 6564 6174 612e 636f     cw = edata.co
-00010b20: 6e64 6f72 6365 745f 7769 6e6e 6572 2863  ndorcet_winner(c
-00010b30: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
-00010b40: 5f63 616e 6473 290a 2020 2020 6966 2063  _cands).    if c
-00010b50: 7720 6973 206e 6f74 204e 6f6e 653a 200a  w is not None: .
-00010b60: 2020 2020 2020 2020 7265 7475 726e 205b          return [
-00010b70: 6377 5d0a 2020 2020 656c 7365 3a20 0a20  cw].    else: . 
-00010b80: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-00010b90: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00010ba0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00010bb0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00010bc0: 6375 7272 5f63 616e 6473 0a20 2020 2020  curr_cands.     
-00010bd0: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
-00010be0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
-00010bf0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
-00010c00: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
-00010c10: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
-00010c20: 756e 6374 696f 6e20 200a 0a20 2020 2020  unction  ..     
-00010c30: 2020 206d 6174 6368 6573 203d 205b 2861     matches = [(a
-00010c40: 2c20 622c 2073 7472 656e 6774 685f 6675  , b, strength_fu
-00010c50: 6e63 7469 6f6e 2861 2c20 6229 2920 666f  nction(a, b)) fo
-00010c60: 7220 6120 696e 2063 7572 725f 6361 6e64  r a in curr_cand
-00010c70: 7320 666f 7220 6220 696e 2063 7572 725f  s for b in curr_
-00010c80: 6361 6e64 7320 6966 2061 2021 3d20 625d  cands if a != b]
-00010c90: 0a20 2020 2020 2020 2073 6f72 7465 645f  .        sorted_
-00010ca0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
-00010cb0: 286d 6174 6368 6573 2c20 7265 7665 7273  (matches, revers
-00010cc0: 653d 5472 7565 2c20 6b65 793d 6c61 6d62  e=True, key=lamb
-00010cd0: 6461 206d 5f77 5f77 6569 6768 743a 206d  da m_w_weight: m
-00010ce0: 5f77 5f77 6569 6768 745b 325d 290a 0a20  _w_weight[2]).. 
-00010cf0: 2020 2020 2020 2072 6574 7572 6e20 736f         return so
-00010d00: 7274 6564 285f 7374 6162 6c65 5f76 6f74  rted(_stable_vot
-00010d10: 696e 6728 6564 6174 612c 200a 2020 2020  ing(edata, .    
-00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d40: 6375 7272 5f63 616e 6473 203d 2063 7572  curr_cands = cur
-00010d50: 725f 6361 6e64 732c 200a 2020 2020 2020  r_cands, .      
-00010d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d70: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00010d80: 7265 6e67 7468 5f66 756e 6374 696f 6e20  rength_function 
-00010d90: 3d20 7374 7265 6e67 7468 5f66 756e 6374  = strength_funct
-00010da0: 696f 6e2c 0a20 2020 2020 2020 2020 2020  ion,.           
-00010db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010dc0: 2020 2020 2020 2020 2073 6f72 7465 645f           sorted_
-00010dd0: 6d61 7463 6865 7320 3d20 736f 7274 6564  matches = sorted
-00010de0: 5f6d 6174 6368 6573 2c0a 2020 2020 2020  _matches,.      
-00010df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e00: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-00010e10: 6d5f 7376 5f77 696e 6e65 7273 203d 207b  m_sv_winners = {
-00010e20: 7d29 5b30 5d29 0a0a 6465 6620 5f73 7461  })[0])..def _sta
-00010e30: 626c 655f 766f 7469 6e67 5f62 6173 6963  ble_voting_basic
-00010e40: 280a 2020 2020 2020 2020 6564 6174 612c  (.        edata,
-00010e50: 200a 2020 2020 2020 2020 6375 7272 5f63   .        curr_c
-00010e60: 616e 6473 203d 204e 6f6e 652c 200a 2020  ands = None, .  
-00010e70: 2020 2020 2020 7374 7265 6e67 7468 5f66        strength_f
-00010e80: 756e 6374 696f 6e20 3d20 4e6f 6e65 293a  unction = None):
-00010e90: 200a 2020 2020 2222 2249 6d70 6c65 6d65   .    """Impleme
-00010ea0: 6e74 6174 696f 6e20 6f66 2020 5374 6162  ntation of  Stab
-00010eb0: 6c65 2056 6f74 696e 6720 6672 6f6d 2068  le Voting from h
-00010ec0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
-00010ed0: 2f61 6273 2f32 3130 382e 3030 3534 322e  /abs/2108.00542.
-00010ee0: 200a 0a20 2020 2041 7267 733a 0a20 2020   ..    Args:.   
-00010ef0: 2020 2020 2065 6461 7461 2028 5072 6f66       edata (Prof
-00010f00: 696c 652c 2050 726f 6669 6c65 5769 7468  ile, ProfileWith
-00010f10: 5469 6573 2c20 4d61 7267 696e 4772 6170  Ties, MarginGrap
-00010f20: 6829 3a20 416e 7920 656c 6563 7469 6f6e  h): Any election
-00010f30: 2064 6174 6120 7468 6174 2068 6173 2061   data that has a
-00010f40: 2060 6d61 7267 696e 6020 6d65 7468 6f64   `margin` method
-00010f50: 2e20 0a20 2020 2020 2020 2063 7572 725f  . .        curr_
-00010f60: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
-00010f70: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00010f80: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
-00010f90: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
-00010fa0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
-00010fb0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
-00010fc0: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
-00010fd0: 725f 6361 6e64 7360 600a 2020 2020 2020  r_cands``.      
-00010fe0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-00010ff0: 696f 6e20 2866 756e 6374 696f 6e2c 206f  ion (function, o
-00011000: 7074 696f 6e61 6c29 3a20 5468 6520 7374  ptional): The st
-00011010: 7265 6e67 7468 2066 756e 6374 696f 6e20  rength function 
-00011020: 746f 2062 6520 7573 6564 2074 6f20 6361  to be used to ca
-00011030: 6c63 756c 6174 6520 7468 6520 7374 7265  lculate the stre
-00011040: 6e67 7468 206f 6620 6120 7061 7468 2e20  ngth of a path. 
-00011050: 2020 5468 6520 6465 6661 756c 7420 6973    The default is
-00011060: 2074 6865 206d 6172 6769 6e20 6d65 7468   the margin meth
-00011070: 6f64 206f 6620 6060 6564 6174 6160 602e  od of ``edata``.
-00011080: 2020 2054 6869 7320 6f6e 6c79 206d 6174     This only mat
-00011090: 7465 7273 2077 6865 6e20 7468 6520 6261  ters when the ba
-000110a0: 6c6c 6f74 7320 6172 6520 6e6f 7420 6c69  llots are not li
-000110b0: 6e65 6172 206f 7264 6572 732e 200a 0a20  near orders. .. 
-000110c0: 2020 2052 6574 7572 6e73 3a20 0a20 2020     Returns: .   
-000110d0: 2020 2020 2041 2073 6f72 7465 6420 6c69       A sorted li
-000110e0: 7374 206f 6620 6361 6e64 6964 6174 6573  st of candidates
-000110f0: 2e20 0a0a 2020 2020 2222 220a 0a20 2020  . ..    """..   
-00011100: 2063 7572 725f 6361 6e64 7320 3d20 6564   curr_cands = ed
-00011110: 6174 612e 6361 6e64 6964 6174 6573 2069  ata.candidates i
-00011120: 6620 6375 7272 5f63 616e 6473 2069 7320  f curr_cands is 
-00011130: 4e6f 6e65 2065 6c73 6520 6375 7272 5f63  None else curr_c
-00011140: 616e 6473 0a20 2020 2073 7472 656e 6774  ands.    strengt
-00011150: 685f 6675 6e63 7469 6f6e 203d 2065 6461  h_function = eda
-00011160: 7461 2e6d 6172 6769 6e20 6966 2073 7472  ta.margin if str
-00011170: 656e 6774 685f 6675 6e63 7469 6f6e 2069  ength_function i
-00011180: 7320 4e6f 6e65 2065 6c73 6520 7374 7265  s None else stre
-00011190: 6e67 7468 5f66 756e 6374 696f 6e20 200a  ngth_function  .
-000111a0: 0a20 2020 206d 6174 6368 6573 203d 205b  .    matches = [
-000111b0: 2861 2c20 622c 2073 7472 656e 6774 685f  (a, b, strength_
-000111c0: 6675 6e63 7469 6f6e 2861 2c20 6229 2920  function(a, b)) 
-000111d0: 666f 7220 6120 696e 2063 7572 725f 6361  for a in curr_ca
-000111e0: 6e64 7320 666f 7220 6220 696e 2063 7572  nds for b in cur
-000111f0: 725f 6361 6e64 7320 6966 2061 2021 3d20  r_cands if a != 
-00011200: 625d 0a20 2020 2073 6f72 7465 645f 6d61  b].    sorted_ma
-00011210: 7463 6865 7320 3d20 736f 7274 6564 286d  tches = sorted(m
-00011220: 6174 6368 6573 2c20 7265 7665 7273 653d  atches, reverse=
-00011230: 5472 7565 2c20 6b65 793d 6c61 6d62 6461  True, key=lambda
-00011240: 206d 5f77 5f77 6569 6768 743a 206d 5f77   m_w_weight: m_w
-00011250: 5f77 6569 6768 745b 325d 290a 0a20 2020  _weight[2])..   
-00011260: 2072 6574 7572 6e20 736f 7274 6564 285f   return sorted(_
-00011270: 7374 6162 6c65 5f76 6f74 696e 6728 6564  stable_voting(ed
-00011280: 6174 612c 200a 2020 2020 2020 2020 2020  ata, .          
-00011290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112a0: 2020 2020 2020 2063 7572 725f 6361 6e64         curr_cand
-000112b0: 7320 3d20 6375 7272 5f63 616e 6473 2c20  s = curr_cands, 
-000112c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000112d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000112e0: 2020 7374 7265 6e67 7468 5f66 756e 6374    strength_funct
-000112f0: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
-00011300: 756e 6374 696f 6e2c 0a20 2020 2020 2020  unction,.       
-00011310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011320: 2020 2020 2020 2020 2020 736f 7274 6564            sorted
-00011330: 5f6d 6174 6368 6573 203d 2073 6f72 7465  _matches = sorte
-00011340: 645f 6d61 7463 6865 732c 0a20 2020 2020  d_matches,.     
-00011350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011360: 2020 2020 2020 2020 2020 2020 6d65 6d5f              mem_
-00011370: 7376 5f77 696e 6e65 7273 203d 207b 7d29  sv_winners = {})
-00011380: 5b30 5d29 0a0a 7376 5f70 726f 7065 7274  [0])..sv_propert
-00011390: 6965 7320 3d20 566f 7469 6e67 4d65 7468  ies = VotingMeth
-000113a0: 6f64 5072 6f70 6572 7469 6573 280a 2020  odProperties(.  
-000113b0: 2020 636f 6e64 6f72 6365 745f 7769 6e6e    condorcet_winn
-000113c0: 6572 3d54 7275 652c 200a 2020 2020 636f  er=True, .    co
-000113d0: 6e64 6f72 6365 745f 6c6f 7365 723d 5472  ndorcet_loser=Tr
-000113e0: 7565 2c0a 2020 2020 7061 7265 746f 5f64  ue,.    pareto_d
-000113f0: 6f6d 696e 616e 6365 3d54 7275 652c 0a20  ominance=True,. 
-00011400: 2020 2070 6f73 6974 6976 655f 696e 766f     positive_invo
-00011410: 6c76 656d 656e 743d 4661 6c73 652c 2020  lvement=False,  
-00011420: 0a20 2020 2029 0a40 766d 286e 616d 6520  .    ).@vm(name 
-00011430: 3d20 2253 7461 626c 6520 566f 7469 6e67  = "Stable Voting
-00011440: 222c 0a20 2020 2070 726f 7065 7274 6965  ",.    propertie
-00011450: 7320 3d20 7376 5f70 726f 7065 7274 6965  s = sv_propertie
-00011460: 732c 0a20 2020 2069 6e70 7574 5f74 7970  s,.    input_typ
-00011470: 6573 203d 205b 456c 6563 7469 6f6e 5479  es = [ElectionTy
-00011480: 7065 732e 5052 4f46 494c 452c 2045 6c65  pes.PROFILE, Ele
-00011490: 6374 696f 6e54 7970 6573 2e50 524f 4649  ctionTypes.PROFI
-000114a0: 4c45 5f57 4954 485f 5449 4553 2c20 456c  LE_WITH_TIES, El
-000114b0: 6563 7469 6f6e 5479 7065 732e 4d41 5247  ectionTypes.MARG
-000114c0: 494e 5f47 5241 5048 5d29 0a64 6566 2073  IN_GRAPH]).def s
-000114d0: 7461 626c 655f 766f 7469 6e67 280a 2020  table_voting(.  
-000114e0: 2020 6564 6174 612c 200a 2020 2020 6375    edata, .    cu
-000114f0: 7272 5f63 616e 6473 3d4e 6f6e 652c 200a  rr_cands=None, .
-00011500: 2020 2020 7374 7265 6e67 7468 5f66 756e      strength_fun
-00011510: 6374 696f 6e3d 4e6f 6e65 2c20 0a20 2020  ction=None, .   
-00011520: 2061 6c67 6f72 6974 686d 3d27 6261 7369   algorithm='basi
-00011530: 6327 293a 200a 2020 2020 2222 2249 6d70  c'): .    """Imp
-00011540: 6c65 6d65 6e74 6174 696f 6e20 6f66 2020  lementation of  
-00011550: 5374 6162 6c65 2056 6f74 696e 6720 6672  Stable Voting fr
-00011560: 6f6d 2068 7474 7073 3a2f 2f61 7278 6976  om https://arxiv
-00011570: 2e6f 7267 2f61 6273 2f32 3130 382e 3030  .org/abs/2108.00
-00011580: 3534 322e 200a 0a20 2020 2053 7461 626c  542. ..    Stabl
-00011590: 6520 566f 7469 6e67 2069 7320 6120 7265  e Voting is a re
-000115a0: 6375 7273 6976 6520 766f 7469 6e67 206d  cursive voting m
-000115b0: 6574 686f 6420 6465 6669 6e65 6420 6173  ethod defined as
-000115c0: 2066 6f6c 6c6f 7773 3a20 0a0a 2020 2020   follows: ..    
-000115d0: 312e 2020 4966 2074 6865 7265 2069 7320  1.  If there is 
-000115e0: 6f6e 6c79 206f 6e65 2063 616e 6469 6461  only one candida
-000115f0: 7465 2069 6e20 7468 6520 7072 6f66 696c  te in the profil
-00011600: 652c 2074 6865 6e20 7468 6174 2063 616e  e, then that can
-00011610: 6469 6461 7465 2069 7320 7468 6520 7769  didate is the wi
-00011620: 6e6e 6572 2e20 0a20 2020 2032 2e20 4f72  nner. .    2. Or
-00011630: 6465 7220 7468 6520 7061 6972 7320 3a6d  der the pairs :m
-00011640: 6174 683a 6028 612c 6229 6020 6f66 2063  ath:`(a,b)` of c
-00011650: 616e 6469 6461 7465 7320 6672 6f6d 206c  andidates from l
-00011660: 6172 6765 7374 2074 6f20 736d 616c 6c65  argest to smalle
-00011670: 7374 2076 616c 7565 206f 6620 7468 6520  st value of the 
-00011680: 6d61 7267 696e 206f 6620 3a6d 6174 683a  margin of :math:
-00011690: 6061 6020 6f76 6572 203a 6d61 7468 3a60  `a` over :math:`
-000116a0: 6260 2073 7563 6820 7468 6174 203a 6d61  b` such that :ma
-000116b0: 7468 3a60 6160 2069 7320 756e 6465 6665  th:`a` is undefe
-000116c0: 6174 6564 2061 6363 6f72 6469 6e67 2074  ated according t
-000116d0: 6f20 5370 6c69 7420 4379 636c 652c 2061  o Split Cycle, a
-000116e0: 6e64 2064 6563 6c61 7265 2061 7320 5374  nd declare as St
-000116f0: 6162 6c65 2056 6f74 696e 6720 7769 6e6e  able Voting winn
-00011700: 6572 7320 7468 6520 6361 6e64 6964 6174  ers the candidat
-00011710: 6528 7329 203a 6d61 7468 3a60 6160 2066  e(s) :math:`a` f
-00011720: 726f 6d20 7468 6520 6561 726c 6965 7374  rom the earliest
-00011730: 2070 6169 7228 7329 203a 6d61 7468 3a60   pair(s) :math:`
-00011740: 2861 2c62 2960 2073 7563 6820 7468 6174  (a,b)` such that
-00011750: 203a 6d61 7468 3a60 6160 2069 7320 6120   :math:`a` is a 
-00011760: 5369 6d70 6c65 2053 7461 626c 6520 566f  Simple Stable Vo
-00011770: 7469 6e67 2077 696e 6e65 7220 696e 2074  ting winner in t
-00011780: 6865 2065 6c65 6374 696f 6e20 7769 7468  he election with
-00011790: 6f75 7420 3a6d 6174 683a 6062 602e 200a  out :math:`b`. .
-000117a0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000117b0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
-000117c0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
-000117d0: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
-000117e0: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
-000117f0: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
-00011800: 6d61 7267 696e 6020 6d65 7468 6f64 2e20  margin` method. 
-00011810: 0a20 2020 2020 2020 2063 7572 725f 6361  .        curr_ca
-00011820: 6e64 7320 284c 6973 745b 696e 745d 2c20  nds (List[int], 
-00011830: 6f70 7469 6f6e 616c 293a 2049 6620 7365  optional): If se
-00011840: 742c 2074 6865 6e20 6669 6e64 2074 6865  t, then find the
-00011850: 2077 696e 6e65 7273 2066 6f72 2074 6865   winners for the
-00011860: 2070 726f 6669 6c65 2072 6573 7472 6963   profile restric
-00011870: 7465 6420 746f 2074 6865 2063 616e 6469  ted to the candi
-00011880: 6461 7465 7320 696e 2060 6063 7572 725f  dates in ``curr_
-00011890: 6361 6e64 7360 600a 2020 2020 2020 2020  cands``.        
-000118a0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
-000118b0: 6e20 2866 756e 6374 696f 6e2c 206f 7074  n (function, opt
-000118c0: 696f 6e61 6c29 3a20 5468 6520 7374 7265  ional): The stre
-000118d0: 6e67 7468 2066 756e 6374 696f 6e20 746f  ngth function to
-000118e0: 2062 6520 7573 6564 2074 6f20 6361 6c63   be used to calc
-000118f0: 756c 6174 6520 7468 6520 7374 7265 6e67  ulate the streng
-00011900: 7468 206f 6620 6120 7061 7468 2e20 2020  th of a path.   
-00011910: 5468 6520 6465 6661 756c 7420 6973 2074  The default is t
-00011920: 6865 206d 6172 6769 6e20 6d65 7468 6f64  he margin method
-00011930: 206f 6620 6060 6564 6174 6160 602e 2020   of ``edata``.  
-00011940: 2054 6869 7320 6f6e 6c79 206d 6174 7465   This only matte
-00011950: 7273 2077 6865 6e20 7468 6520 6261 6c6c  rs when the ball
-00011960: 6f74 7320 6172 6520 6e6f 7420 6c69 6e65  ots are not line
-00011970: 6172 206f 7264 6572 732e 200a 0a20 2020  ar orders. ..   
-00011980: 2052 6574 7572 6e73 3a20 0a20 2020 2020   Returns: .     
-00011990: 2020 2041 2073 6f72 7465 6420 6c69 7374     A sorted list
-000119a0: 206f 6620 6361 6e64 6964 6174 6573 2e20   of candidates. 
-000119b0: 0a0a 2020 2020 2e2e 2073 6565 616c 736f  ..    .. seealso
-000119c0: 3a3a 0a0a 2020 2020 2020 2020 3a6d 6574  ::..        :met
-000119d0: 683a 6070 7265 665f 766f 7469 6e67 2e6d  h:`pref_voting.m
-000119e0: 6172 6769 6e5f 6261 7365 645f 6d65 7468  argin_based_meth
-000119f0: 6f64 732e 7369 6d70 6c65 5f73 7461 626c  ods.simple_stabl
-00011a00: 655f 766f 7469 6e67 600a 0a0a 2020 2020  e_voting`...    
-00011a10: 3a45 7861 6d70 6c65 3a20 0a0a 2020 2020  :Example: ..    
-00011a20: 2e2e 2065 7865 635f 636f 6465 3a3a 0a0a  .. exec_code::..
-00011a30: 2020 2020 2020 2020 6672 6f6d 2070 7265          from pre
-00011a40: 665f 766f 7469 6e67 2e77 6569 6768 7465  f_voting.weighte
-00011a50: 645f 6d61 6a6f 7269 7479 5f67 7261 7068  d_majority_graph
-00011a60: 7320 696d 706f 7274 204d 6172 6769 6e47  s import MarginG
-00011a70: 7261 7068 0a20 2020 2020 2020 2066 726f  raph.        fro
-00011a80: 6d20 7072 6566 5f76 6f74 696e 672e 6d61  m pref_voting.ma
-00011a90: 7267 696e 5f62 6173 6564 5f6d 6574 686f  rgin_based_metho
-00011aa0: 6473 2069 6d70 6f72 7420 7374 6162 6c65  ds import stable
-00011ab0: 5f76 6f74 696e 670a 0a20 2020 2020 2020  _voting..       
-00011ac0: 206d 6720 3d20 4d61 7267 696e 4772 6170   mg = MarginGrap
-00011ad0: 6828 5b30 2c20 312c 2032 2c20 335d 2c20  h([0, 1, 2, 3], 
-00011ae0: 5b28 302c 2033 2c20 3829 2c20 2831 2c20  [(0, 3, 8), (1, 
-00011af0: 302c 2031 3029 2c20 2832 2c20 302c 2034  0, 10), (2, 0, 4
-00011b00: 292c 2028 322c 2031 2c20 3829 2c20 2833  ), (2, 1, 8), (3
-00011b10: 2c20 312c 2038 295d 290a 0a20 2020 2020  , 1, 8)])..     
-00011b20: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
-00011b30: 2e64 6973 706c 6179 286d 6729 0a20 2020  .display(mg).   
-00011b40: 2020 2020 2073 7461 626c 655f 766f 7469       stable_voti
-00011b50: 6e67 2e64 6973 706c 6179 286d 672c 2061  ng.display(mg, a
-00011b60: 6c67 6f72 6974 686d 3d27 6261 7369 6327  lgorithm='basic'
-00011b70: 290a 2020 2020 2020 2020 7374 6162 6c65  ).        stable
-00011b80: 5f76 6f74 696e 672e 6469 7370 6c61 7928  _voting.display(
-00011b90: 6d67 2c20 616c 676f 7269 7468 6d3d 2777  mg, algorithm='w
-00011ba0: 6974 685f 636f 6e64 6f72 6365 745f 6368  ith_condorcet_ch
-00011bb0: 6563 6b27 290a 0a20 2020 2022 2222 0a0a  eck')..    """..
-00011bc0: 2020 2020 6966 2061 6c67 6f72 6974 686d      if algorithm
-00011bd0: 203d 3d20 2762 6173 6963 273a 200a 2020   == 'basic': .  
-00011be0: 2020 2020 2020 7265 7475 726e 205f 7374        return _st
-00011bf0: 6162 6c65 5f76 6f74 696e 675f 6261 7369  able_voting_basi
-00011c00: 6328 6564 6174 612c 2063 7572 725f 6361  c(edata, curr_ca
-00011c10: 6e64 7320 3d20 6375 7272 5f63 616e 6473  nds = curr_cands
-00011c20: 2c20 7374 7265 6e67 7468 5f66 756e 6374  , strength_funct
-00011c30: 696f 6e20 3d20 7374 7265 6e67 7468 5f66  ion = strength_f
-00011c40: 756e 6374 696f 6e29 0a20 2020 2065 6c69  unction).    eli
-00011c50: 6620 616c 676f 7269 7468 6d20 3d3d 2027  f algorithm == '
-00011c60: 7769 7468 5f63 6f6e 646f 7263 6574 5f63  with_condorcet_c
-00011c70: 6865 636b 273a 0a20 2020 2020 2020 2072  heck':.        r
-00011c80: 6574 7572 6e20 5f73 7461 626c 655f 766f  eturn _stable_vo
-00011c90: 7469 6e67 5f77 6974 685f 636f 6e64 6f72  ting_with_condor
-00011ca0: 6365 745f 6368 6563 6b28 6564 6174 612c  cet_check(edata,
-00011cb0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
-00011cc0: 7272 5f63 616e 6473 2c20 7374 7265 6e67  rr_cands, streng
-00011cd0: 7468 5f66 756e 6374 696f 6e20 3d20 7374  th_function = st
-00011ce0: 7265 6e67 7468 5f66 756e 6374 696f 6e29  rength_function)
-00011cf0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-00011d00: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00011d10: 726f 7228 2249 6e76 616c 6964 2061 6c67  ror("Invalid alg
-00011d20: 6f72 6974 686d 2073 7065 6369 6669 6564  orithm specified
-00011d30: 2e22 290a 2020 2020 0a0a 6573 7365 6e74  .").    ..essent
-00011d40: 6961 6c5f 7365 745f 7072 6f70 6572 7469  ial_set_properti
-00011d50: 6573 203d 2056 6f74 696e 674d 6574 686f  es = VotingMetho
-00011d60: 6450 726f 7065 7274 6965 7328 0a20 2020  dProperties(.   
-00011d70: 2063 6f6e 646f 7263 6574 5f77 696e 6e65   condorcet_winne
-00011d80: 723d 5472 7565 2c20 0a20 2020 2063 6f6e  r=True, .    con
-00011d90: 646f 7263 6574 5f6c 6f73 6572 3d54 7275  dorcet_loser=Tru
-00011da0: 652c 0a20 2020 2070 6172 6574 6f5f 646f  e,.    pareto_do
-00011db0: 6d69 6e61 6e63 653d 5472 7565 2c0a 2020  minance=True,.  
-00011dc0: 2020 706f 7369 7469 7665 5f69 6e76 6f6c    positive_invol
-00011dd0: 7665 6d65 6e74 3d46 616c 7365 2c20 0a20  vement=False, . 
-00011de0: 2020 2029 0a40 766d 286e 616d 653d 2245     ).@vm(name="E
-00011df0: 7373 656e 7469 616c 2053 6574 222c 0a20  ssential Set",. 
-00011e00: 2020 2070 726f 7065 7274 6965 733d 6573     properties=es
-00011e10: 7365 6e74 6961 6c5f 7365 745f 7072 6f70  sential_set_prop
-00011e20: 6572 7469 6573 2c0a 2020 2020 696e 7075  erties,.    inpu
-00011e30: 745f 7479 7065 733d 5b45 6c65 6374 696f  t_types=[Electio
-00011e40: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
-00011e50: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-00011e60: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
-00011e70: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
-00011e80: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
-00011e90: 6620 6573 7365 6e74 6961 6c28 6564 6174  f essential(edat
-00011ea0: 612c 2063 7572 725f 6361 6e64 7320 3d20  a, curr_cands = 
-00011eb0: 4e6f 6e65 2c20 7468 7265 7368 6f6c 6420  None, threshold 
-00011ec0: 3d20 302e 3030 3030 3030 3129 3a20 0a20  = 0.0000001): . 
-00011ed0: 2020 2022 2222 5468 6520 4573 7365 6e74     """The Essent
-00011ee0: 6961 6c20 5365 7420 6973 2074 6865 2073  ial Set is the s
-00011ef0: 7570 706f 7274 206f 6620 7468 6520 2863  upport of the (c
-00011f00: 686f 7365 6e29 2043 3220 6d61 7869 6d61  hosen) C2 maxima
-00011f10: 6c20 6c6f 7474 6572 792e 0a0a 2020 2020  l lottery...    
-00011f20: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00011f30: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00011f40: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00011f50: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00011f60: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00011f70: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00011f80: 6e5f 6d61 7472 6978 6020 6174 7472 6962  n_matrix` attrib
-00011f90: 7574 652e 0a20 2020 2020 2020 2063 7572  ute..        cur
-00011fa0: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
-00011fb0: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
-00011fc0: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
-00011fd0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
-00011fe0: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
-00011ff0: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
-00012000: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
-00012010: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
-00012020: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00012030: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
-00012040: 6f66 2063 616e 6469 6461 7465 732e 0a0a  of candidates...
-00012050: 2020 2020 2222 220a 2020 2020 6d6c 203d      """.    ml =
-00012060: 206d 6178 696d 616c 5f6c 6f74 7465 7279   maximal_lottery
-00012070: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
-00012080: 6473 3d63 7572 725f 6361 6e64 7329 0a0a  ds=curr_cands)..
-00012090: 2020 2020 7265 7475 726e 2073 6f72 7465      return sorte
-000120a0: 6428 5b63 2066 6f72 2063 2069 6e20 6d6c  d([c for c in ml
-000120b0: 2e6b 6579 7328 2920 6966 206d 6c5b 635d  .keys() if ml[c]
-000120c0: 203e 2074 6872 6573 686f 6c64 5d29 0a0a   > threshold])..
-000120d0: 7765 6967 6874 6564 5f63 6f76 6572 696e  weighted_coverin
-000120e0: 675f 7072 6f70 6572 7469 6573 203d 2056  g_properties = V
-000120f0: 6f74 696e 674d 6574 686f 6450 726f 7065  otingMethodPrope
-00012100: 7274 6965 7328 0a20 2020 2063 6f6e 646f  rties(.    condo
-00012110: 7263 6574 5f77 696e 6e65 723d 5472 7565  rcet_winner=True
-00012120: 2c20 0a20 2020 2063 6f6e 646f 7263 6574  , .    condorcet
-00012130: 5f6c 6f73 6572 3d54 7275 652c 0a20 2020  _loser=True,.   
-00012140: 2070 6172 6574 6f5f 646f 6d69 6e61 6e63   pareto_dominanc
-00012150: 653d 5472 7565 2c0a 2020 2020 706f 7369  e=True,.    posi
-00012160: 7469 7665 5f69 6e76 6f6c 7665 6d65 6e74  tive_involvement
-00012170: 3d54 7275 652c 200a 2020 2020 290a 4076  =True, .    ).@v
-00012180: 6d28 6e61 6d65 3d22 5765 6967 6874 6564  m(name="Weighted
-00012190: 2043 6f76 6572 696e 6722 2c0a 2020 2020   Covering",.    
-000121a0: 7072 6f70 6572 7469 6573 3d77 6569 6768  properties=weigh
-000121b0: 7465 645f 636f 7665 7269 6e67 5f70 726f  ted_covering_pro
-000121c0: 7065 7274 6965 732c 0a20 2020 2069 6e70  perties,.    inp
-000121d0: 7574 5f74 7970 6573 3d5b 456c 6563 7469  ut_types=[Electi
-000121e0: 6f6e 5479 7065 732e 5052 4f46 494c 452c  onTypes.PROFILE,
-000121f0: 2045 6c65 6374 696f 6e54 7970 6573 2e50   ElectionTypes.P
-00012200: 524f 4649 4c45 5f57 4954 485f 5449 4553  ROFILE_WITH_TIES
-00012210: 2c20 456c 6563 7469 6f6e 5479 7065 732e  , ElectionTypes.
-00012220: 4d41 5247 494e 5f47 5241 5048 5d29 0a64  MARGIN_GRAPH]).d
-00012230: 6566 2077 6569 6768 7465 645f 636f 7665  ef weighted_cove
-00012240: 7269 6e67 2865 6461 7461 2c20 6375 7272  ring(edata, curr
-00012250: 5f63 616e 6473 3d4e 6f6e 6529 3a20 0a20  _cands=None): . 
-00012260: 2020 2022 2222 4163 636f 7264 696e 6720     """According 
-00012270: 746f 2057 6569 6768 7465 6420 436f 7665  to Weighted Cove
-00012280: 7269 6e67 2c20 7820 6465 6665 6174 7320  ring, x defeats 
-00012290: 7920 6966 2074 6865 206d 6172 6769 6e20  y if the margin 
-000122a0: 6f66 2078 206f 7665 7220 7920 6973 2070  of x over y is p
-000122b0: 6f73 6974 6976 6520 616e 6420 666f 7220  ositive and for 
-000122c0: 6576 6572 7920 6f74 6865 7220 7a2c 2074  every other z, t
-000122d0: 6865 206d 6172 6769 6e20 6f66 2078 206f  he margin of x o
-000122e0: 7665 7220 7a20 6973 2067 7265 6174 6572  ver z is greater
-000122f0: 2074 6861 6e20 6f72 2065 7175 616c 2074   than or equal t
-00012300: 6f20 7468 6520 6d61 7267 696e 206f 6620  o the margin of 
-00012310: 7920 6f76 6572 207a 2e20 0a0a 2020 2020  y over z. ..    
-00012320: 4172 6773 3a0a 2020 2020 2020 2020 6564  Args:.        ed
-00012330: 6174 6120 2850 726f 6669 6c65 2c20 5072  ata (Profile, Pr
-00012340: 6f66 696c 6557 6974 6854 6965 732c 204d  ofileWithTies, M
-00012350: 6172 6769 6e47 7261 7068 293a 2041 6e79  arginGraph): Any
-00012360: 2065 6c65 6374 696f 6e20 6461 7461 2074   election data t
-00012370: 6861 7420 6861 7320 6120 606d 6172 6769  hat has a `margi
-00012380: 6e60 206d 6574 686f 642e 0a20 2020 2020  n` method..     
-00012390: 2020 2063 7572 725f 6361 6e64 7320 284c     curr_cands (L
-000123a0: 6973 745b 696e 745d 2c20 6f70 7469 6f6e  ist[int], option
-000123b0: 616c 293a 2049 6620 7365 742c 2074 6865  al): If set, the
-000123c0: 6e20 6669 6e64 2074 6865 2077 696e 6e65  n find the winne
-000123d0: 7273 2066 6f72 2074 6865 2070 726f 6669  rs for the profi
-000123e0: 6c65 2072 6573 7472 6963 7465 6420 746f  le restricted to
-000123f0: 2074 6865 2063 616e 6469 6461 7465 7320   the candidates 
-00012400: 696e 2060 6063 7572 725f 6361 6e64 7360  in ``curr_cands`
-00012410: 600a 0a20 2020 2052 6574 7572 6e73 3a0a  `..    Returns:.
-00012420: 2020 2020 2020 2020 4120 736f 7274 6564          A sorted
-00012430: 206c 6973 7420 6f66 2063 616e 6469 6461   list of candida
-00012440: 7465 732e 0a0a 2020 2020 2e2e 206e 6f74  tes...    .. not
-00012450: 653a 3a0a 2020 2020 2020 2020 5365 652c  e::.        See,
-00012460: 2065 2e67 2e2c 2042 6861 736b 6172 2044   e.g., Bhaskar D
-00012470: 7574 7461 2061 6e64 204a 6561 6e2d 4672  utta and Jean-Fr
-00012480: 616e 636f 6973 204c 6173 6c69 6572 2c20  ancois Laslier, 
-00012490: 2243 6f6d 7061 7269 736f 6e20 6675 6e63  "Comparison func
-000124a0: 7469 6f6e 7320 616e 6420 6368 6f69 6365  tions and choice
-000124b0: 2063 6f72 7265 7370 6f6e 6465 6e63 6573   correspondences
-000124c0: 2c22 2053 6f63 6961 6c20 4368 6f69 6365  ," Social Choice
-000124d0: 2061 6e64 2057 656c 6661 7265 2c20 3136   and Welfare, 16
-000124e0: 3a35 3133 e280 9335 3332 2c20 3139 3939  :513...532, 1999
-000124f0: 2c20 646f 693a 3130 2e31 3030 372f 7330  , doi:10.1007/s0
-00012500: 3033 3535 3030 3530 3135 382c 2061 6e64  03550050158, and
-00012510: 2052 6175 cc81 6c20 5065 cc81 7265 7a2d   Rau..l Pe..rez-
-00012520: 4665 726e 61cc 816e 6465 7a20 616e 6420  Ferna..ndez and 
-00012530: 4265 726e 6172 6420 4465 2042 6165 7473  Bernard De Baets
-00012540: 2c20 2254 6865 2073 7570 6572 636f 7665  , "The supercove
-00012550: 7269 6e67 2072 656c 6174 696f 6e2c 2074  ring relation, t
-00012560: 6865 2070 6169 7277 6973 6520 7769 6e6e  he pairwise winn
-00012570: 6572 2c20 616e 6420 6d6f 7265 206d 6973  er, and more mis
-00012580: 7369 6e67 206c 696e 6b73 2062 6574 7765  sing links betwe
-00012590: 656e 2042 6f72 6461 2061 6e64 2043 6f6e  en Borda and Con
-000125a0: 646f 7263 6574 2c22 2053 6f63 6961 6c20  dorcet," Social 
-000125b0: 4368 6f69 6365 2061 6e64 2057 656c 6661  Choice and Welfa
-000125c0: 7265 2c20 3530 3a33 3239 e280 9333 3532  re, 50:329...352
-000125d0: 2c20 3230 3138 2c20 646f 693a 3130 2e31  , 2018, doi:10.1
-000125e0: 3030 372f 7330 3033 3535 2d30 3137 2d31  007/s00355-017-1
-000125f0: 3038 362d 302e 0a20 2020 2022 2222 0a0a  086-0..    """..
-00012600: 2020 2020 6361 6e64 6964 6174 6573 203d      candidates =
-00012610: 2065 6461 7461 2e63 616e 6469 6461 7465   edata.candidate
-00012620: 7320 6966 2063 7572 725f 6361 6e64 7320  s if curr_cands 
-00012630: 6973 204e 6f6e 6520 656c 7365 2063 7572  is None else cur
-00012640: 725f 6361 6e64 730a 0a20 2020 2075 635f  r_cands..    uc_
-00012650: 7365 7420 3d20 6c69 7374 2829 0a0a 2020  set = list()..  
-00012660: 2020 666f 7220 7920 696e 2063 616e 6469    for y in candi
-00012670: 6461 7465 733a 0a20 2020 2020 2020 2069  dates:.        i
-00012680: 735f 696e 5f75 6373 203d 2054 7275 650a  s_in_ucs = True.
-00012690: 2020 2020 2020 2020 666f 7220 7820 696e          for x in
-000126a0: 2065 6461 7461 2e64 6f6d 696e 6174 6f72   edata.dominator
-000126b0: 7328 792c 2063 7572 725f 6361 6e64 7320  s(y, curr_cands 
-000126c0: 3d20 6375 7272 5f63 616e 6473 293a 0a20  = curr_cands):. 
-000126d0: 2020 2020 2020 2020 2020 2023 2063 6865             # che
-000126e0: 636b 2069 6620 7920 636f 7665 7273 2078  ck if y covers x
-000126f0: 2c20 692e 652e 2c20 666f 7220 6576 6572  , i.e., for ever
-00012700: 7920 7a2c 206d 6172 6769 6e28 782c 207a  y z, margin(x, z
-00012710: 2920 3e3d 206d 6172 6769 6e28 792c 207a  ) >= margin(y, z
-00012720: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
-00012730: 7665 7273 203d 2054 7275 650a 2020 2020  vers = True.    
-00012740: 2020 2020 2020 2020 666f 7220 7a20 696e          for z in
-00012750: 2063 616e 6469 6461 7465 733a 0a20 2020   candidates:.   
-00012760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00012770: 6564 6174 612e 6d61 7267 696e 2878 2c20  edata.margin(x, 
-00012780: 7a29 203c 2065 6461 7461 2e6d 6172 6769  z) < edata.margi
-00012790: 6e28 792c 207a 293a 0a20 2020 2020 2020  n(y, z):.       
-000127a0: 2020 2020 2020 2020 2020 2020 2063 6f76               cov
-000127b0: 6572 7320 3d20 4661 6c73 650a 2020 2020  ers = False.    
-000127c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127d0: 6272 6561 6b0a 2020 2020 2020 2020 2020  break.          
-000127e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000127f0: 636f 7665 7273 3a0a 2020 2020 2020 2020  covers:.        
-00012800: 2020 2020 2020 2020 6973 5f69 6e5f 7563          is_in_uc
-00012810: 7320 3d20 4661 6c73 650a 2020 2020 2020  s = False.      
-00012820: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
-00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012840: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
-00012850: 6e5f 7563 733a 0a20 2020 2020 2020 2020  n_ucs:.         
-00012860: 2020 2075 635f 7365 742e 6170 7065 6e64     uc_set.append
-00012870: 2879 290a 0a20 2020 2072 6574 7572 6e20  (y)..    return 
-00012880: 736f 7274 6564 2875 635f 7365 7429 0a0a  sorted(uc_set)..
-00012890: 6c6f 7373 5f74 7269 6d6d 6572 5f70 726f  loss_trimmer_pro
-000128a0: 7065 7274 6965 7320 3d20 566f 7469 6e67  perties = Voting
-000128b0: 4d65 7468 6f64 5072 6f70 6572 7469 6573  MethodProperties
-000128c0: 280a 2020 2020 636f 6e64 6f72 6365 745f  (.    condorcet_
-000128d0: 7769 6e6e 6572 3d54 7275 652c 200a 2020  winner=True, .  
-000128e0: 2020 636f 6e64 6f72 6365 745f 6c6f 7365    condorcet_lose
-000128f0: 723d 5472 7565 2c0a 2020 2020 7061 7265  r=True,.    pare
-00012900: 746f 5f64 6f6d 696e 616e 6365 3d54 7275  to_dominance=Tru
-00012910: 652c 0a20 2020 2070 6f73 6974 6976 655f  e,.    positive_
-00012920: 696e 766f 6c76 656d 656e 743d 4661 6c73  involvement=Fals
-00012930: 652c 200a 2020 2020 290a 4076 6d28 6e61  e, .    ).@vm(na
-00012940: 6d65 203d 2022 4c6f 7373 2d54 7269 6d6d  me = "Loss-Trimm
-00012950: 6572 2056 6f74 696e 6722 2c0a 2020 2020  er Voting",.    
-00012960: 7072 6f70 6572 7469 6573 203d 206c 6f73  properties = los
-00012970: 735f 7472 696d 6d65 725f 7072 6f70 6572  s_trimmer_proper
-00012980: 7469 6573 2c0a 2020 2020 696e 7075 745f  ties,.    input_
-00012990: 7479 7065 7320 3d20 5b45 6c65 6374 696f  types = [Electio
-000129a0: 6e54 7970 6573 2e50 524f 4649 4c45 2c20  nTypes.PROFILE, 
-000129b0: 456c 6563 7469 6f6e 5479 7065 732e 5052  ElectionTypes.PR
-000129c0: 4f46 494c 455f 5749 5448 5f54 4945 532c  OFILE_WITH_TIES,
-000129d0: 2045 6c65 6374 696f 6e54 7970 6573 2e4d   ElectionTypes.M
-000129e0: 4152 4749 4e5f 4752 4150 485d 290a 6465  ARGIN_GRAPH]).de
-000129f0: 6620 6c6f 7373 5f74 7269 6d6d 6572 2865  f loss_trimmer(e
-00012a00: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
-00012a10: 203d 204e 6f6e 6529 3a0a 2020 2020 2222   = None):.    ""
-00012a20: 2249 7465 7261 7469 7665 6c79 2065 6c69  "Iteratively eli
-00012a30: 6d69 6e61 7465 2074 6865 2063 616e 6469  minate the candi
-00012a40: 6461 7465 2077 6974 6820 7468 6520 6c61  date with the la
-00012a50: 7267 6573 7420 7375 6d20 6f66 206d 6172  rgest sum of mar
-00012a60: 6769 6e73 206f 6620 6c6f 7373 2075 6e74  gins of loss unt
-00012a70: 696c 2061 2043 6f6e 646f 7263 6574 2077  il a Condorcet w
-00012a80: 696e 6e65 7220 6973 2066 6f75 6e64 2e20  inner is found. 
-00012a90: 496e 2074 6869 7320 7665 7273 696f 6e20  In this version 
-00012aa0: 6f66 2074 6865 206d 6574 686f 642c 2070  of the method, p
-00012ab0: 6172 616c 6c65 6c2d 756e 6976 6572 7365  arallel-universe
-00012ac0: 2074 6965 6272 6561 6b69 6e67 2069 7320   tiebreaking is 
-00012ad0: 7573 6564 2069 6620 7468 6572 6520 6172  used if there ar
-00012ae0: 6520 6d75 6c74 6970 6c65 2063 616e 6469  e multiple candi
-00012af0: 6461 7465 7320 7769 7468 2074 6865 206c  dates with the l
-00012b00: 6172 6765 7374 2073 756d 206f 6620 6d61  argest sum of ma
-00012b10: 7267 696e 7320 6f66 206c 6f73 732e 0a0a  rgins of loss...
-00012b20: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00012b30: 2020 6564 6174 6120 2850 726f 6669 6c65    edata (Profile
-00012b40: 2c20 5072 6f66 696c 6557 6974 6854 6965  , ProfileWithTie
-00012b50: 732c 204d 6172 6769 6e47 7261 7068 293a  s, MarginGraph):
-00012b60: 2041 6e79 2065 6c65 6374 696f 6e20 6461   Any election da
-00012b70: 7461 2074 6861 7420 6861 7320 6120 6d61  ta that has a ma
-00012b80: 7267 696e 206d 6574 686f 642e 0a20 2020  rgin method..   
-00012b90: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
-00012ba0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
-00012bb0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
-00012bc0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
-00012bd0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
-00012be0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
-00012bf0: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
-00012c00: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
-00012c10: 7360 600a 0a20 2020 2052 6574 7572 6e73  s``..    Returns
-00012c20: 3a20 0a20 2020 2020 2020 2041 2073 6f72  : .        A sor
-00012c30: 7465 6420 6c69 7374 206f 6620 6361 6e64  ted list of cand
-00012c40: 6964 6174 6573 0a0a 2020 2020 2e2e 206e  idates..    .. n
-00012c50: 6f74 653a 3a0a 2020 2020 2020 2020 4d65  ote::.        Me
-00012c60: 7468 6f64 2070 726f 706f 7365 6420 6279  thod proposed by
-00012c70: 2052 6963 6861 7264 2042 2e20 4461 726c   Richard B. Darl
-00012c80: 696e 6774 6f6e 2069 6e20 2254 6865 2043  ington in "The C
-00012c90: 6173 6520 666f 7220 7468 6520 4c6f 7373  ase for the Loss
-00012ca0: 2d54 7269 6d6d 6572 2056 6f74 696e 6720  -Trimmer Voting 
-00012cb0: 5379 7374 656d 2e22 0a0a 2020 2020 2222  System."..    ""
-00012cc0: 220a 0a20 2020 2063 7572 725f 6361 6e64  "..    curr_cand
-00012cd0: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00012ce0: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00012cf0: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00012d00: 6375 7272 5f63 616e 6473 0a0a 2020 2020  curr_cands..    
-00012d10: 7765 616b 5f63 7720 3d20 6564 6174 612e  weak_cw = edata.
-00012d20: 7765 616b 5f63 6f6e 646f 7263 6574 5f77  weak_condorcet_w
-00012d30: 696e 6e65 7228 6375 7272 5f63 616e 6473  inner(curr_cands
-00012d40: 203d 2063 7572 725f 6361 6e64 7329 0a20   = curr_cands). 
-00012d50: 2020 2023 2049 6620 7468 6572 6520 6172     # If there ar
-00012d60: 6520 7765 616b 2043 6f6e 646f 7263 6574  e weak Condorcet
-00012d70: 2077 696e 6e65 7273 2c20 7265 7475 726e   winners, return
-00012d80: 2074 686f 7365 2063 616e 6469 6461 7465   those candidate
-00012d90: 730a 2020 2020 6966 2065 6461 7461 2e77  s.    if edata.w
-00012da0: 6561 6b5f 636f 6e64 6f72 6365 745f 7769  eak_condorcet_wi
-00012db0: 6e6e 6572 2863 7572 725f 6361 6e64 7320  nner(curr_cands 
-00012dc0: 3d20 6375 7272 5f63 616e 6473 2920 6973  = curr_cands) is
-00012dd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00012de0: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
-00012df0: 2877 6561 6b5f 6377 290a 2020 2020 0a20  (weak_cw).    . 
-00012e00: 2020 2023 204f 7468 6572 7769 7365 2c20     # Otherwise, 
-00012e10: 6361 6c63 756c 6174 6520 7468 6520 7375  calculate the su
-00012e20: 6d20 6f66 206d 6172 6769 6e73 206f 6620  m of margins of 
-00012e30: 6c6f 7373 2066 6f72 2065 6163 6820 6361  loss for each ca
-00012e40: 6e64 6964 6174 650a 2020 2020 7375 6d5f  ndidate.    sum_
-00012e50: 6f66 5f6d 6172 6769 6e73 5f6f 665f 6c6f  of_margins_of_lo
-00012e60: 7373 203d 207b 6361 6e64 3a20 7375 6d28  ss = {cand: sum(
-00012e70: 5b65 6461 7461 2e6d 6172 6769 6e28 6f74  [edata.margin(ot
-00012e80: 6865 725f 6361 6e64 2c20 6361 6e64 2920  her_cand, cand) 
-00012e90: 666f 7220 6f74 6865 725f 6361 6e64 2069  for other_cand i
-00012ea0: 6e20 6375 7272 5f63 616e 6473 2069 6620  n curr_cands if 
-00012eb0: 6564 6174 612e 6d61 7267 696e 286f 7468  edata.margin(oth
-00012ec0: 6572 5f63 616e 642c 2063 616e 6429 203e  er_cand, cand) >
-00012ed0: 2030 5d29 2066 6f72 2063 616e 6420 696e   0]) for cand in
-00012ee0: 2063 7572 725f 6361 6e64 737d 0a0a 2020   curr_cands}..  
-00012ef0: 2020 2320 4669 6e64 2074 6865 2063 616e    # Find the can
-00012f00: 6469 6461 7465 7320 7769 7468 2074 6865  didates with the
-00012f10: 206c 6172 6765 7374 2073 756d 206f 6620   largest sum of 
-00012f20: 6d61 7267 696e 7320 6f66 206c 6f73 730a  margins of loss.
-00012f30: 2020 2020 6d61 785f 7375 6d5f 6f66 5f6d      max_sum_of_m
-00012f40: 6172 6769 6e73 5f6f 665f 6c6f 7373 203d  argins_of_loss =
-00012f50: 206d 6178 2873 756d 5f6f 665f 6d61 7267   max(sum_of_marg
-00012f60: 696e 735f 6f66 5f6c 6f73 732e 7661 6c75  ins_of_loss.valu
-00012f70: 6573 2829 290a 2020 2020 6269 6767 6573  es()).    bigges
-00012f80: 745f 6c6f 7365 7273 203d 205b 6361 6e64  t_losers = [cand
-00012f90: 2066 6f72 2063 616e 6420 696e 2063 7572   for cand in cur
-00012fa0: 725f 6361 6e64 7320 6966 2073 756d 5f6f  r_cands if sum_o
-00012fb0: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
-00012fc0: 735b 6361 6e64 5d20 3d3d 206d 6178 5f73  s[cand] == max_s
-00012fd0: 756d 5f6f 665f 6d61 7267 696e 735f 6f66  um_of_margins_of
-00012fe0: 5f6c 6f73 735d 0a0a 2020 2020 7769 6e6e  _loss]..    winn
-00012ff0: 6572 7320 3d20 5b5d 0a0a 2020 2020 2320  ers = []..    # 
-00013000: 466f 7220 6561 6368 2062 6967 6765 7374  For each biggest
-00013010: 206c 6f73 6572 2c20 6361 6c63 756c 6174   loser, calculat
-00013020: 6520 7468 6520 7769 6e6e 6572 7320 6166  e the winners af
-00013030: 7465 7220 7265 6d6f 7669 6e67 2074 6861  ter removing tha
-00013040: 7420 6361 6e64 6964 6174 652e 2054 6865  t candidate. The
-00013050: 2075 6e69 6f6e 206f 6620 7468 6573 6520   union of these 
-00013060: 7365 7473 2069 7320 7468 6520 7365 7420  sets is the set 
-00013070: 6f66 2077 696e 6e65 7273 2e0a 2020 2020  of winners..    
-00013080: 666f 7220 626c 2069 6e20 6269 6767 6573  for bl in bigges
-00013090: 745f 6c6f 7365 7273 3a0a 2020 2020 2020  t_losers:.      
-000130a0: 2020 7769 6e6e 6572 735f 7769 7468 6f75    winners_withou
-000130b0: 745f 626c 203d 206c 6f73 735f 7472 696d  t_bl = loss_trim
-000130c0: 6d65 7228 6564 6174 612c 2063 7572 725f  mer(edata, curr_
-000130d0: 6361 6e64 7320 3d20 5b63 616e 6420 666f  cands = [cand fo
-000130e0: 7220 6361 6e64 2069 6e20 6375 7272 5f63  r cand in curr_c
-000130f0: 616e 6473 2069 6620 6361 6e64 2021 3d20  ands if cand != 
-00013100: 626c 5d29 0a20 2020 2020 2020 2077 696e  bl]).        win
-00013110: 6e65 7273 202b 3d20 7769 6e6e 6572 735f  ners += winners_
-00013120: 7769 7468 6f75 745f 626c 0a0a 2020 2020  without_bl..    
-00013130: 7265 7475 726e 2073 6f72 7465 6428 6c69  return sorted(li
-00013140: 7374 2873 6574 2877 696e 6e65 7273 2929  st(set(winners))
-00013150: 290a 0a0a 6465 6620 6469 7374 616e 6365  )...def distance
-00013160: 5f74 6f5f 6d61 7267 696e 5f67 7261 7068  _to_margin_graph
-00013170: 2865 6461 7461 2c20 7265 6c2c 2065 7870  (edata, rel, exp
-00013180: 203d 2031 2c20 6375 7272 5f63 616e 6473   = 1, curr_cands
-00013190: 203d 204e 6f6e 6529 3a20 0a20 2020 2022   = None): .    "
-000131a0: 2222 0a20 2020 2043 616c 6375 6c61 7465  "".    Calculate
-000131b0: 2074 6865 2064 6973 7461 6e63 6520 6f66   the distance of
-000131c0: 2060 6072 656c 6060 2028 6120 7265 6c61   ``rel`` (a rela
-000131d0: 7469 6f6e 2920 746f 2074 6865 206d 616a  tion) to the maj
-000131e0: 6f72 6974 7920 6772 6170 6820 6f66 2060  ority graph of `
-000131f0: 6065 6461 7461 6060 2e20 0a20 2020 2022  `edata``. .    "
-00013200: 2222 0a20 2020 2063 616e 6469 6461 7465  "".    candidate
-00013210: 7320 3d20 6564 6174 612e 6361 6e64 6964  s = edata.candid
-00013220: 6174 6573 2069 6620 6375 7272 5f63 616e  ates if curr_can
-00013230: 6473 2069 7320 4e6f 6e65 2065 6c73 6520  ds is None else 
-00013240: 6375 7272 5f63 616e 6473 0a20 2020 200a  curr_cands.    .
-00013250: 2020 2020 6966 2074 7970 6528 6564 6174      if type(edat
-00013260: 6129 203d 3d20 4d61 6a6f 7269 7479 4772  a) == MajorityGr
-00013270: 6170 6820 616e 6420 6578 7020 3d3d 2030  aph and exp == 0
-00013280: 3a0a 2020 2020 2020 2020 2320 6966 2065  :.        # if e
-00013290: 6461 7461 2069 7320 6120 4d61 6a6f 7269  data is a Majori
-000132a0: 7479 4772 6170 682c 2077 6520 6e65 6564  tyGraph, we need
-000132b0: 2074 6f20 6164 6420 6d61 7267 696e 7320   to add margins 
-000132c0: 666f 7220 7468 6520 666f 6c6c 6f77 696e  for the followin
-000132d0: 6720 636f 6465 2074 6f20 776f 726b 2e20  g code to work. 
-000132e0: 2054 6865 206d 6172 6769 6e73 2064 6f20   The margins do 
-000132f0: 6e6f 7420 6d61 7474 6572 2077 6865 6e20  not matter when 
-00013300: 6578 703d 3d30 2e20 2020 0a20 2020 2020  exp==0.   .     
-00013310: 2020 2065 6461 7461 203d 204d 6172 6769     edata = Margi
-00013320: 6e47 7261 7068 2863 616e 6469 6461 7465  nGraph(candidate
-00013330: 732c 205b 2863 312c 2063 322c 2031 2920  s, [(c1, c2, 1) 
-00013340: 666f 7220 6331 2c20 6332 2069 6e20 6564  for c1, c2 in ed
-00013350: 6174 612e 6564 6765 7320 6966 2028 6331  ata.edges if (c1
-00013360: 2069 6e20 6361 6e64 6964 6174 6573 2061   in candidates a
-00013370: 6e64 2063 3220 696e 2063 616e 6469 6461  nd c2 in candida
-00013380: 7465 7329 5d29 0a20 2020 2070 656e 616c  tes)]).    penal
-00013390: 7479 203d 2030 0a20 2020 2066 6f72 2061  ty = 0.    for a
-000133a0: 2c62 2069 6e20 636f 6d62 696e 6174 696f  ,b in combinatio
-000133b0: 6e73 2863 616e 6469 6461 7465 732c 2032  ns(candidates, 2
-000133c0: 293a 200a 2020 2020 2020 2020 6966 2065  ): .        if e
-000133d0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-000133e0: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-000133f0: 2862 2c61 2920 696e 2072 656c 3a20 0a20  (b,a) in rel: . 
-00013400: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-00013410: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-00013420: 6769 6e28 612c 2062 2920 2a2a 2065 7870  gin(a, b) ** exp
-00013430: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-00013440: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-00013450: 6566 6572 7328 622c 2061 2920 616e 6420  efers(b, a) and 
-00013460: 2861 2c62 2920 696e 2072 656c 3a20 0a20  (a,b) in rel: . 
-00013470: 2020 2020 2020 2020 2020 2070 656e 616c             penal
-00013480: 7479 202b 3d20 2865 6461 7461 2e6d 6172  ty += (edata.mar
-00013490: 6769 6e28 622c 2061 2920 2a2a 2065 7870  gin(b, a) ** exp
-000134a0: 290a 2020 2020 2020 2020 656c 6966 2065  ).        elif e
-000134b0: 6461 7461 2e6d 616a 6f72 6974 795f 7072  data.majority_pr
-000134c0: 6566 6572 7328 612c 2062 2920 616e 6420  efers(a, b) and 
-000134d0: 2861 2c62 2920 6e6f 7420 696e 2072 656c  (a,b) not in rel
-000134e0: 2061 6e64 2028 622c 6129 206e 6f74 2069   and (b,a) not i
-000134f0: 6e20 7265 6c3a 200a 2020 2020 2020 2020  n rel: .        
-00013500: 2020 2020 7065 6e61 6c74 7920 2b3d 2028      penalty += (
-00013510: 6564 6174 612e 6d61 7267 696e 2861 2c20  edata.margin(a, 
-00013520: 6229 202a 2a20 6578 7029 202f 2032 200a  b) ** exp) / 2 .
-00013530: 2020 2020 2020 2020 656c 6966 2065 6461          elif eda
-00013540: 7461 2e6d 616a 6f72 6974 795f 7072 6566  ta.majority_pref
-00013550: 6572 7328 622c 2061 2920 616e 6420 2861  ers(b, a) and (a
-00013560: 2c62 2920 6e6f 7420 696e 2072 656c 2061  ,b) not in rel a
-00013570: 6e64 2028 622c 6129 206e 6f74 2069 6e20  nd (b,a) not in 
-00013580: 7265 6c3a 200a 2020 2020 2020 2020 2020  rel: .          
-00013590: 2020 7065 6e61 6c74 7920 2b3d 2028 6564    penalty += (ed
-000135a0: 6174 612e 6d61 7267 696e 2862 2c20 6129  ata.margin(b, a)
-000135b0: 202a 2a20 6578 7029 2020 2f20 320a 2020   ** exp)  / 2.  
-000135c0: 2020 7265 7475 726e 2070 656e 616c 7479    return penalty
-000135d0: 0a                                       .
+00010610: 2020 2073 6f72 7465 645f 6d61 7463 6865     sorted_matche
+00010620: 7320 3d20 736f 7274 6564 5f6d 6174 6368  s = sorted_match
+00010630: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00010640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010650: 2020 2020 2020 2020 6d65 6d5f 7376 5f77          mem_sv_w
+00010660: 696e 6e65 7273 203d 207b 7d29 5b30 5d29  inners = {})[0])
+00010670: 0a0a 6465 6620 5f73 7461 626c 655f 766f  ..def _stable_vo
+00010680: 7469 6e67 5f62 6173 6963 280a 2020 2020  ting_basic(.    
+00010690: 2020 2020 6564 6174 612c 200a 2020 2020      edata, .    
+000106a0: 2020 2020 6375 7272 5f63 616e 6473 203d      curr_cands =
+000106b0: 204e 6f6e 652c 200a 2020 2020 2020 2020   None, .        
+000106c0: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+000106d0: 6e20 3d20 4e6f 6e65 293a 200a 2020 2020  n = None): .    
+000106e0: 2222 2249 6d70 6c65 6d65 6e74 6174 696f  """Implementatio
+000106f0: 6e20 6f66 2020 5374 6162 6c65 2056 6f74  n of  Stable Vot
+00010700: 696e 6720 6672 6f6d 2068 7474 7073 3a2f  ing from https:/
+00010710: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00010720: 3130 382e 3030 3534 322e 200a 0a20 2020  108.00542. ..   
+00010730: 2041 7267 733a 0a20 2020 2020 2020 2065   Args:.        e
+00010740: 6461 7461 2028 5072 6f66 696c 652c 2050  data (Profile, P
+00010750: 726f 6669 6c65 5769 7468 5469 6573 2c20  rofileWithTies, 
+00010760: 4d61 7267 696e 4772 6170 6829 3a20 416e  MarginGraph): An
+00010770: 7920 656c 6563 7469 6f6e 2064 6174 6120  y election data 
+00010780: 7468 6174 2068 6173 2061 2060 6d61 7267  that has a `marg
+00010790: 696e 6020 6d65 7468 6f64 2e20 0a20 2020  in` method. .   
+000107a0: 2020 2020 2063 7572 725f 6361 6e64 7320       curr_cands 
+000107b0: 284c 6973 745b 696e 745d 2c20 6f70 7469  (List[int], opti
+000107c0: 6f6e 616c 293a 2049 6620 7365 742c 2074  onal): If set, t
+000107d0: 6865 6e20 6669 6e64 2074 6865 2077 696e  hen find the win
+000107e0: 6e65 7273 2066 6f72 2074 6865 2070 726f  ners for the pro
+000107f0: 6669 6c65 2072 6573 7472 6963 7465 6420  file restricted 
+00010800: 746f 2074 6865 2063 616e 6469 6461 7465  to the candidate
+00010810: 7320 696e 2060 6063 7572 725f 6361 6e64  s in ``curr_cand
+00010820: 7360 600a 2020 2020 2020 2020 7374 7265  s``.        stre
+00010830: 6e67 7468 5f66 756e 6374 696f 6e20 2866  ngth_function (f
+00010840: 756e 6374 696f 6e2c 206f 7074 696f 6e61  unction, optiona
+00010850: 6c29 3a20 5468 6520 7374 7265 6e67 7468  l): The strength
+00010860: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
+00010870: 7573 6564 2074 6f20 6361 6c63 756c 6174  used to calculat
+00010880: 6520 7468 6520 7374 7265 6e67 7468 206f  e the strength o
+00010890: 6620 6120 7061 7468 2e20 2020 5468 6520  f a path.   The 
+000108a0: 6465 6661 756c 7420 6973 2074 6865 206d  default is the m
+000108b0: 6172 6769 6e20 6d65 7468 6f64 206f 6620  argin method of 
+000108c0: 6060 6564 6174 6160 602e 2020 2054 6869  ``edata``.   Thi
+000108d0: 7320 6f6e 6c79 206d 6174 7465 7273 2077  s only matters w
+000108e0: 6865 6e20 7468 6520 6261 6c6c 6f74 7320  hen the ballots 
+000108f0: 6172 6520 6e6f 7420 6c69 6e65 6172 206f  are not linear o
+00010900: 7264 6572 732e 200a 0a20 2020 2052 6574  rders. ..    Ret
+00010910: 7572 6e73 3a20 0a20 2020 2020 2020 2041  urns: .        A
+00010920: 2073 6f72 7465 6420 6c69 7374 206f 6620   sorted list of 
+00010930: 6361 6e64 6964 6174 6573 2e20 0a0a 2020  candidates. ..  
+00010940: 2020 2222 220a 0a20 2020 2063 7572 725f    """..    curr_
+00010950: 6361 6e64 7320 3d20 6564 6174 612e 6361  cands = edata.ca
+00010960: 6e64 6964 6174 6573 2069 6620 6375 7272  ndidates if curr
+00010970: 5f63 616e 6473 2069 7320 4e6f 6e65 2065  _cands is None e
+00010980: 6c73 6520 6375 7272 5f63 616e 6473 0a20  lse curr_cands. 
+00010990: 2020 2073 7472 656e 6774 685f 6675 6e63     strength_func
+000109a0: 7469 6f6e 203d 2065 6461 7461 2e6d 6172  tion = edata.mar
+000109b0: 6769 6e20 6966 2073 7472 656e 6774 685f  gin if strength_
+000109c0: 6675 6e63 7469 6f6e 2069 7320 4e6f 6e65  function is None
+000109d0: 2065 6c73 6520 7374 7265 6e67 7468 5f66   else strength_f
+000109e0: 756e 6374 696f 6e20 200a 0a20 2020 206d  unction  ..    m
+000109f0: 6174 6368 6573 203d 205b 2861 2c20 622c  atches = [(a, b,
+00010a00: 2073 7472 656e 6774 685f 6675 6e63 7469   strength_functi
+00010a10: 6f6e 2861 2c20 6229 2920 666f 7220 6120  on(a, b)) for a 
+00010a20: 696e 2063 7572 725f 6361 6e64 7320 666f  in curr_cands fo
+00010a30: 7220 6220 696e 2063 7572 725f 6361 6e64  r b in curr_cand
+00010a40: 7320 6966 2061 2021 3d20 625d 0a20 2020  s if a != b].   
+00010a50: 2073 6f72 7465 645f 6d61 7463 6865 7320   sorted_matches 
+00010a60: 3d20 736f 7274 6564 286d 6174 6368 6573  = sorted(matches
+00010a70: 2c20 7265 7665 7273 653d 5472 7565 2c20  , reverse=True, 
+00010a80: 6b65 793d 6c61 6d62 6461 206d 5f77 5f77  key=lambda m_w_w
+00010a90: 6569 6768 743a 206d 5f77 5f77 6569 6768  eight: m_w_weigh
+00010aa0: 745b 325d 290a 0a20 2020 2072 6574 7572  t[2])..    retur
+00010ab0: 6e20 736f 7274 6564 285f 7374 6162 6c65  n sorted(_stable
+00010ac0: 5f76 6f74 696e 6728 6564 6174 612c 200a  _voting(edata, .
+00010ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010af0: 2063 7572 725f 6361 6e64 7320 3d20 6375   curr_cands = cu
+00010b00: 7272 5f63 616e 6473 2c20 0a20 2020 2020  rr_cands, .     
+00010b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b20: 2020 2020 2020 2020 2020 2020 7374 7265              stre
+00010b30: 6e67 7468 5f66 756e 6374 696f 6e20 3d20  ngth_function = 
+00010b40: 7374 7265 6e67 7468 5f66 756e 6374 696f  strength_functio
+00010b50: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00010b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010b70: 2020 2020 736f 7274 6564 5f6d 6174 6368      sorted_match
+00010b80: 6573 203d 2073 6f72 7465 645f 6d61 7463  es = sorted_matc
+00010b90: 6865 732c 0a20 2020 2020 2020 2020 2020  hes,.           
+00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010bb0: 2020 2020 2020 6d65 6d5f 7376 5f77 696e        mem_sv_win
+00010bc0: 6e65 7273 203d 207b 7d29 5b30 5d29 0a0a  ners = {})[0])..
+00010bd0: 4076 6d28 6e61 6d65 203d 2022 5374 6162  @vm(name = "Stab
+00010be0: 6c65 2056 6f74 696e 6722 2c0a 2020 2020  le Voting",.    
+00010bf0: 696e 7075 745f 7479 7065 7320 3d20 5b45  input_types = [E
+00010c00: 6c65 6374 696f 6e54 7970 6573 2e50 524f  lectionTypes.PRO
+00010c10: 4649 4c45 2c20 456c 6563 7469 6f6e 5479  FILE, ElectionTy
+00010c20: 7065 732e 5052 4f46 494c 455f 5749 5448  pes.PROFILE_WITH
+00010c30: 5f54 4945 532c 2045 6c65 6374 696f 6e54  _TIES, ElectionT
+00010c40: 7970 6573 2e4d 4152 4749 4e5f 4752 4150  ypes.MARGIN_GRAP
+00010c50: 485d 290a 6465 6620 7374 6162 6c65 5f76  H]).def stable_v
+00010c60: 6f74 696e 6728 0a20 2020 2065 6461 7461  oting(.    edata
+00010c70: 2c20 0a20 2020 2063 7572 725f 6361 6e64  , .    curr_cand
+00010c80: 733d 4e6f 6e65 2c20 0a20 2020 2073 7472  s=None, .    str
+00010c90: 656e 6774 685f 6675 6e63 7469 6f6e 3d4e  ength_function=N
+00010ca0: 6f6e 652c 200a 2020 2020 616c 676f 7269  one, .    algori
+00010cb0: 7468 6d3d 2762 6173 6963 2729 3a20 0a20  thm='basic'): . 
+00010cc0: 2020 2022 2222 496d 706c 656d 656e 7461     """Implementa
+00010cd0: 7469 6f6e 206f 6620 2053 7461 626c 6520  tion of  Stable 
+00010ce0: 566f 7469 6e67 2066 726f 6d20 6874 7470  Voting from http
+00010cf0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00010d00: 732f 3231 3038 2e30 3035 3432 2e20 0a0a  s/2108.00542. ..
+00010d10: 2020 2020 5374 6162 6c65 2056 6f74 696e      Stable Votin
+00010d20: 6720 6973 2061 2072 6563 7572 7369 7665  g is a recursive
+00010d30: 2076 6f74 696e 6720 6d65 7468 6f64 2064   voting method d
+00010d40: 6566 696e 6564 2061 7320 666f 6c6c 6f77  efined as follow
+00010d50: 733a 200a 0a20 2020 2031 2e20 2049 6620  s: ..    1.  If 
+00010d60: 7468 6572 6520 6973 206f 6e6c 7920 6f6e  there is only on
+00010d70: 6520 6361 6e64 6964 6174 6520 696e 2074  e candidate in t
+00010d80: 6865 2070 726f 6669 6c65 2c20 7468 656e  he profile, then
+00010d90: 2074 6861 7420 6361 6e64 6964 6174 6520   that candidate 
+00010da0: 6973 2074 6865 2077 696e 6e65 722e 200a  is the winner. .
+00010db0: 2020 2020 322e 204f 7264 6572 2074 6865      2. Order the
+00010dc0: 2070 6169 7273 203a 6d61 7468 3a60 2861   pairs :math:`(a
+00010dd0: 2c62 2960 206f 6620 6361 6e64 6964 6174  ,b)` of candidat
+00010de0: 6573 2066 726f 6d20 6c61 7267 6573 7420  es from largest 
+00010df0: 746f 2073 6d61 6c6c 6573 7420 7661 6c75  to smallest valu
+00010e00: 6520 6f66 2074 6865 206d 6172 6769 6e20  e of the margin 
+00010e10: 6f66 203a 6d61 7468 3a60 6160 206f 7665  of :math:`a` ove
+00010e20: 7220 3a6d 6174 683a 6062 6020 7375 6368  r :math:`b` such
+00010e30: 2074 6861 7420 3a6d 6174 683a 6061 6020   that :math:`a` 
+00010e40: 6973 2075 6e64 6566 6561 7465 6420 6163  is undefeated ac
+00010e50: 636f 7264 696e 6720 746f 2053 706c 6974  cording to Split
+00010e60: 2043 7963 6c65 2c20 616e 6420 6465 636c   Cycle, and decl
+00010e70: 6172 6520 6173 2053 7461 626c 6520 566f  are as Stable Vo
+00010e80: 7469 6e67 2077 696e 6e65 7273 2074 6865  ting winners the
+00010e90: 2063 616e 6469 6461 7465 2873 2920 3a6d   candidate(s) :m
+00010ea0: 6174 683a 6061 6020 6672 6f6d 2074 6865  ath:`a` from the
+00010eb0: 2065 6172 6c69 6573 7420 7061 6972 2873   earliest pair(s
+00010ec0: 2920 3a6d 6174 683a 6028 612c 6229 6020  ) :math:`(a,b)` 
+00010ed0: 7375 6368 2074 6861 7420 3a6d 6174 683a  such that :math:
+00010ee0: 6061 6020 6973 2061 2053 696d 706c 6520  `a` is a Simple 
+00010ef0: 5374 6162 6c65 2056 6f74 696e 6720 7769  Stable Voting wi
+00010f00: 6e6e 6572 2069 6e20 7468 6520 656c 6563  nner in the elec
+00010f10: 7469 6f6e 2077 6974 686f 7574 203a 6d61  tion without :ma
+00010f20: 7468 3a60 6260 2e20 0a0a 2020 2020 4172  th:`b`. ..    Ar
+00010f30: 6773 3a0a 2020 2020 2020 2020 6564 6174  gs:.        edat
+00010f40: 6120 2850 726f 6669 6c65 2c20 5072 6f66  a (Profile, Prof
+00010f50: 696c 6557 6974 6854 6965 732c 204d 6172  ileWithTies, Mar
+00010f60: 6769 6e47 7261 7068 293a 2041 6e79 2065  ginGraph): Any e
+00010f70: 6c65 6374 696f 6e20 6461 7461 2074 6861  lection data tha
+00010f80: 7420 6861 7320 6120 606d 6172 6769 6e60  t has a `margin`
+00010f90: 206d 6574 686f 642e 200a 2020 2020 2020   method. .      
+00010fa0: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00010fb0: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00010fc0: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00010fd0: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00010fe0: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+00010ff0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+00011000: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+00011010: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+00011020: 0a20 2020 2020 2020 2073 7472 656e 6774  .        strengt
+00011030: 685f 6675 6e63 7469 6f6e 2028 6675 6e63  h_function (func
+00011040: 7469 6f6e 2c20 6f70 7469 6f6e 616c 293a  tion, optional):
+00011050: 2054 6865 2073 7472 656e 6774 6820 6675   The strength fu
+00011060: 6e63 7469 6f6e 2074 6f20 6265 2075 7365  nction to be use
+00011070: 6420 746f 2063 616c 6375 6c61 7465 2074  d to calculate t
+00011080: 6865 2073 7472 656e 6774 6820 6f66 2061  he strength of a
+00011090: 2070 6174 682e 2020 2054 6865 2064 6566   path.   The def
+000110a0: 6175 6c74 2069 7320 7468 6520 6d61 7267  ault is the marg
+000110b0: 696e 206d 6574 686f 6420 6f66 2060 6065  in method of ``e
+000110c0: 6461 7461 6060 2e20 2020 5468 6973 206f  data``.   This o
+000110d0: 6e6c 7920 6d61 7474 6572 7320 7768 656e  nly matters when
+000110e0: 2074 6865 2062 616c 6c6f 7473 2061 7265   the ballots are
+000110f0: 206e 6f74 206c 696e 6561 7220 6f72 6465   not linear orde
+00011100: 7273 2e20 0a0a 2020 2020 5265 7475 726e  rs. ..    Return
+00011110: 733a 200a 2020 2020 2020 2020 4120 736f  s: .        A so
+00011120: 7274 6564 206c 6973 7420 6f66 2063 616e  rted list of can
+00011130: 6469 6461 7465 732e 200a 0a20 2020 202e  didates. ..    .
+00011140: 2e20 7365 6561 6c73 6f3a 3a0a 0a20 2020  . seealso::..   
+00011150: 2020 2020 203a 6d65 7468 3a60 7072 6566       :meth:`pref
+00011160: 5f76 6f74 696e 672e 6d61 7267 696e 5f62  _voting.margin_b
+00011170: 6173 6564 5f6d 6574 686f 6473 2e73 696d  ased_methods.sim
+00011180: 706c 655f 7374 6162 6c65 5f76 6f74 696e  ple_stable_votin
+00011190: 6760 0a0a 0a20 2020 203a 4578 616d 706c  g`...    :Exampl
+000111a0: 653a 200a 0a20 2020 202e 2e20 6578 6563  e: ..    .. exec
+000111b0: 5f63 6f64 653a 3a0a 0a20 2020 2020 2020  _code::..       
+000111c0: 2066 726f 6d20 7072 6566 5f76 6f74 696e   from pref_votin
+000111d0: 672e 7765 6967 6874 6564 5f6d 616a 6f72  g.weighted_major
+000111e0: 6974 795f 6772 6170 6873 2069 6d70 6f72  ity_graphs impor
+000111f0: 7420 4d61 7267 696e 4772 6170 680a 2020  t MarginGraph.  
+00011200: 2020 2020 2020 6672 6f6d 2070 7265 665f        from pref_
+00011210: 766f 7469 6e67 2e6d 6172 6769 6e5f 6261  voting.margin_ba
+00011220: 7365 645f 6d65 7468 6f64 7320 696d 706f  sed_methods impo
+00011230: 7274 2073 7461 626c 655f 766f 7469 6e67  rt stable_voting
+00011240: 0a0a 2020 2020 2020 2020 6d67 203d 204d  ..        mg = M
+00011250: 6172 6769 6e47 7261 7068 285b 302c 2031  arginGraph([0, 1
+00011260: 2c20 322c 2033 5d2c 205b 2830 2c20 332c  , 2, 3], [(0, 3,
+00011270: 2038 292c 2028 312c 2030 2c20 3130 292c   8), (1, 0, 10),
+00011280: 2028 322c 2030 2c20 3429 2c20 2832 2c20   (2, 0, 4), (2, 
+00011290: 312c 2038 292c 2028 332c 2031 2c20 3829  1, 8), (3, 1, 8)
+000112a0: 5d29 0a0a 2020 2020 2020 2020 7374 6162  ])..        stab
+000112b0: 6c65 5f76 6f74 696e 672e 6469 7370 6c61  le_voting.displa
+000112c0: 7928 6d67 290a 2020 2020 2020 2020 7374  y(mg).        st
+000112d0: 6162 6c65 5f76 6f74 696e 672e 6469 7370  able_voting.disp
+000112e0: 6c61 7928 6d67 2c20 616c 676f 7269 7468  lay(mg, algorith
+000112f0: 6d3d 2762 6173 6963 2729 0a20 2020 2020  m='basic').     
+00011300: 2020 2073 7461 626c 655f 766f 7469 6e67     stable_voting
+00011310: 2e64 6973 706c 6179 286d 672c 2061 6c67  .display(mg, alg
+00011320: 6f72 6974 686d 3d27 7769 7468 5f63 6f6e  orithm='with_con
+00011330: 646f 7263 6574 5f63 6865 636b 2729 0a0a  dorcet_check')..
+00011340: 2020 2020 2222 220a 0a20 2020 2069 6620      """..    if 
+00011350: 616c 676f 7269 7468 6d20 3d3d 2027 6261  algorithm == 'ba
+00011360: 7369 6327 3a20 0a20 2020 2020 2020 2072  sic': .        r
+00011370: 6574 7572 6e20 5f73 7461 626c 655f 766f  eturn _stable_vo
+00011380: 7469 6e67 5f62 6173 6963 2865 6461 7461  ting_basic(edata
+00011390: 2c20 6375 7272 5f63 616e 6473 203d 2063  , curr_cands = c
+000113a0: 7572 725f 6361 6e64 732c 2073 7472 656e  urr_cands, stren
+000113b0: 6774 685f 6675 6e63 7469 6f6e 203d 2073  gth_function = s
+000113c0: 7472 656e 6774 685f 6675 6e63 7469 6f6e  trength_function
+000113d0: 290a 2020 2020 656c 6966 2061 6c67 6f72  ).    elif algor
+000113e0: 6974 686d 203d 3d20 2777 6974 685f 636f  ithm == 'with_co
+000113f0: 6e64 6f72 6365 745f 6368 6563 6b27 3a0a  ndorcet_check':.
+00011400: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00011410: 7374 6162 6c65 5f76 6f74 696e 675f 7769  stable_voting_wi
+00011420: 7468 5f63 6f6e 646f 7263 6574 5f63 6865  th_condorcet_che
+00011430: 636b 2865 6461 7461 2c20 6375 7272 5f63  ck(edata, curr_c
+00011440: 616e 6473 203d 2063 7572 725f 6361 6e64  ands = curr_cand
+00011450: 732c 2073 7472 656e 6774 685f 6675 6e63  s, strength_func
+00011460: 7469 6f6e 203d 2073 7472 656e 6774 685f  tion = strength_
+00011470: 6675 6e63 7469 6f6e 290a 2020 2020 656c  function).    el
+00011480: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
+00011490: 6520 5661 6c75 6545 7272 6f72 2822 496e  e ValueError("In
+000114a0: 7661 6c69 6420 616c 676f 7269 7468 6d20  valid algorithm 
+000114b0: 7370 6563 6966 6965 642e 2229 0a20 2020  specified.").   
+000114c0: 200a 0a40 766d 286e 616d 653d 2245 7373   ..@vm(name="Ess
+000114d0: 656e 7469 616c 2053 6574 222c 0a20 2020  ential Set",.   
+000114e0: 2069 6e70 7574 5f74 7970 6573 3d5b 456c   input_types=[El
+000114f0: 6563 7469 6f6e 5479 7065 732e 5052 4f46  ectionTypes.PROF
+00011500: 494c 452c 2045 6c65 6374 696f 6e54 7970  ILE, ElectionTyp
+00011510: 6573 2e50 524f 4649 4c45 5f57 4954 485f  es.PROFILE_WITH_
+00011520: 5449 4553 2c20 456c 6563 7469 6f6e 5479  TIES, ElectionTy
+00011530: 7065 732e 4d41 5247 494e 5f47 5241 5048  pes.MARGIN_GRAPH
+00011540: 5d29 0a64 6566 2065 7373 656e 7469 616c  ]).def essential
+00011550: 2865 6461 7461 2c20 6375 7272 5f63 616e  (edata, curr_can
+00011560: 6473 203d 204e 6f6e 652c 2074 6872 6573  ds = None, thres
+00011570: 686f 6c64 203d 2030 2e30 3030 3030 3031  hold = 0.0000001
+00011580: 293a 200a 2020 2020 2222 2254 6865 2045  ): .    """The E
+00011590: 7373 656e 7469 616c 2053 6574 2069 7320  ssential Set is 
+000115a0: 7468 6520 7375 7070 6f72 7420 6f66 2074  the support of t
+000115b0: 6865 2028 6368 6f73 656e 2920 4332 206d  he (chosen) C2 m
+000115c0: 6178 696d 616c 206c 6f74 7465 7279 2e0a  aximal lottery..
+000115d0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+000115e0: 2020 2065 6461 7461 2028 5072 6f66 696c     edata (Profil
+000115f0: 652c 2050 726f 6669 6c65 5769 7468 5469  e, ProfileWithTi
+00011600: 6573 2c20 4d61 7267 696e 4772 6170 6829  es, MarginGraph)
+00011610: 3a20 416e 7920 656c 6563 7469 6f6e 2064  : Any election d
+00011620: 6174 6120 7468 6174 2068 6173 2061 2060  ata that has a `
+00011630: 6d61 7267 696e 5f6d 6174 7269 7860 2061  margin_matrix` a
+00011640: 7474 7269 6275 7465 2e0a 2020 2020 2020  ttribute..      
+00011650: 2020 6375 7272 5f63 616e 6473 2028 4c69    curr_cands (Li
+00011660: 7374 5b69 6e74 5d2c 206f 7074 696f 6e61  st[int], optiona
+00011670: 6c29 3a20 4966 2073 6574 2c20 7468 656e  l): If set, then
+00011680: 2066 696e 6420 7468 6520 7769 6e6e 6572   find the winner
+00011690: 7320 666f 7220 7468 6520 7072 6f66 696c  s for the profil
+000116a0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+000116b0: 7468 6520 6361 6e64 6964 6174 6573 2069  the candidates i
+000116c0: 6e20 6060 6375 7272 5f63 616e 6473 6060  n ``curr_cands``
+000116d0: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
+000116e0: 2020 2020 2020 2041 2073 6f72 7465 6420         A sorted 
+000116f0: 6c69 7374 206f 6620 6361 6e64 6964 6174  list of candidat
+00011700: 6573 2e0a 0a20 2020 2022 2222 0a20 2020  es...    """.   
+00011710: 206d 6c20 3d20 6d61 7869 6d61 6c5f 6c6f   ml = maximal_lo
+00011720: 7474 6572 7928 6564 6174 612c 2063 7572  ttery(edata, cur
+00011730: 725f 6361 6e64 733d 6375 7272 5f63 616e  r_cands=curr_can
+00011740: 6473 290a 0a20 2020 2072 6574 7572 6e20  ds)..    return 
+00011750: 736f 7274 6564 285b 6320 666f 7220 6320  sorted([c for c 
+00011760: 696e 206d 6c2e 6b65 7973 2829 2069 6620  in ml.keys() if 
+00011770: 6d6c 5b63 5d20 3e20 7468 7265 7368 6f6c  ml[c] > threshol
+00011780: 645d 290a 0a40 766d 286e 616d 653d 2257  d])..@vm(name="W
+00011790: 6569 6768 7465 6420 436f 7665 7269 6e67  eighted Covering
+000117a0: 222c 0a20 2020 2069 6e70 7574 5f74 7970  ",.    input_typ
+000117b0: 6573 3d5b 456c 6563 7469 6f6e 5479 7065  es=[ElectionType
+000117c0: 732e 5052 4f46 494c 452c 2045 6c65 6374  s.PROFILE, Elect
+000117d0: 696f 6e54 7970 6573 2e50 524f 4649 4c45  ionTypes.PROFILE
+000117e0: 5f57 4954 485f 5449 4553 2c20 456c 6563  _WITH_TIES, Elec
+000117f0: 7469 6f6e 5479 7065 732e 4d41 5247 494e  tionTypes.MARGIN
+00011800: 5f47 5241 5048 5d29 0a64 6566 2077 6569  _GRAPH]).def wei
+00011810: 6768 7465 645f 636f 7665 7269 6e67 2865  ghted_covering(e
+00011820: 6461 7461 2c20 6375 7272 5f63 616e 6473  data, curr_cands
+00011830: 3d4e 6f6e 6529 3a20 0a20 2020 2022 2222  =None): .    """
+00011840: 4163 636f 7264 696e 6720 746f 2057 6569  According to Wei
+00011850: 6768 7465 6420 436f 7665 7269 6e67 2c20  ghted Covering, 
+00011860: 7820 6465 6665 6174 7320 7920 6966 2074  x defeats y if t
+00011870: 6865 206d 6172 6769 6e20 6f66 2078 206f  he margin of x o
+00011880: 7665 7220 7920 6973 2070 6f73 6974 6976  ver y is positiv
+00011890: 6520 616e 6420 666f 7220 6576 6572 7920  e and for every 
+000118a0: 6f74 6865 7220 7a2c 2074 6865 206d 6172  other z, the mar
+000118b0: 6769 6e20 6f66 2078 206f 7665 7220 7a20  gin of x over z 
+000118c0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
+000118d0: 6f72 2065 7175 616c 2074 6f20 7468 6520  or equal to the 
+000118e0: 6d61 7267 696e 206f 6620 7920 6f76 6572  margin of y over
+000118f0: 207a 2e20 0a0a 2020 2020 4172 6773 3a0a   z. ..    Args:.
+00011900: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00011910: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00011920: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00011930: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00011940: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00011950: 7320 6120 606d 6172 6769 6e60 206d 6574  s a `margin` met
+00011960: 686f 642e 0a20 2020 2020 2020 2063 7572  hod..        cur
+00011970: 725f 6361 6e64 7320 284c 6973 745b 696e  r_cands (List[in
+00011980: 745d 2c20 6f70 7469 6f6e 616c 293a 2049  t], optional): I
+00011990: 6620 7365 742c 2074 6865 6e20 6669 6e64  f set, then find
+000119a0: 2074 6865 2077 696e 6e65 7273 2066 6f72   the winners for
+000119b0: 2074 6865 2070 726f 6669 6c65 2072 6573   the profile res
+000119c0: 7472 6963 7465 6420 746f 2074 6865 2063  tricted to the c
+000119d0: 616e 6469 6461 7465 7320 696e 2060 6063  andidates in ``c
+000119e0: 7572 725f 6361 6e64 7360 600a 0a20 2020  urr_cands``..   
+000119f0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00011a00: 2020 4120 736f 7274 6564 206c 6973 7420    A sorted list 
+00011a10: 6f66 2063 616e 6469 6461 7465 732e 0a0a  of candidates...
+00011a20: 2020 2020 2e2e 206e 6f74 653a 3a0a 2020      .. note::.  
+00011a30: 2020 2020 2020 5365 652c 2065 2e67 2e2c        See, e.g.,
+00011a40: 2042 6861 736b 6172 2044 7574 7461 2061   Bhaskar Dutta a
+00011a50: 6e64 204a 6561 6e2d 4672 616e 636f 6973  nd Jean-Francois
+00011a60: 204c 6173 6c69 6572 2c20 2243 6f6d 7061   Laslier, "Compa
+00011a70: 7269 736f 6e20 6675 6e63 7469 6f6e 7320  rison functions 
+00011a80: 616e 6420 6368 6f69 6365 2063 6f72 7265  and choice corre
+00011a90: 7370 6f6e 6465 6e63 6573 2c22 2053 6f63  spondences," Soc
+00011aa0: 6961 6c20 4368 6f69 6365 2061 6e64 2057  ial Choice and W
+00011ab0: 656c 6661 7265 2c20 3136 3a35 3133 e280  elfare, 16:513..
+00011ac0: 9335 3332 2c20 3139 3939 2c20 646f 693a  .532, 1999, doi:
+00011ad0: 3130 2e31 3030 372f 7330 3033 3535 3030  10.1007/s0035500
+00011ae0: 3530 3135 382c 2061 6e64 2052 6175 cc81  50158, and Rau..
+00011af0: 6c20 5065 cc81 7265 7a2d 4665 726e 61cc  l Pe..rez-Ferna.
+00011b00: 816e 6465 7a20 616e 6420 4265 726e 6172  .ndez and Bernar
+00011b10: 6420 4465 2042 6165 7473 2c20 2254 6865  d De Baets, "The
+00011b20: 2073 7570 6572 636f 7665 7269 6e67 2072   supercovering r
+00011b30: 656c 6174 696f 6e2c 2074 6865 2070 6169  elation, the pai
+00011b40: 7277 6973 6520 7769 6e6e 6572 2c20 616e  rwise winner, an
+00011b50: 6420 6d6f 7265 206d 6973 7369 6e67 206c  d more missing l
+00011b60: 696e 6b73 2062 6574 7765 656e 2042 6f72  inks between Bor
+00011b70: 6461 2061 6e64 2043 6f6e 646f 7263 6574  da and Condorcet
+00011b80: 2c22 2053 6f63 6961 6c20 4368 6f69 6365  ," Social Choice
+00011b90: 2061 6e64 2057 656c 6661 7265 2c20 3530   and Welfare, 50
+00011ba0: 3a33 3239 e280 9333 3532 2c20 3230 3138  :329...352, 2018
+00011bb0: 2c20 646f 693a 3130 2e31 3030 372f 7330  , doi:10.1007/s0
+00011bc0: 3033 3535 2d30 3137 2d31 3038 362d 302e  0355-017-1086-0.
+00011bd0: 0a20 2020 2022 2222 0a0a 2020 2020 6361  .    """..    ca
+00011be0: 6e64 6964 6174 6573 203d 2065 6461 7461  ndidates = edata
+00011bf0: 2e63 616e 6469 6461 7465 7320 6966 2063  .candidates if c
+00011c00: 7572 725f 6361 6e64 7320 6973 204e 6f6e  urr_cands is Non
+00011c10: 6520 656c 7365 2063 7572 725f 6361 6e64  e else curr_cand
+00011c20: 730a 0a20 2020 2075 635f 7365 7420 3d20  s..    uc_set = 
+00011c30: 6c69 7374 2829 0a0a 2020 2020 666f 7220  list()..    for 
+00011c40: 7920 696e 2063 616e 6469 6461 7465 733a  y in candidates:
+00011c50: 0a20 2020 2020 2020 2069 735f 696e 5f75  .        is_in_u
+00011c60: 6373 203d 2054 7275 650a 2020 2020 2020  cs = True.      
+00011c70: 2020 666f 7220 7820 696e 2065 6461 7461    for x in edata
+00011c80: 2e64 6f6d 696e 6174 6f72 7328 792c 2063  .dominators(y, c
+00011c90: 7572 725f 6361 6e64 7320 3d20 6375 7272  urr_cands = curr
+00011ca0: 5f63 616e 6473 293a 0a20 2020 2020 2020  _cands):.       
+00011cb0: 2020 2020 2023 2063 6865 636b 2069 6620       # check if 
+00011cc0: 7920 636f 7665 7273 2078 2c20 692e 652e  y covers x, i.e.
+00011cd0: 2c20 666f 7220 6576 6572 7920 7a2c 206d  , for every z, m
+00011ce0: 6172 6769 6e28 782c 207a 2920 3e3d 206d  argin(x, z) >= m
+00011cf0: 6172 6769 6e28 792c 207a 290a 2020 2020  argin(y, z).    
+00011d00: 2020 2020 2020 2020 636f 7665 7273 203d          covers =
+00011d10: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00011d20: 2020 666f 7220 7a20 696e 2063 616e 6469    for z in candi
+00011d30: 6461 7465 733a 0a20 2020 2020 2020 2020  dates:.         
+00011d40: 2020 2020 2020 2069 6620 6564 6174 612e         if edata.
+00011d50: 6d61 7267 696e 2878 2c20 7a29 203c 2065  margin(x, z) < e
+00011d60: 6461 7461 2e6d 6172 6769 6e28 792c 207a  data.margin(y, z
+00011d70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00011d80: 2020 2020 2020 2063 6f76 6572 7320 3d20         covers = 
+00011d90: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00011da0: 2020 2020 2020 2020 2020 6272 6561 6b0a            break.
+00011db0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00011dc0: 2020 2020 2020 2069 6620 636f 7665 7273         if covers
+00011dd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011de0: 2020 6973 5f69 6e5f 7563 7320 3d20 4661    is_in_ucs = Fa
+00011df0: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00011e00: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00011e10: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00011e20: 2020 2069 6620 6973 5f69 6e5f 7563 733a     if is_in_ucs:
+00011e30: 0a20 2020 2020 2020 2020 2020 2075 635f  .            uc_
+00011e40: 7365 742e 6170 7065 6e64 2879 290a 0a20  set.append(y).. 
+00011e50: 2020 2072 6574 7572 6e20 736f 7274 6564     return sorted
+00011e60: 2875 635f 7365 7429 0a0a 4076 6d28 6e61  (uc_set)..@vm(na
+00011e70: 6d65 203d 2022 4c6f 7373 2d54 7269 6d6d  me = "Loss-Trimm
+00011e80: 6572 2056 6f74 696e 6722 2c0a 2020 2020  er Voting",.    
+00011e90: 696e 7075 745f 7479 7065 7320 3d20 5b45  input_types = [E
+00011ea0: 6c65 6374 696f 6e54 7970 6573 2e50 524f  lectionTypes.PRO
+00011eb0: 4649 4c45 2c20 456c 6563 7469 6f6e 5479  FILE, ElectionTy
+00011ec0: 7065 732e 5052 4f46 494c 455f 5749 5448  pes.PROFILE_WITH
+00011ed0: 5f54 4945 532c 2045 6c65 6374 696f 6e54  _TIES, ElectionT
+00011ee0: 7970 6573 2e4d 4152 4749 4e5f 4752 4150  ypes.MARGIN_GRAP
+00011ef0: 485d 290a 6465 6620 6c6f 7373 5f74 7269  H]).def loss_tri
+00011f00: 6d6d 6572 2865 6461 7461 2c20 6375 7272  mmer(edata, curr
+00011f10: 5f63 616e 6473 203d 204e 6f6e 6529 3a0a  _cands = None):.
+00011f20: 2020 2020 2222 2249 7465 7261 7469 7665      """Iterative
+00011f30: 6c79 2065 6c69 6d69 6e61 7465 2074 6865  ly eliminate the
+00011f40: 2063 616e 6469 6461 7465 2077 6974 6820   candidate with 
+00011f50: 7468 6520 6c61 7267 6573 7420 7375 6d20  the largest sum 
+00011f60: 6f66 206d 6172 6769 6e73 206f 6620 6c6f  of margins of lo
+00011f70: 7373 2075 6e74 696c 2061 2043 6f6e 646f  ss until a Condo
+00011f80: 7263 6574 2077 696e 6e65 7220 6973 2066  rcet winner is f
+00011f90: 6f75 6e64 2e20 496e 2074 6869 7320 7665  ound. In this ve
+00011fa0: 7273 696f 6e20 6f66 2074 6865 206d 6574  rsion of the met
+00011fb0: 686f 642c 2070 6172 616c 6c65 6c2d 756e  hod, parallel-un
+00011fc0: 6976 6572 7365 2074 6965 6272 6561 6b69  iverse tiebreaki
+00011fd0: 6e67 2069 7320 7573 6564 2069 6620 7468  ng is used if th
+00011fe0: 6572 6520 6172 6520 6d75 6c74 6970 6c65  ere are multiple
+00011ff0: 2063 616e 6469 6461 7465 7320 7769 7468   candidates with
+00012000: 2074 6865 206c 6172 6765 7374 2073 756d   the largest sum
+00012010: 206f 6620 6d61 7267 696e 7320 6f66 206c   of margins of l
+00012020: 6f73 732e 0a0a 2020 2020 4172 6773 3a0a  oss...    Args:.
+00012030: 2020 2020 2020 2020 6564 6174 6120 2850          edata (P
+00012040: 726f 6669 6c65 2c20 5072 6f66 696c 6557  rofile, ProfileW
+00012050: 6974 6854 6965 732c 204d 6172 6769 6e47  ithTies, MarginG
+00012060: 7261 7068 293a 2041 6e79 2065 6c65 6374  raph): Any elect
+00012070: 696f 6e20 6461 7461 2074 6861 7420 6861  ion data that ha
+00012080: 7320 6120 6d61 7267 696e 206d 6574 686f  s a margin metho
+00012090: 642e 0a20 2020 2020 2020 2063 7572 725f  d..        curr_
+000120a0: 6361 6e64 7320 284c 6973 745b 696e 745d  cands (List[int]
+000120b0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+000120c0: 7365 742c 2074 6865 6e20 6669 6e64 2074  set, then find t
+000120d0: 6865 2077 696e 6e65 7273 2066 6f72 2074  he winners for t
+000120e0: 6865 2070 726f 6669 6c65 2072 6573 7472  he profile restr
+000120f0: 6963 7465 6420 746f 2074 6865 2063 616e  icted to the can
+00012100: 6469 6461 7465 7320 696e 2060 6063 7572  didates in ``cur
+00012110: 725f 6361 6e64 7360 600a 0a20 2020 2052  r_cands``..    R
+00012120: 6574 7572 6e73 3a20 0a20 2020 2020 2020  eturns: .       
+00012130: 2041 2073 6f72 7465 6420 6c69 7374 206f   A sorted list o
+00012140: 6620 6361 6e64 6964 6174 6573 0a0a 2020  f candidates..  
+00012150: 2020 2e2e 206e 6f74 653a 3a0a 2020 2020    .. note::.    
+00012160: 2020 2020 4d65 7468 6f64 2070 726f 706f      Method propo
+00012170: 7365 6420 6279 2052 6963 6861 7264 2042  sed by Richard B
+00012180: 2e20 4461 726c 696e 6774 6f6e 2069 6e20  . Darlington in 
+00012190: 2254 6865 2043 6173 6520 666f 7220 7468  "The Case for th
+000121a0: 6520 4c6f 7373 2d54 7269 6d6d 6572 2056  e Loss-Trimmer V
+000121b0: 6f74 696e 6720 5379 7374 656d 2e22 0a0a  oting System."..
+000121c0: 2020 2020 2222 220a 0a20 2020 2063 7572      """..    cur
+000121d0: 725f 6361 6e64 7320 3d20 6564 6174 612e  r_cands = edata.
+000121e0: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+000121f0: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00012200: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00012210: 0a0a 2020 2020 7765 616b 5f63 7720 3d20  ..    weak_cw = 
+00012220: 6564 6174 612e 7765 616b 5f63 6f6e 646f  edata.weak_condo
+00012230: 7263 6574 5f77 696e 6e65 7228 6375 7272  rcet_winner(curr
+00012240: 5f63 616e 6473 203d 2063 7572 725f 6361  _cands = curr_ca
+00012250: 6e64 7329 0a20 2020 2023 2049 6620 7468  nds).    # If th
+00012260: 6572 6520 6172 6520 7765 616b 2043 6f6e  ere are weak Con
+00012270: 646f 7263 6574 2077 696e 6e65 7273 2c20  dorcet winners, 
+00012280: 7265 7475 726e 2074 686f 7365 2063 616e  return those can
+00012290: 6469 6461 7465 730a 2020 2020 6966 2065  didates.    if e
+000122a0: 6461 7461 2e77 6561 6b5f 636f 6e64 6f72  data.weak_condor
+000122b0: 6365 745f 7769 6e6e 6572 2863 7572 725f  cet_winner(curr_
+000122c0: 6361 6e64 7320 3d20 6375 7272 5f63 616e  cands = curr_can
+000122d0: 6473 2920 6973 206e 6f74 204e 6f6e 653a  ds) is not None:
+000122e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000122f0: 736f 7274 6564 2877 6561 6b5f 6377 290a  sorted(weak_cw).
+00012300: 2020 2020 0a20 2020 2023 204f 7468 6572      .    # Other
+00012310: 7769 7365 2c20 6361 6c63 756c 6174 6520  wise, calculate 
+00012320: 7468 6520 7375 6d20 6f66 206d 6172 6769  the sum of margi
+00012330: 6e73 206f 6620 6c6f 7373 2066 6f72 2065  ns of loss for e
+00012340: 6163 6820 6361 6e64 6964 6174 650a 2020  ach candidate.  
+00012350: 2020 7375 6d5f 6f66 5f6d 6172 6769 6e73    sum_of_margins
+00012360: 5f6f 665f 6c6f 7373 203d 207b 6361 6e64  _of_loss = {cand
+00012370: 3a20 7375 6d28 5b65 6461 7461 2e6d 6172  : sum([edata.mar
+00012380: 6769 6e28 6f74 6865 725f 6361 6e64 2c20  gin(other_cand, 
+00012390: 6361 6e64 2920 666f 7220 6f74 6865 725f  cand) for other_
+000123a0: 6361 6e64 2069 6e20 6375 7272 5f63 616e  cand in curr_can
+000123b0: 6473 2069 6620 6564 6174 612e 6d61 7267  ds if edata.marg
+000123c0: 696e 286f 7468 6572 5f63 616e 642c 2063  in(other_cand, c
+000123d0: 616e 6429 203e 2030 5d29 2066 6f72 2063  and) > 0]) for c
+000123e0: 616e 6420 696e 2063 7572 725f 6361 6e64  and in curr_cand
+000123f0: 737d 0a0a 2020 2020 2320 4669 6e64 2074  s}..    # Find t
+00012400: 6865 2063 616e 6469 6461 7465 7320 7769  he candidates wi
+00012410: 7468 2074 6865 206c 6172 6765 7374 2073  th the largest s
+00012420: 756d 206f 6620 6d61 7267 696e 7320 6f66  um of margins of
+00012430: 206c 6f73 730a 2020 2020 6d61 785f 7375   loss.    max_su
+00012440: 6d5f 6f66 5f6d 6172 6769 6e73 5f6f 665f  m_of_margins_of_
+00012450: 6c6f 7373 203d 206d 6178 2873 756d 5f6f  loss = max(sum_o
+00012460: 665f 6d61 7267 696e 735f 6f66 5f6c 6f73  f_margins_of_los
+00012470: 732e 7661 6c75 6573 2829 290a 2020 2020  s.values()).    
+00012480: 6269 6767 6573 745f 6c6f 7365 7273 203d  biggest_losers =
+00012490: 205b 6361 6e64 2066 6f72 2063 616e 6420   [cand for cand 
+000124a0: 696e 2063 7572 725f 6361 6e64 7320 6966  in curr_cands if
+000124b0: 2073 756d 5f6f 665f 6d61 7267 696e 735f   sum_of_margins_
+000124c0: 6f66 5f6c 6f73 735b 6361 6e64 5d20 3d3d  of_loss[cand] ==
+000124d0: 206d 6178 5f73 756d 5f6f 665f 6d61 7267   max_sum_of_marg
+000124e0: 696e 735f 6f66 5f6c 6f73 735d 0a0a 2020  ins_of_loss]..  
+000124f0: 2020 7769 6e6e 6572 7320 3d20 5b5d 0a0a    winners = []..
+00012500: 2020 2020 2320 466f 7220 6561 6368 2062      # For each b
+00012510: 6967 6765 7374 206c 6f73 6572 2c20 6361  iggest loser, ca
+00012520: 6c63 756c 6174 6520 7468 6520 7769 6e6e  lculate the winn
+00012530: 6572 7320 6166 7465 7220 7265 6d6f 7669  ers after removi
+00012540: 6e67 2074 6861 7420 6361 6e64 6964 6174  ng that candidat
+00012550: 652e 2054 6865 2075 6e69 6f6e 206f 6620  e. The union of 
+00012560: 7468 6573 6520 7365 7473 2069 7320 7468  these sets is th
+00012570: 6520 7365 7420 6f66 2077 696e 6e65 7273  e set of winners
+00012580: 2e0a 2020 2020 666f 7220 626c 2069 6e20  ..    for bl in 
+00012590: 6269 6767 6573 745f 6c6f 7365 7273 3a0a  biggest_losers:.
+000125a0: 2020 2020 2020 2020 7769 6e6e 6572 735f          winners_
+000125b0: 7769 7468 6f75 745f 626c 203d 206c 6f73  without_bl = los
+000125c0: 735f 7472 696d 6d65 7228 6564 6174 612c  s_trimmer(edata,
+000125d0: 2063 7572 725f 6361 6e64 7320 3d20 5b63   curr_cands = [c
+000125e0: 616e 6420 666f 7220 6361 6e64 2069 6e20  and for cand in 
+000125f0: 6375 7272 5f63 616e 6473 2069 6620 6361  curr_cands if ca
+00012600: 6e64 2021 3d20 626c 5d29 0a20 2020 2020  nd != bl]).     
+00012610: 2020 2077 696e 6e65 7273 202b 3d20 7769     winners += wi
+00012620: 6e6e 6572 735f 7769 7468 6f75 745f 626c  nners_without_bl
+00012630: 0a0a 2020 2020 7265 7475 726e 2073 6f72  ..    return sor
+00012640: 7465 6428 6c69 7374 2873 6574 2877 696e  ted(list(set(win
+00012650: 6e65 7273 2929 290a 0a0a 6465 6620 6469  ners)))...def di
+00012660: 7374 616e 6365 5f74 6f5f 6d61 7267 696e  stance_to_margin
+00012670: 5f67 7261 7068 2865 6461 7461 2c20 7265  _graph(edata, re
+00012680: 6c2c 2065 7870 203d 2031 2c20 6375 7272  l, exp = 1, curr
+00012690: 5f63 616e 6473 203d 204e 6f6e 6529 3a20  _cands = None): 
+000126a0: 0a20 2020 2022 2222 0a20 2020 2043 616c  .    """.    Cal
+000126b0: 6375 6c61 7465 2074 6865 2064 6973 7461  culate the dista
+000126c0: 6e63 6520 6f66 2060 6072 656c 6060 2028  nce of ``rel`` (
+000126d0: 6120 7265 6c61 7469 6f6e 2920 746f 2074  a relation) to t
+000126e0: 6865 206d 616a 6f72 6974 7920 6772 6170  he majority grap
+000126f0: 6820 6f66 2060 6065 6461 7461 6060 2e20  h of ``edata``. 
+00012700: 0a20 2020 2022 2222 0a20 2020 2063 616e  .    """.    can
+00012710: 6469 6461 7465 7320 3d20 6564 6174 612e  didates = edata.
+00012720: 6361 6e64 6964 6174 6573 2069 6620 6375  candidates if cu
+00012730: 7272 5f63 616e 6473 2069 7320 4e6f 6e65  rr_cands is None
+00012740: 2065 6c73 6520 6375 7272 5f63 616e 6473   else curr_cands
+00012750: 0a20 2020 200a 2020 2020 6966 2074 7970  .    .    if typ
+00012760: 6528 6564 6174 6129 203d 3d20 4d61 6a6f  e(edata) == Majo
+00012770: 7269 7479 4772 6170 6820 616e 6420 6578  rityGraph and ex
+00012780: 7020 3d3d 2030 3a0a 2020 2020 2020 2020  p == 0:.        
+00012790: 2320 6966 2065 6461 7461 2069 7320 6120  # if edata is a 
+000127a0: 4d61 6a6f 7269 7479 4772 6170 682c 2077  MajorityGraph, w
+000127b0: 6520 6e65 6564 2074 6f20 6164 6420 6d61  e need to add ma
+000127c0: 7267 696e 7320 666f 7220 7468 6520 666f  rgins for the fo
+000127d0: 6c6c 6f77 696e 6720 636f 6465 2074 6f20  llowing code to 
+000127e0: 776f 726b 2e20 2054 6865 206d 6172 6769  work.  The margi
+000127f0: 6e73 2064 6f20 6e6f 7420 6d61 7474 6572  ns do not matter
+00012800: 2077 6865 6e20 6578 703d 3d30 2e20 2020   when exp==0.   
+00012810: 0a20 2020 2020 2020 2065 6461 7461 203d  .        edata =
+00012820: 204d 6172 6769 6e47 7261 7068 2863 616e   MarginGraph(can
+00012830: 6469 6461 7465 732c 205b 2863 312c 2063  didates, [(c1, c
+00012840: 322c 2031 2920 666f 7220 6331 2c20 6332  2, 1) for c1, c2
+00012850: 2069 6e20 6564 6174 612e 6564 6765 7320   in edata.edges 
+00012860: 6966 2028 6331 2069 6e20 6361 6e64 6964  if (c1 in candid
+00012870: 6174 6573 2061 6e64 2063 3220 696e 2063  ates and c2 in c
+00012880: 616e 6469 6461 7465 7329 5d29 0a20 2020  andidates)]).   
+00012890: 2070 656e 616c 7479 203d 2030 0a20 2020   penalty = 0.   
+000128a0: 2066 6f72 2061 2c62 2069 6e20 636f 6d62   for a,b in comb
+000128b0: 696e 6174 696f 6e73 2863 616e 6469 6461  inations(candida
+000128c0: 7465 732c 2032 293a 200a 2020 2020 2020  tes, 2): .      
+000128d0: 2020 6966 2065 6461 7461 2e6d 616a 6f72    if edata.major
+000128e0: 6974 795f 7072 6566 6572 7328 612c 2062  ity_prefers(a, b
+000128f0: 2920 616e 6420 2862 2c61 2920 696e 2072  ) and (b,a) in r
+00012900: 656c 3a20 0a20 2020 2020 2020 2020 2020  el: .           
+00012910: 2070 656e 616c 7479 202b 3d20 2865 6461   penalty += (eda
+00012920: 7461 2e6d 6172 6769 6e28 612c 2062 2920  ta.margin(a, b) 
+00012930: 2a2a 2065 7870 290a 2020 2020 2020 2020  ** exp).        
+00012940: 656c 6966 2065 6461 7461 2e6d 616a 6f72  elif edata.major
+00012950: 6974 795f 7072 6566 6572 7328 622c 2061  ity_prefers(b, a
+00012960: 2920 616e 6420 2861 2c62 2920 696e 2072  ) and (a,b) in r
+00012970: 656c 3a20 0a20 2020 2020 2020 2020 2020  el: .           
+00012980: 2070 656e 616c 7479 202b 3d20 2865 6461   penalty += (eda
+00012990: 7461 2e6d 6172 6769 6e28 622c 2061 2920  ta.margin(b, a) 
+000129a0: 2a2a 2065 7870 290a 2020 2020 2020 2020  ** exp).        
+000129b0: 656c 6966 2065 6461 7461 2e6d 616a 6f72  elif edata.major
+000129c0: 6974 795f 7072 6566 6572 7328 612c 2062  ity_prefers(a, b
+000129d0: 2920 616e 6420 2861 2c62 2920 6e6f 7420  ) and (a,b) not 
+000129e0: 696e 2072 656c 2061 6e64 2028 622c 6129  in rel and (b,a)
+000129f0: 206e 6f74 2069 6e20 7265 6c3a 200a 2020   not in rel: .  
+00012a00: 2020 2020 2020 2020 2020 7065 6e61 6c74            penalt
+00012a10: 7920 2b3d 2028 6564 6174 612e 6d61 7267  y += (edata.marg
+00012a20: 696e 2861 2c20 6229 202a 2a20 6578 7029  in(a, b) ** exp)
+00012a30: 202f 2032 200a 2020 2020 2020 2020 656c   / 2 .        el
+00012a40: 6966 2065 6461 7461 2e6d 616a 6f72 6974  if edata.majorit
+00012a50: 795f 7072 6566 6572 7328 622c 2061 2920  y_prefers(b, a) 
+00012a60: 616e 6420 2861 2c62 2920 6e6f 7420 696e  and (a,b) not in
+00012a70: 2072 656c 2061 6e64 2028 622c 6129 206e   rel and (b,a) n
+00012a80: 6f74 2069 6e20 7265 6c3a 200a 2020 2020  ot in rel: .    
+00012a90: 2020 2020 2020 2020 7065 6e61 6c74 7920          penalty 
+00012aa0: 2b3d 2028 6564 6174 612e 6d61 7267 696e  += (edata.margin
+00012ab0: 2862 2c20 6129 202a 2a20 6578 7029 2020  (b, a) ** exp)  
+00012ac0: 2f20 320a 2020 2020 7265 7475 726e 2070  / 2.    return p
+00012ad0: 656e 616c 7479 0a                        enalty.
```

### Comparing `pref_voting-1.3.2/pref_voting/margin_based_methods_old.py` & `pref_voting-1.3.3/pref_voting/margin_based_methods_old.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/monotonicity_axioms.py` & `pref_voting-1.3.3/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/other_methods.py` & `pref_voting-1.3.3/pref_voting/other_methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pref_voting.voting_method import *
 from pref_voting.scoring_methods import plurality
 from pref_voting.profiles import _find_updated_profile, _num_rank
 from pref_voting.profiles_with_ties import ProfileWithTies
 from pref_voting.weighted_majority_graphs import MarginGraph
 from itertools import combinations, permutations
-from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
+from pref_voting.voting_method_properties import ElectionTypes
 
 @vm(name = "Majority",
     skip_registration=True, # skip registration since majority may return an empty list
     input_types = [ElectionTypes.PROFILE])
 def majority(profile, curr_cands = None):
     """The majority winner is the candidate with a strict majority  of first place votes.  Returns an empty list if there is no candidate with a strict majority of first place votes. Returns the majority winner in the ``profile`` restricted to ``curr_cands``.
 
@@ -50,22 +50,15 @@
     curr_cands = profile.candidates if curr_cands is None else curr_cands
 
     plurality_scores = profile.plurality_scores(curr_cands = curr_cands)
     maj_winner = [c for c in curr_cands if plurality_scores[c] >= maj_size]
 
     return sorted(maj_winner)
 
-pareto_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=False,
-    pareto_dominance=True,
-    positive_involvement = True,
-)
 @vm(name = "Pareto",
-    properties = pareto_properties,
     input_types = [ElectionTypes.PROFILE, ElectionTypes.PROFILE_WITH_TIES])
 def pareto(profile, curr_cands = None, strong_Pareto = False, use_extended_strict_preferences = True):
     """Returns the set of candidates who are not Pareto dominated.
 
     For ProfilesWithTies, if strong_Pareto == True, then a dominates b if some voter strictly prefers a to b and no voter strictly prefers b to a.
 
     Args:
@@ -160,22 +153,15 @@
     """
     candidates = profile.candidates if curr_cands is None else curr_cands
     
     rankings = profile._rankings if curr_cands is None else _find_updated_profile(profile._rankings, np.array([c for c in profile.candidates if c not in curr_cands]),  profile.num_cands)
     return _kemeny_young_rankings(list(rankings), list(profile._rcounts), candidates)
 
 
-kemeny_young_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Kemeny-Young",
-    properties = kemeny_young_properties,
     input_types = [ElectionTypes.PROFILE,ElectionTypes.PROFILE_WITH_TIES,  ElectionTypes.MARGIN_GRAPH])
 def kemeny_young(edata, curr_cands = None, algorithm = "marginal"): 
     """A Kemeny-Young ranking is a ranking that maximizes the sum of the margins of pairs of candidates in the ranking. Equivalently, a Kemeny-Young ranking is a ranking that minimizes the sum of the Kendall tau distances to the voters' rankings. The Kemeny-Young winners are the candidates that are ranked first by some Kemeny-Young ranking.
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -235,22 +221,15 @@
                 best_ranking_score = score_of_r
                 ky_rankings = [r]
             if score_of_r == best_ranking_score:
                 ky_rankings.append(r)
     
     return sorted(list(set([r[0] for r in ky_rankings])))
 
-preliminary_weighted_condorcet_properties = VotingMethodProperties(
-    condorcet_winner=True,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm("Preliminary Weighted Condorcet",
-    properties = preliminary_weighted_condorcet_properties,
     input_types = [ElectionTypes.PROFILE])
 def preliminary_weighted_condorcet(prof, curr_cands = None, show_orders = False, require_positive_plurality_score = False):
     """The preliminary version of the Weighted Condorcet Rule in Tideman's book, Collective Decisions and Voting (p. 223). The winners are the candidates ranked first by some linear order of the candidates with highest score, where the score of an order (c_1,...,c_n) is the sum over all i<j of the margin of c_i vs. c_j multiplied by the plurality scores of c_i and c_j. 
     
     The multiplication by plurality scores is what distinguishes this method from the Kemeny-Young method.
     
     Tideman (p. 224) defines a more complicated Weighted Condorcet rule that is intended to be used when some candidates receive zero first-place votes.
@@ -291,22 +270,15 @@
 
     winners = [r[0] for r in best_orders]
 
     return list(set(winners))
 
 ### Bucklin
 
-bucklin_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=False,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Bucklin",
-    properties = bucklin_properties,
     input_types = [ElectionTypes.PROFILE])
 def bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes.  Return the candidates with the greatest overall score.  
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -402,22 +374,15 @@
                        for c in candidates}
         if any([s >= strict_maj_size for s in cand_scores.values()]):
             break
     max_score = max(cand_scores.values())
     return sorted([c for c in candidates if cand_scores[c] >= max_score]), cand_scores
 
 
-simplified_bucklin_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=False,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Simplified Bucklin",
-    properties = simplified_bucklin_properties,
     input_types = [ElectionTypes.PROFILE])
 def simplified_bucklin(profile, curr_cands = None): 
     """If a candidate has a strict majority of first-place votes, then that candidate is the winner. If no such candidate exists, then check the candidates that are ranked first or second.  If a candidate has a strict majority of first- or second-place voters, then that candidate is the winner. If no such winner is found move on to the 3rd, 4th, etc. place votes. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -511,22 +476,15 @@
         cand_scores = {c:sum([cand_to_num_voters_rank[_r][c] for _r in cand_to_num_voters_rank.keys()]) 
                        for c in candidates}
         if any([s >= strict_maj_size for s in cand_scores.values()]):
             break
             
     return sorted([c for c in candidates if cand_scores[c] >= strict_maj_size]), cand_scores
 
-weighted_bucklin_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=None,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Weighted Bucklin",
-    properties = weighted_bucklin_properties,
     input_types = [ElectionTypes.PROFILE])
 def weighted_bucklin(profile, curr_cands = None, strict_threshold = False, score = lambda num_cands, rank: (num_cands - rank)/ (num_cands - 1) if num_cands > 1 else 1): 
     """The Weighted Bucklin procedure, studied by D. Marc Kilgour, Jean-Charles Grégoire, and Angèle Foley. The k-th Weighted Bucklin score of a candidate c is the sum for j \leq k of the product of score(num_cands,j) and the number of voters who rank c in j-th place. Compute higher-order Weighted Bucklin scores until reaching a k such that some candidate's k-th Weighted Bucklin score is at least half the number of voters (or the strict majority size if strict_threshold = True). Then return the candidates with maximal k-th Weighted Bucklin score. Bucklin is the special case where strict_threshold = True and score = lambda num_cands, rank: 1.
     
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -573,22 +531,15 @@
                        for c in candidates}
         if any([s >= threshold for s in cand_scores.values()]):
             break
     max_score = max(cand_scores.values())
 
     return sorted([c for c in candidates if cand_scores[c] >= max_score])
 
-bracket_voting_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Bracket Voting",
-    properties = bracket_voting_properties,
     input_types = [ElectionTypes.PROFILE])
 def bracket_voting(profile, curr_cands = None, seed = None):
     """The candidates with the top four plurality scores are seeded into a bracket: the candidate with the highest plurality score is seeded 1st, the candidate with the second highest plurality score is seeded 2nd, etc. The 1st seed faces the 4th seed in a head-to-head match decided by majority rule, and the 2nd seed faces the 3rd seed in a head-to-head match decided by majority rule. The winners of these two matches face each other in a final head-to-head match decided by majority rule. The winner of the final is the winner of the election.
 
     .. note::
         A version of bracket voting as proposed by Edward B. Foley. This is a probabilistic method that always returns a unique winner. Ties are broken using a random tie breaking ordering of the candidates.
 
@@ -646,22 +597,15 @@
 
     # Ties in the final head-to-head match are broken in favor of the higher-seeded candidate
     else:
         winner = one_four_winner if one_four_winner_seed < two_three_winner_seed else two_three_winner
 
     return [winner]
 
-superior_voting_properties = VotingMethodProperties(
-    condorcet_winner=False,
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=False,
-)
 @vm(name = "Superior Voting",
-    properties = superior_voting_properties,
     input_types = [ElectionTypes.PROFILE])
 def superior_voting(profile, curr_cands = None):
     """One candidate is superior to another if more ballots rank the first candidate above the second than vice versa. A candidate earns a point from a ballot if they are ranked first on that ballot or they are superior to the candidate ranked first on that ballot. The candidate with the most points wins.
 
     .. note::
         Devised by Wesley H. Holliday as a simple Condorcet-compliant method for political elections. Always elects a Condorcet winner if one exists and elects only the Condorcet winner provided the Condorcet winner receives at least one first-place vote. Edward B. Foley suggested the name 'Superior Voting' because the method is based on the idea that if A is superior to B, then A should get B's first-place votes added to their own.
```

### Comparing `pref_voting-1.3.2/pref_voting/prob_voting_method.py` & `pref_voting-1.3.3/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/probabilistic_methods.py` & `pref_voting-1.3.3/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/profiles.py` & `pref_voting-1.3.3/pref_voting/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,14 +543,26 @@
         return ProfileWithTies(
             [{c:cidx for cidx,c in enumerate(list(r))} 
              for r in ranks], 
             rcounts=list(rcounts), 
             candidates = self.candidates, 
             cmap=self.cmap)
     
+    def to_utility_profile(self, seed=None): 
+        """Returns the profile as a UtilityProfile using the function Utility.from_linear_profile to generate the utility function.  
+        So, it assigns a random utility that represents the ranking. 
+        """
+
+        from pref_voting.mappings import Utility
+        from pref_voting.utility_profiles import UtilityProfile
+        
+        return UtilityProfile(
+            [Utility.from_linear_ranking(r, seed=(seed + idx if seed is not None else None)) for idx,r in enumerate(self.rankings)]
+        )
+    
     def to_latex(self, cmap = None, curr_cands = None):
         """Returns a string describing the profile (restricted to ``curr_cands``) as a LaTeX table (use the provided ``cmap`` or the ``cmap`` associated with the profile).
 
         :Example: 
 
         .. exec_code::
```

### Comparing `pref_voting-1.3.2/pref_voting/profiles_with_ties.py` & `pref_voting-1.3.3/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/rankings.py` & `pref_voting-1.3.3/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/scoring_methods.py` & `pref_voting-1.3.3/pref_voting/scoring_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,24 +8,17 @@
 from pref_voting.voting_method import  *
 from pref_voting.social_welfare_function import  *
 from pref_voting.profiles import Profile
 from pref_voting.rankings import Ranking, break_ties_alphabetically
 from pref_voting.voting_method import _num_rank_last 
 from pref_voting.profiles import _find_updated_profile, _num_rank
 from pref_voting.weighted_majority_graphs import MarginGraph
-from pref_voting.voting_method_properties import VotingMethodProperties, ElectionTypes
+from pref_voting.voting_method_properties import  ElectionTypes
 
-pl_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=True,
-    positive_involvement=True, 
-    )
 @vm(name = "Plurality", 
-    properties=pl_properties, 
     input_types=[ElectionTypes.PROFILE, 
                  ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def plurality(profile, curr_cands = None):
     """The **Plurality score** of a candidate :math:`c` is the number of voters that rank :math:`c` in first place. The Plurality winners are the candidates with the largest Plurality score in the ``profile`` restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
@@ -101,22 +94,15 @@
     p_ranking.normalize_ranks()
 
     if tie_breaking == "alphabetic":
         p_ranking = break_ties_alphabetically(p_ranking)
 
     return p_ranking
 
-borda_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=True,
-    pareto_dominance=True,
-    positive_involvement=True, 
-    )
 @vm(name = "Borda",
-    properties=borda_properties,
     input_types=[ElectionTypes.PROFILE, ElectionTypes.MARGIN_GRAPH])
 def borda(edata, curr_cands = None, algorithm = "positional"):
     """The **Borda score** of a candidate is calculated as follows: If there are :math:`m` candidates, then the Borda score of candidate :math:`c` is :math:`\sum_{r=1}^{m} (m - r) * Rank(c,r)` where :math:`Rank(c,r)` is the number of voters that rank candidate :math:`c` in position :math:`r`. The Borda winners are the candidates with the largest Borda score in the ``profile`` restricted to ``curr_cands``. 
     Args:
         edata (Profile, MarginGraph): An anonymous profile of linear orders or a MarginGraph.
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         algorithm (String): if "positional", then the Borda score of a candidate is calculated from each voter's ranking as described above. If "marginal", then the Borda score of a candidate is calculated as the sum of the margins of the candidate vs. all other candidates. The positional scores and marginal scores are affinely equivalent.
@@ -196,22 +182,15 @@
     b_ranking.normalize_ranks()
 
     if tie_breaking == "alphabetic":
         b_ranking = break_ties_alphabetically(b_ranking)
 
     return b_ranking
 
-anti_plurality_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=False,
-    positive_involvement=True,
-    )
 @vm(name = "Anti-Plurality",
-    properties=anti_plurality_properties,
     input_types=[ElectionTypes.PROFILE])
 def anti_plurality(profile, curr_cands = None):
     """The **Anti-Plurality score** of a candidate $c$ is the number of voters that rank $c$ in last place.  The Anti-Plurality winners are the candidates with the smallest Anti-Plurality score in the ``profile`` restricted to ``curr_cands``. 
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -343,22 +322,15 @@
     """Create a scoring method using a given score function and name."""
 
     def _vm(profile, curr_cands = None):
         return scoring_rule(profile, curr_cands = curr_cands, score = score)
 
     return VotingMethod(_vm, name = name)
 
-dowdall_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=True, 
-    positive_involvement=True,
-    )
 @vm(name = "Dowdall",
-    properties=dowdall_properties,
     input_types=[ElectionTypes.PROFILE])
 def dowdall(profile, curr_cands = None):
     """The first-ranked candidate gets 1 point, the second-ranked candidate gets 1/2 point, the third-ranked candidate gets 1/3 point, and so on.  The Dowdall winners are the candidates with the greatest overall score in the profile restricted to ``curr_cands``.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``.
@@ -369,22 +341,15 @@
     .. note::
         This system is used in Nauru. See, e.g., Jon Fraenkel & Bernard Grofman (2014), "The Borda Count and its real-world alternatives: Comparing scoring rules in Nauru and Slovenia," Australian Journal of Political Science, 49:2, 186-205, DOI: 10.1080/10361146.2014.900530.
     
     """
 
     return scoring_rule(profile, curr_cands = curr_cands, score = lambda num_cands, rank: 1 / rank)
 
-pos_neg_voting_properties = VotingMethodProperties(
-    condorcet_winner=False, 
-    condorcet_loser=False,
-    pareto_dominance=False,
-    positive_involvement=True, 
-    )
 @vm(name="Positive-Negative Voting",
-    properties=pos_neg_voting_properties,
     input_types=[ElectionTypes.PROFILE])
 def positive_negative_voting(profile, curr_cands = None):
     """The **Positive-Negative Voting** method is a scoring rule where each voter assigns a score of 1 to their top-ranked candidate and a score of -1 to their bottom-ranked candidate.  See https://onlinelibrary.wiley.com/doi/10.1111/ecin.12929 for more information.
 
     Args:
         profile (Profile): An anonymous profile of linear orders on a set of candidates
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -478,21 +443,15 @@
 
     """
     
     return  {cand: -sum([len([_cand for _cand in profile.candidates if r.extended_strict_pref(_cand, cand)]) * c 
                     for r,c in zip(*profile.rankings_counts)]) for cand in profile.candidates}
 
 
-borda_prof_with_ties_properties = VotingMethodProperties(
-    condorcet_winner=None, 
-    condorcet_loser=None,
-    pareto_dominance=None, 
-    )
 @vm(name="Borda (for Truncated Profiles)",
-    properties=borda_prof_with_ties_properties,
     input_types=[ElectionTypes.TRUNCATED_LINEAR_PROFILE])
 def borda_for_profile_with_ties(
     profile, 
     curr_cands=None, 
     borda_scores=symmetric_borda_scores): 
     """
     Borda score for truncated linear orders using different ways of defining the Borda score for truncated linear
```

### Comparing `pref_voting-1.3.2/pref_voting/social_welfare_function.py` & `pref_voting-1.3.3/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/spatial_profiles.py` & `pref_voting-1.3.3/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/strategic_axioms.py` & `pref_voting-1.3.3/pref_voting/strategic_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/swf_axioms.py` & `pref_voting-1.3.3/pref_voting/swf_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/conftest.py` & `pref_voting-1.3.3/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_c1_methods.py` & `pref_voting-1.3.3/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_combined_methods.py` & `pref_voting-1.3.3/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_generate_profiles.py` & `pref_voting-1.3.3/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-1.3.3/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_io.py` & `pref_voting-1.3.3/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_iterative_methods.py` & `pref_voting-1.3.3/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_majority_graph.py` & `pref_voting-1.3.3/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_mapping.py` & `pref_voting-1.3.3/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-1.3.3/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_margin_graph.py` & `pref_voting-1.3.3/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_other_methods.py` & `pref_voting-1.3.3/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-1.3.3/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_profile.py` & `pref_voting-1.3.3/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-1.3.3/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_ranking.py` & `pref_voting-1.3.3/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_scoring_rules.py` & `pref_voting-1.3.3/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-1.3.3/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_spatial_profile.py` & `pref_voting-1.3.3/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_support_graph.py` & `pref_voting-1.3.3/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_utility_function.py` & `pref_voting-1.3.3/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_utility_functions.py` & `pref_voting-1.3.3/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/tests/test_voting_method.py` & `pref_voting-1.3.3/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/utility_functions.py` & `pref_voting-1.3.3/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/utility_methods.py` & `pref_voting-1.3.3/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/utility_profiles.py` & `pref_voting-1.3.3/pref_voting/utility_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,19 +54,22 @@
     def __init__(self, utilities, ucounts=None, domain=None, cmap=None):
         """Constructor method"""
 
         assert ucounts is None or len(utilities) == len(
             ucounts
         ), "The number of utilities much be the same as the number of ucounts"
 
-        self.domain = (
-            sorted(domain)
-            if domain is not None
-            else sorted(list(set([x for u in utilities for x in u.keys()])))
-        )
+        _domain = domain if domain is not None else []
+        for u in utilities:
+            if isinstance(u, dict):
+                _domain += [x for x in u.keys() if x not in _domain]
+            elif isinstance(u, Utility):
+                _domain += [x for x in u.domain if x not in _domain]
+
+        self.domain = sorted(list(set(_domain)))
         """The domain of the profile. """
 
         self.cmap = cmap if cmap is not None else {c: str(c) for c in self.domain}
         """The candidate map is a dictionary associating an alternative with the name used when displaying a alternative."""
 
         self._utilities = [
             Utility(u, domain = self.domain, cmap=self.cmap)
```

### Comparing `pref_voting-1.3.2/pref_voting/variable_candidate_axioms.py` & `pref_voting-1.3.3/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/variable_voter_axioms.py` & `pref_voting-1.3.3/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pref_voting/voting_method.py` & `pref_voting-1.3.3/pref_voting/voting_method.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 '''
 
 import functools
 import inspect
 import numpy as np
 from numba import jit # Remove until numba supports python 3.11
 import random
+import json
+from pref_voting.voting_method_properties import VotingMethodProperties
+from filelock import FileLock, Timeout
 
 class VotingMethod(object): 
     """
     A class to add functionality to voting methods. 
 
     Args:
         vm (function): An implementation of a voting method. The function should accept a Profile, ProfileWithTies, MajorityGraph, and/or MarginGraph, and a keyword parameter ``curr_cands`` to find the winner after restricting to ``curr_cands``. 
@@ -23,25 +26,32 @@
         properties (VotingMethodProperties): The properties of the voting method.
         input_types (list): The types of input that the voting method can accept.
 
     """
     def __init__(self, 
                  vm, 
                  name=None, 
-                 properties=None, 
                  input_types=None, 
                  skip_registration=False): 
-        
         self.vm = vm
         self.name = name
+
+        # get the properties of the voting method
+        # open voting_methods_properties.json
+
+        vm_props = json.load(open("voting_methods_properties.json"))
+        if name in vm_props:
+            properties = VotingMethodProperties(**vm_props[name])
+        else:
+            properties = VotingMethodProperties()
         self.properties = properties
         self.input_types = input_types
         self.skip_registration = skip_registration
         self.algorithm = None
-        
+
         functools.update_wrapper(self, vm)   
 
     def __call__(self, edata, curr_cands = None, **kwargs):
         
         if (curr_cands is not None and len(curr_cands) == 0) or len(edata.candidates) == 0: 
             return []
         
@@ -82,15 +92,15 @@
         ws = self.__call__(edata, curr_cands = curr_cands)
         return {c: 1.0 / len(ws) if c in ws else 0.0 for c in edata.candidates}
     
     def display(self, edata, curr_cands = None, cmap = None, **kwargs): 
         """
         Display the winning set of candidates.
         """
- 
+
         cmap = cmap if cmap is not None else edata.cmap
 
         ws = self.__call__(edata, curr_cands = curr_cands, **kwargs)
 
         if ws is None:  # some voting methods, such as ``ranked_pairs_with_test``, may return None if it is taking long to compute the winner.
             print(f"{self.name} winning set is not available")
         else: 
@@ -98,23 +108,68 @@
             print(w_str + "{" + ", ".join([str(cmap[c]) for c in ws]) + "}")
         
     def set_name(self, new_name):
         """Set the name of the voting method."""
 
         self.name = new_name
 
+    def add_property(self, prop, value):
+        """Add a property to the voting method."""
+
+        setattr(self.properties, prop, value)
+
+    def remove_property(self, prop):
+        """Remove a property from the voting method."""
+
+        delattr(self.properties, prop)
+
+    def load_properties(self, filename="voting_methods_properties.json"):
+        """Load the properties of the voting method from a JSON file."""
+
+        lock = FileLock(f"{filename}.lock")
+        with lock:
+            try:
+                with open(filename, 'r') as file:
+                    vm_props = json.load(file)
+            except FileNotFoundError:
+                vm_props = {}
+
+            if self.name in vm_props:
+                self.properties = VotingMethodProperties(**vm_props[self.name])
+
+    def save_properties(self, filename="voting_methods_properties.json"):
+        """Save the properties of the voting method to a JSON file."""
+
+        lock = FileLock(f"{filename}.lock")
+        with lock:
+            try:
+                with open(filename, 'r') as file:
+                    vm_props = json.load(file)
+            except FileNotFoundError:
+                vm_props = {}
+
+            vm_props[self.name] = self.properties.__dict__
+
+            with open(filename, 'w') as file:
+                json.dump(vm_props, file, indent=4, sort_keys=True )
+
     def __str__(self): 
         return f"{self.name}"
 
-def vm(name=None, properties=None, input_types=None, skip_registration=False):
+def vm(name=None, 
+       input_types=None, 
+       skip_registration=False):
     """
     A decorator used when creating a voting method. 
     """
     def wrapper(f):
-        return VotingMethod(f, name=name, properties=properties, input_types=input_types, skip_registration=skip_registration)
+        return VotingMethod(f, 
+                            name=name,
+                            input_types=input_types, 
+                            skip_registration=skip_registration)
     return wrapper
 
 @jit(nopython=True, fastmath=True)
 def isin(arr, val):
     """compiled function testing if the value val is in the array arr
     """
```

### Comparing `pref_voting-1.3.2/pref_voting/voting_method_properties.py` & `pref_voting-1.3.3/pref_voting/voting_method_properties.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 class VotingMethodProperties:
     """
     Class to encapsulate properties of voting methods.
 
     Attributes:
         condorcet_consistent (bool): Indicates if the voting method always elects a Condorcet winner when one exists.
     """
-    def __init__(self, condorcet_winner=False, **kwargs):
-        self.condorcet_winner = condorcet_winner
+    def __init__(self, **kwargs):
         for key, value in kwargs.items():
             setattr(self, key, value)
 
     def satisfied(self):
         return [key for key, value in self.__dict__.items() if value==True]
     
     def violated(self):
```

### Comparing `pref_voting-1.3.2/pref_voting/voting_methods_registry.py` & `pref_voting-1.3.3/pref_voting/voting_methods_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,17 @@
                 continue
 
             # If all conditions are met, add to results
             found_methods.append(method_info['method'])
 
         return found_methods
 
+    def __len__(self):
+        return len(self.methods)
+    
     def __iter__(self):
         self._iter = iter(method_details['method'] for method_details in self.methods.values())
         return self
 
     def __next__(self):
         return next(self._iter)
```

### Comparing `pref_voting-1.3.2/pref_voting/weighted_majority_graphs.py` & `pref_voting-1.3.3/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-1.3.2/pyproject.toml` & `pref_voting-1.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "1.3.2"
+version = "1.3.3"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-1.3.2/setup.py` & `pref_voting-1.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '1.3.2',
+    'version': '1.3.3',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-1.3.2/PKG-INFO` & `pref_voting-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 1.3.2
+Version: 1.3.3
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

