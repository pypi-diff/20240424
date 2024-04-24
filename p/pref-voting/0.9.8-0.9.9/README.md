# Comparing `tmp/pref_voting-0.9.8.tar.gz` & `tmp/pref_voting-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.9.8.tar", max compression
+gzip compressed data, was "pref_voting-0.9.9.tar", max compression
```

## Comparing `pref_voting-0.9.8.tar` & `pref_voting-0.9.9.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.8/LICENSE
--rw-r--r--   0        0        0     1770 2024-04-17 23:21:32.714695 pref_voting-0.9.8/README.md
--rw-r--r--   0        0        0       22 2024-04-24 20:32:55.623064 pref_voting-0.9.8/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.8/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.8/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.8/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.8/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-0.9.8/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.8/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.8/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    24283 2024-04-24 20:11:29.996428 pref_voting-0.9.8/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.8/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.8/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.8/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.8/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.8/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-0.9.8/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.8/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.8/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-0.9.8/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-0.9.8/pref_voting/io/writers.py
--rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-0.9.8/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.8/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-0.9.8/pref_voting/mappings.py
--rw-r--r--   0        0        0    70816 2024-04-15 14:41:33.937321 pref_voting-0.9.8/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-0.9.8/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.8/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-0.9.8/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-0.9.8/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.8/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.8/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.8/pref_voting/rankings.py
--rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-0.9.8/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-0.9.8/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.8/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.8/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0    15778 2024-04-19 09:27:40.264571 pref_voting-0.9.8/pref_voting/strategic_axioms.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.8/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.8/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.8/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-0.9.8/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-0.9.8/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-0.9.8/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-0.9.8/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-0.9.8/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.8/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-0.9.8/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0     7265 2024-04-15 14:48:24.940292 pref_voting-0.9.8/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-0.9.8/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-0.9.8/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-0.9.8/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.8/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-0.9.8/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-0.9.8/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-0.9.8/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-0.9.8/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-0.9.8/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-0.9.8/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-0.9.8/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.8/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-0.9.8/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-0.9.8/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.8/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.8/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.8/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    57492 2024-04-19 01:31:48.812848 pref_voting-0.9.8/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.8/pref_voting/voting_method.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.8/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-0.9.8/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      760 2024-04-24 20:32:55.622157 pref_voting-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-0.9.8/setup.py
--rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-17 23:21:32.714695 pref_voting-0.9.9/README.md
+-rw-r--r--   0        0        0       22 2024-04-24 21:20:14.001443 pref_voting-0.9.9/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.9/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.9/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.9/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.9/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-0.9.9/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.9/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.9/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:51:32.848337 pref_voting-0.9.9/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.9/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.9/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.9/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.9/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.9/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-0.9.9/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.9/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.9/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-0.9.9/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-0.9.9/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-0.9.9/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.9/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-0.9.9/pref_voting/mappings.py
+-rw-r--r--   0        0        0    70816 2024-04-15 14:41:33.937321 pref_voting-0.9.9/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-0.9.9/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.9/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-0.9.9/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-0.9.9/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.9/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.9/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.9/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-0.9.9/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-0.9.9/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.9/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.9/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15790 2024-04-24 21:18:21.291486 pref_voting-0.9.9/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.9/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.9/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.9/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-0.9.9/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-0.9.9/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-0.9.9/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-0.9.9/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-0.9.9/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.9/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-0.9.9/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0     7265 2024-04-15 14:48:24.940292 pref_voting-0.9.9/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-0.9.9/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-0.9.9/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-0.9.9/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.9/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-0.9.9/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-0.9.9/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-0.9.9/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-0.9.9/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-0.9.9/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-0.9.9/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-0.9.9/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.9/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-0.9.9/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-0.9.9/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.9/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.9/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.9/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    57504 2024-04-24 21:14:50.598729 pref_voting-0.9.9/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.9/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.9/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-0.9.9/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      760 2024-04-24 21:20:14.000628 pref_voting-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     2855 1970-01-01 00:00:00.000000 pref_voting-0.9.9/setup.py
+-rw-r--r--   0        0        0     2996 1970-01-01 00:00:00.000000 pref_voting-0.9.9/PKG-INFO
```

### Comparing `pref_voting-0.9.8/LICENSE` & `pref_voting-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/README.md` & `pref_voting-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/analysis.py` & `pref_voting-0.9.9/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/axiom.py` & `pref_voting-0.9.9/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/c1_methods.py` & `pref_voting-0.9.9/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/combined_methods.py` & `pref_voting-0.9.9/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/dominance_axioms.py` & `pref_voting-0.9.9/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/generate_profiles.py` & `pref_voting-0.9.9/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/generate_spatial_profiles.py` & `pref_voting-0.9.9/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/generate_utility_profiles.py` & `pref_voting-0.9.9/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.9.9/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/grade_methods.py` & `pref_voting-0.9.9/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/grade_profiles.py` & `pref_voting-0.9.9/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/helper.py` & `pref_voting-0.9.9/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/invariance_axioms.py` & `pref_voting-0.9.9/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/io/readers.py` & `pref_voting-0.9.9/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/io/writers.py` & `pref_voting-0.9.9/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/iterative_methods.py` & `pref_voting-0.9.9/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/maj_graph_ex1.png` & `pref_voting-0.9.9/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/mappings.py` & `pref_voting-0.9.9/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/margin_based_methods.py` & `pref_voting-0.9.9/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/monotonicity_axioms.py` & `pref_voting-0.9.9/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/other_methods.py` & `pref_voting-0.9.9/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/prob_voting_method.py` & `pref_voting-0.9.9/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/probabilistic_methods.py` & `pref_voting-0.9.9/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/profiles.py` & `pref_voting-0.9.9/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/profiles_with_ties.py` & `pref_voting-0.9.9/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/rankings.py` & `pref_voting-0.9.9/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/scoring_methods.py` & `pref_voting-0.9.9/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/social_welfare_function.py` & `pref_voting-0.9.9/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/spatial_profiles.py` & `pref_voting-0.9.9/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/strategic_axioms.py` & `pref_voting-0.9.9/pref_voting/strategic_axioms.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     
     Strategic axioms 
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.axiom_helpers import *
 from itertools import permutations
-from helper import weak_orders
+from pref_voting.helper import weak_orders
 
 def has_strategy_proofness_violation(prof, vm, set_preference = "single-winner", verbose=False):
     """
     Returns True if there is a voter who can benefit by misrepresenting their preferences.
 
     If set_preference = "single-winner", a voter benefits only if they can change the unique winner in the original profile to a unique winner in the new profile such that in their original ranking, the new winner is above the old winner.
```

### Comparing `pref_voting-0.9.8/pref_voting/tests/conftest.py` & `pref_voting-0.9.9/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_c1_methods.py` & `pref_voting-0.9.9/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_combined_methods.py` & `pref_voting-0.9.9/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_generate_profiles.py` & `pref_voting-0.9.9/pref_voting/tests/test_generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-0.9.9/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_io.py` & `pref_voting-0.9.9/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_iterative_methods.py` & `pref_voting-0.9.9/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_majority_graph.py` & `pref_voting-0.9.9/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_mapping.py` & `pref_voting-0.9.9/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-0.9.9/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_margin_graph.py` & `pref_voting-0.9.9/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_other_methods.py` & `pref_voting-0.9.9/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-0.9.9/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_profile.py` & `pref_voting-0.9.9/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-0.9.9/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_ranking.py` & `pref_voting-0.9.9/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_scoring_rules.py` & `pref_voting-0.9.9/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-0.9.9/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_spatial_profile.py` & `pref_voting-0.9.9/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_support_graph.py` & `pref_voting-0.9.9/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_utility_function.py` & `pref_voting-0.9.9/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_utility_functions.py` & `pref_voting-0.9.9/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/tests/test_voting_method.py` & `pref_voting-0.9.9/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/utility_functions.py` & `pref_voting-0.9.9/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/utility_methods.py` & `pref_voting-0.9.9/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/utility_profiles.py` & `pref_voting-0.9.9/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/variable_candidate_axioms.py` & `pref_voting-0.9.9/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/variable_voter_axioms.py` & `pref_voting-0.9.9/pref_voting/variable_voter_axioms.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     Variable voter axioms 
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.axiom_helpers import *
 import numpy as np
 from itertools import product, combinations, permutations
-from helper import weak_orders
+from pref_voting.helper import weak_orders
 
 def divide_electorate(prof):
     """Given a Profile or ProfileWithTies object, yield all possible ways to divide the electorate into two nonempty electorates."""
 
     R, C = prof.rankings_counts
 
     ranges = [range(count+1) for count in C]
```

### Comparing `pref_voting-0.9.8/pref_voting/voting_method.py` & `pref_voting-0.9.9/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.9.9/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.8/pyproject.toml` & `pref_voting-0.9.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.9.8"
+version = "0.9.9"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.9.8/setup.py` & `pref_voting-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'prefsampling>=0.1.16,<0.2.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.',
     'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n\n## Documentation\n\nOnline documentation is available at [https://pref-voting.readthedocs.io](https://pref-voting.readthedocs.io).\n\n## Example Usage\n\nA profile (of linear orders over the candidates) is created by initializing a `Profile` class object.  Simply provide a list of rankings (each ranking is a tuple of numbers) and a list giving the number of voters with each ranking:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [\n    (0, 1, 2, 3), \n    (2, 3, 1, 0), \n    (3, 1, 2, 0), \n    (1, 2, 0, 3), \n    (1, 3, 2, 0)]\n\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function `generate_profile` is used to generate a profile for a given number of candidates and voters:  \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\nTo use one of the many voting methods, import the function from `pref_voting.voting_methods` and apply it to the profile: \n\n```python\nfrom pref_voting.generate_profiles import generate_profile\nfrom pref_voting.voting_methods import *\n\nprof = generate_profile(3, 4)\nsplit_cycle(prof) # returns the sorted list of winning candidates\nsplit_cycle.display(prof) # display the winning candidates\n\n```\n\n## Questions?\n\nFeel free to [send an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
```

### Comparing `pref_voting-0.9.8/PKG-INFO` & `pref_voting-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.9.8
+Version: 0.9.9
 Summary: pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```
