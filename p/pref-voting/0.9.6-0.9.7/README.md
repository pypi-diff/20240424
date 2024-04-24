# Comparing `tmp/pref_voting-0.9.6.tar.gz` & `tmp/pref_voting-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.9.6.tar", max compression
+gzip compressed data, was "pref_voting-0.9.7.tar", max compression
```

## Comparing `pref_voting-0.9.6.tar` & `pref_voting-0.9.7.tar`

### file list

```diff
@@ -1,71 +1,72 @@
--rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.6/LICENSE
--rw-r--r--   0        0        0     3940 2024-03-19 19:30:31.741533 pref_voting-0.9.6/README.md
--rw-r--r--   0        0        0       22 2024-04-15 23:36:02.122378 pref_voting-0.9.6/pref_voting/__init__.py
--rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.6/pref_voting/analysis.py
--rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.6/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.6/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.6/pref_voting/axioms.py
--rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-0.9.6/pref_voting/c1_methods.py
--rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.6/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.6/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    22821 2024-02-18 15:20:46.307786 pref_voting-0.9.6/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.6/pref_voting/generate_spatial_profiles.py
--rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.6/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.6/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.6/pref_voting/grade_methods.py
--rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.6/pref_voting/grade_profiles.py
--rw-r--r--   0        0        0     7381 2024-03-02 21:50:31.230170 pref_voting-0.9.6/pref_voting/helper.py
--rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.6/pref_voting/invariance_axioms.py
--rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.6/pref_voting/io/__init__.py
--rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-0.9.6/pref_voting/io/readers.py
--rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-0.9.6/pref_voting/io/writers.py
--rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-0.9.6/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.6/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-0.9.6/pref_voting/mappings.py
--rw-r--r--   0        0        0    70816 2024-04-15 14:41:33.937321 pref_voting-0.9.6/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-0.9.6/pref_voting/monotonicity_axioms.py
--rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.6/pref_voting/other_methods.py
--rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-0.9.6/pref_voting/prob_voting_method.py
--rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-0.9.6/pref_voting/probabilistic_methods.py
--rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.6/pref_voting/profiles.py
--rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.6/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.6/pref_voting/rankings.py
--rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-0.9.6/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-0.9.6/pref_voting/social_welfare_function.py
--rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.6/pref_voting/social_welfare_functions.py
--rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.6/pref_voting/spatial_profiles.py
--rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.6/pref_voting/tests/__init__.py
--rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.6/pref_voting/tests/conftest.py
--rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.6/pref_voting/tests/test_c1_methods.py
--rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-0.9.6/pref_voting/tests/test_combined_methods.py
--rw-r--r--   0        0        0    12369 2024-02-18 15:11:22.281074 pref_voting-0.9.6/pref_voting/tests/test_generate_profiles.py
--rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-0.9.6/pref_voting/tests/test_generate_spatial_profile.py
--rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-0.9.6/pref_voting/tests/test_io.py
--rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-0.9.6/pref_voting/tests/test_iterative_methods.py
--rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.6/pref_voting/tests/test_majority_graph.py
--rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-0.9.6/pref_voting/tests/test_mapping.py
--rw-r--r--   0        0        0     7265 2024-04-15 14:48:24.940292 pref_voting-0.9.6/pref_voting/tests/test_margin_based_methods.py
--rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-0.9.6/pref_voting/tests/test_margin_graph.py
--rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-0.9.6/pref_voting/tests/test_other_methods.py
--rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-0.9.6/pref_voting/tests/test_prob_voting_method.py
--rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.6/pref_voting/tests/test_profile.py
--rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-0.9.6/pref_voting/tests/test_profile_with_ties.py
--rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-0.9.6/pref_voting/tests/test_ranking.py
--rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-0.9.6/pref_voting/tests/test_scoring_rules.py
--rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-0.9.6/pref_voting/tests/test_social_welfare_functions.py
--rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-0.9.6/pref_voting/tests/test_spatial_profile.py
--rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-0.9.6/pref_voting/tests/test_support_graph.py
--rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-0.9.6/pref_voting/tests/test_utility_function.py
--rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.6/pref_voting/tests/test_utility_functions.py
--rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-0.9.6/pref_voting/tests/test_voting_method.py
--rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-0.9.6/pref_voting/utility_functions.py
--rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.6/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.6/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.6/pref_voting/variable_candidate_axioms.py
--rw-r--r--   0        0        0    52062 2023-12-13 22:47:24.616165 pref_voting-0.9.6/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.6/pref_voting/voting_method.py
--rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.6/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-0.9.6/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      759 2024-04-15 23:36:02.120192 pref_voting-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 pref_voting-0.9.6/setup.py
--rw-r--r--   0        0        0     5165 1970-01-01 00:00:00.000000 pref_voting-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-03-19 19:26:58.359673 pref_voting-0.9.7/LICENSE
+-rw-r--r--   0        0        0     1770 2024-04-17 23:21:32.714695 pref_voting-0.9.7/README.md
+-rw-r--r--   0        0        0       22 2024-04-24 20:17:01.880394 pref_voting-0.9.7/pref_voting/__init__.py
+-rw-r--r--   0        0        0    18867 2023-11-14 11:21:19.592605 pref_voting-0.9.7/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1270 2023-11-14 11:21:20.178458 pref_voting-0.9.7/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.9.7/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.9.7/pref_voting/axioms.py
+-rw-r--r--   0        0        0    33205 2024-04-09 01:59:48.226095 pref_voting-0.9.7/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0    15161 2024-03-15 20:53:44.539281 pref_voting-0.9.7/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    12659 2023-12-07 15:15:32.783919 pref_voting-0.9.7/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    24283 2024-04-24 20:11:29.996428 pref_voting-0.9.7/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     7648 2023-09-26 23:38:41.018490 pref_voting-0.9.7/pref_voting/generate_spatial_profiles.py
+-rw-r--r--   0        0        0     6181 2023-11-14 11:21:22.463664 pref_voting-0.9.7/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    12781 2024-01-20 19:48:28.167312 pref_voting-0.9.7/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     8796 2024-03-02 21:50:31.229821 pref_voting-0.9.7/pref_voting/grade_methods.py
+-rw-r--r--   0        0        0    15536 2024-02-19 21:31:17.860108 pref_voting-0.9.7/pref_voting/grade_profiles.py
+-rw-r--r--   0        0        0     8068 2024-04-19 01:31:48.812126 pref_voting-0.9.7/pref_voting/helper.py
+-rw-r--r--   0        0        0    12710 2023-10-25 22:23:58.100791 pref_voting-0.9.7/pref_voting/invariance_axioms.py
+-rw-r--r--   0        0        0        0 2024-03-17 12:02:53.705325 pref_voting-0.9.7/pref_voting/io/__init__.py
+-rw-r--r--   0        0        0    17327 2024-04-15 10:20:24.422714 pref_voting-0.9.7/pref_voting/io/readers.py
+-rw-r--r--   0        0        0     9283 2024-04-15 10:10:45.393951 pref_voting-0.9.7/pref_voting/io/writers.py
+-rw-r--r--   0        0        0    90549 2024-04-15 01:51:51.467855 pref_voting-0.9.7/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.9.7/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    22586 2024-04-15 17:48:22.507316 pref_voting-0.9.7/pref_voting/mappings.py
+-rw-r--r--   0        0        0    70816 2024-04-15 14:41:33.937321 pref_voting-0.9.7/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    39807 2024-04-15 09:43:01.243011 pref_voting-0.9.7/pref_voting/monotonicity_axioms.py
+-rw-r--r--   0        0        0    24548 2024-03-16 15:19:40.029463 pref_voting-0.9.7/pref_voting/other_methods.py
+-rw-r--r--   0        0        0     2994 2024-04-15 22:33:37.313589 pref_voting-0.9.7/pref_voting/prob_voting_method.py
+-rw-r--r--   0        0        0     4338 2024-04-15 22:36:04.584538 pref_voting-0.9.7/pref_voting/probabilistic_methods.py
+-rw-r--r--   0        0        0    30126 2024-03-21 11:19:48.716586 pref_voting-0.9.7/pref_voting/profiles.py
+-rw-r--r--   0        0        0    31608 2024-03-19 11:44:23.373414 pref_voting-0.9.7/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    13859 2024-03-03 16:50:37.545900 pref_voting-0.9.7/pref_voting/rankings.py
+-rw-r--r--   0        0        0    21026 2024-04-09 02:00:24.744126 pref_voting-0.9.7/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     1891 2024-04-15 22:36:47.601045 pref_voting-0.9.7/pref_voting/social_welfare_function.py
+-rw-r--r--   0        0        0      362 2024-02-16 02:11:21.780066 pref_voting-0.9.7/pref_voting/social_welfare_functions.py
+-rw-r--r--   0        0        0     7395 2024-03-19 17:48:42.747157 pref_voting-0.9.7/pref_voting/spatial_profiles.py
+-rw-r--r--   0        0        0    15778 2024-04-19 09:27:40.264571 pref_voting-0.9.7/pref_voting/strategic_axioms.py
+-rw-r--r--   0        0        0        0 2023-12-03 11:15:38.617857 pref_voting-0.9.7/pref_voting/tests/__init__.py
+-rw-r--r--   0        0        0      666 2024-03-02 21:50:31.231806 pref_voting-0.9.7/pref_voting/tests/conftest.py
+-rw-r--r--   0        0        0     5062 2024-03-19 01:38:04.296201 pref_voting-0.9.7/pref_voting/tests/test_c1_methods.py
+-rw-r--r--   0        0        0     2576 2024-03-19 00:18:02.163482 pref_voting-0.9.7/pref_voting/tests/test_combined_methods.py
+-rw-r--r--   0        0        0    12962 2024-04-24 20:08:43.229903 pref_voting-0.9.7/pref_voting/tests/test_generate_profiles.py
+-rw-r--r--   0        0        0     2504 2024-03-19 18:59:44.204010 pref_voting-0.9.7/pref_voting/tests/test_generate_spatial_profile.py
+-rw-r--r--   0        0        0    15002 2024-04-15 10:21:41.931501 pref_voting-0.9.7/pref_voting/tests/test_io.py
+-rw-r--r--   0        0        0     8943 2024-03-17 11:39:53.682951 pref_voting-0.9.7/pref_voting/tests/test_iterative_methods.py
+-rw-r--r--   0        0        0    11912 2024-03-16 21:03:40.865827 pref_voting-0.9.7/pref_voting/tests/test_majority_graph.py
+-rw-r--r--   0        0        0     6284 2024-04-15 17:49:58.759298 pref_voting-0.9.7/pref_voting/tests/test_mapping.py
+-rw-r--r--   0        0        0     7265 2024-04-15 14:48:24.940292 pref_voting-0.9.7/pref_voting/tests/test_margin_based_methods.py
+-rw-r--r--   0        0        0     7778 2024-04-08 19:41:37.247861 pref_voting-0.9.7/pref_voting/tests/test_margin_graph.py
+-rw-r--r--   0        0        0     3722 2024-03-17 11:44:20.741638 pref_voting-0.9.7/pref_voting/tests/test_other_methods.py
+-rw-r--r--   0        0        0     1815 2024-04-15 22:34:08.166452 pref_voting-0.9.7/pref_voting/tests/test_prob_voting_method.py
+-rw-r--r--   0        0        0    11558 2024-03-19 11:40:09.393149 pref_voting-0.9.7/pref_voting/tests/test_profile.py
+-rw-r--r--   0        0        0    20184 2024-04-08 19:41:37.248346 pref_voting-0.9.7/pref_voting/tests/test_profile_with_ties.py
+-rw-r--r--   0        0        0     8964 2024-03-17 10:17:34.347218 pref_voting-0.9.7/pref_voting/tests/test_ranking.py
+-rw-r--r--   0        0        0     5543 2024-03-19 11:54:18.932325 pref_voting-0.9.7/pref_voting/tests/test_scoring_rules.py
+-rw-r--r--   0        0        0     1531 2024-04-15 14:32:09.859043 pref_voting-0.9.7/pref_voting/tests/test_social_welfare_functions.py
+-rw-r--r--   0        0        0     5459 2024-04-08 19:41:37.248846 pref_voting-0.9.7/pref_voting/tests/test_spatial_profile.py
+-rw-r--r--   0        0        0     2429 2024-04-08 19:41:37.249181 pref_voting-0.9.7/pref_voting/tests/test_support_graph.py
+-rw-r--r--   0        0        0     3808 2024-04-15 19:15:01.227825 pref_voting-0.9.7/pref_voting/tests/test_utility_function.py
+-rw-r--r--   0        0        0     1943 2024-03-19 18:31:19.950002 pref_voting-0.9.7/pref_voting/tests/test_utility_functions.py
+-rw-r--r--   0        0        0     1585 2024-04-08 19:41:37.249465 pref_voting-0.9.7/pref_voting/tests/test_voting_method.py
+-rw-r--r--   0        0        0     3963 2024-04-08 22:35:46.799439 pref_voting-0.9.7/pref_voting/utility_functions.py
+-rw-r--r--   0        0        0     7245 2024-02-16 01:32:30.000312 pref_voting-0.9.7/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    12673 2024-02-19 23:28:54.492364 pref_voting-0.9.7/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0    18724 2023-12-05 16:58:20.198435 pref_voting-0.9.7/pref_voting/variable_candidate_axioms.py
+-rw-r--r--   0        0        0    57492 2024-04-19 01:31:48.812848 pref_voting-0.9.7/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5566 2023-12-07 15:03:17.438046 pref_voting-0.9.7/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      372 2023-11-14 00:06:58.907333 pref_voting-0.9.7/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    57320 2024-04-08 19:41:37.250216 pref_voting-0.9.7/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      758 2024-04-24 20:17:01.877386 pref_voting-0.9.7/pyproject.toml
+-rw-r--r--   0        0        0     2847 1970-01-01 00:00:00.000000 pref_voting-0.9.7/setup.py
+-rw-r--r--   0        0        0     2988 1970-01-01 00:00:00.000000 pref_voting-0.9.7/PKG-INFO
```

### Comparing `pref_voting-0.9.6/LICENSE` & `pref_voting-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/analysis.py` & `pref_voting-0.9.7/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/axiom.py` & `pref_voting-0.9.7/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/c1_methods.py` & `pref_voting-0.9.7/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/combined_methods.py` & `pref_voting-0.9.7/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/dominance_axioms.py` & `pref_voting-0.9.7/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/generate_profiles.py` & `pref_voting-0.9.7/pref_voting/generate_profiles.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pref_voting.generate_spatial_profiles import generate_spatial_profile
 from pref_voting.generate_utility_profiles import linear_utility
 import numpy as np 
 import math
 import random
 from scipy.stats import gamma
 from itertools import permutations
+from pref_voting.helper import weak_compositions
 
 from pref_voting.profiles_with_ties import ProfileWithTies
 from ortools.linear_solver import pywraplp
 from prefsampling.ordinal import impartial, impartial_anonymous, urn, plackett_luce, didi, stratification, single_peaked_conitzer, single_peaked_walsh, single_peaked_circle, single_crossing, euclidean, mallows
 
 from prefsampling.core.euclidean import EuclideanSpace
 from collections import Counter
@@ -395,34 +396,37 @@
         rankings = single_crossing(num_voters,
                                    num_candidates, 
                                    seed=seed) 
         
     elif probmodel == "euclidean":
         
         euclidean_spaces = {
-            "uniform": EuclideanSpace.UNIFORM,
-            "ball": EuclideanSpace.BALL,
-            "gaussian": EuclideanSpace.GAUSSIAN,
-            "sphere": EuclideanSpace.SPHERE,
+            "gaussian_ball": EuclideanSpace.GAUSSIAN_BALL,
+            "gaussian_cube": EuclideanSpace.GAUSSIAN_CUBE,
+            "unbounded_gaussian": EuclideanSpace.UNBOUNDED_GAUSSIAN,
+            "uniform_ball": EuclideanSpace.UNIFORM_BALL,
+            "uniform_cube": EuclideanSpace.UNIFORM_CUBE,
+            "uniform_sphere": EuclideanSpace.UNIFORM_SPHERE,
         }
 
         if 'space' in kwargs:
             space = kwargs['space']
         else:
-            space = "uniform"
+            space = "uniform_ball"
 
         if 'dimension' in kwargs:
             dimension = kwargs['dimension']
         else:
             dimension = 2
 
         rankings = euclidean(num_voters,
                              num_candidates, 
-                             space=euclidean_spaces[space],
-                             dimension=dimension, 
+                             voters_positions=euclidean_spaces[space],
+                             candidates_positions=euclidean_spaces[space],
+                             num_dimensions=dimension, 
                              seed=seed) 
     
     else: 
         raise ValueError("Error: The probability model is not recognized.")
         
     return rankings
 
@@ -500,14 +504,50 @@
         if anonymize: 
             prof = prof.anonymize()
         profs.append(prof)
 
     return profs[0] if num_profiles == 1 else profs
 
 
+def enumerate_anon_profile(num_cands, num_voters):
+    """A generator that enumerates all anonymous profiles with num_cands candidates and num_voters voters.
+
+    Args:
+        num_cands (int): Number of candidates.
+        num_voters (int): Number of voters.
+
+    Yields:
+        Profile: An anonymous profile.
+    """
+    
+    ballot_types = list(permutations(range(num_cands)))
+    num_ballot_types = len(ballot_types)
+
+    for comp in weak_compositions(num_voters, num_ballot_types):
+        yield Profile(ballot_types, rcounts = comp)
+
+
+def enumerate_anon_profile_with_ties(num_cands, num_voters):
+    """A generator that enumerates all anonymous profiles--allowing ties and omissions in ballots--with num_cands candidates and num_voters voters
+
+    Args:
+        num_cands (int): Number of candidates.
+        num_voters (int): Number of voters.
+
+    Yields:
+        ProfileWithTies: An anonymous profile.
+    """
+    
+    ballot_types = list(weak_orders(range(num_cands)))
+    num_ballot_types = len(ballot_types)
+
+    for comp in weak_compositions(num_voters, num_ballot_types):
+        yield ProfileWithTies(ballot_types, rcounts = comp)
+
+
 ####
 # Generating ProfilesWithTies
 ####
 
 
 def strict_weak_orders(A):
     if not A:  # i.e., A is empty
@@ -592,26 +632,26 @@
         cmap=lprof.cmap,
         candidates=lprof.candidates
     )
     prof.use_extended_strict_preference()
     return prof
 
 ####
-# Generating Profile from qualitative margin graph
+# Generating Profile from ordinal margin graph
 ####
 
 def minimal_profile_from_edge_order(cands, edge_order):
-    """Given a list of candidates and a list of edges (positive margin edges only) in order of descending strength, find a minimal profile whose qualitative margin graph has that edge order.
+    """Given a list of candidates and a list of edges (positive margin edges only) in order of descending strength, find a minimal profile whose ordinal margin graph has that edge order.
 
     Args: 
         cands (list): list of candidates
         edge_order (list): list of edges in order of descending strength
 
     Returns:
-        Profile: a profile whose qualitative margin graph has the given edge order
+        Profile: a profile whose ordinal margin graph has the given edge order
     """
 
     solver = pywraplp.Solver.CreateSolver("SAT")
 
     num_cands = len(cands)
     rankings = list(permutations(range(num_cands)))
```

### Comparing `pref_voting-0.9.6/pref_voting/generate_spatial_profiles.py` & `pref_voting-0.9.7/pref_voting/generate_spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/generate_utility_profiles.py` & `pref_voting-0.9.7/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.9.7/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/grade_methods.py` & `pref_voting-0.9.7/pref_voting/grade_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/grade_profiles.py` & `pref_voting-0.9.7/pref_voting/grade_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/helper.py` & `pref_voting-0.9.7/pref_voting/helper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from pref_voting.profiles import Profile
 from pref_voting.profiles_with_ties import ProfileWithTies
 from pref_voting.weighted_majority_graphs import MajorityGraph
 from pref_voting.rankings import Ranking
 from pref_voting.social_welfare_function import *
 from pref_voting.voting_method import *
+from itertools import combinations
 import random
 
 import networkx as nx
 
 def get_mg(edata, curr_cands = None): 
     
     if curr_cands == None: 
@@ -192,7 +193,29 @@
 
     def _register(self, a, b):
         """register that a P b, without forming the transitive closure"""
         if not self.P[a][b]:
             self.P[a][b] = True
             self.preds[b].append(a)
             self.succs[a].append(b)
+
+def weak_orders(A):
+    """A generator for all weak orders on A"""
+    if not A:
+        yield {}
+        return
+    for k in range(1, len(A) + 1):
+        for B in itertools.combinations(A, k):
+            for order in weak_orders(set(A) - set(B)):
+                new_order = {cand: rank + 1 for cand, rank in order.items()}
+                yield {**new_order, **{cand: 0 for cand in B}}
+
+
+def weak_compositions(n, k):
+    """A generator for all weak compositions of n into k parts"""
+
+    if k == 1:
+        yield [n]
+    else:
+        for i in range(n + 1):
+            for comp in weak_compositions(n - i, k - 1):
+                yield [i] + comp
```

### Comparing `pref_voting-0.9.6/pref_voting/invariance_axioms.py` & `pref_voting-0.9.7/pref_voting/invariance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/io/readers.py` & `pref_voting-0.9.7/pref_voting/io/readers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/io/writers.py` & `pref_voting-0.9.7/pref_voting/io/writers.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/iterative_methods.py` & `pref_voting-0.9.7/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/maj_graph_ex1.png` & `pref_voting-0.9.7/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/mappings.py` & `pref_voting-0.9.7/pref_voting/mappings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/margin_based_methods.py` & `pref_voting-0.9.7/pref_voting/margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/monotonicity_axioms.py` & `pref_voting-0.9.7/pref_voting/monotonicity_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/other_methods.py` & `pref_voting-0.9.7/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/prob_voting_method.py` & `pref_voting-0.9.7/pref_voting/prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/probabilistic_methods.py` & `pref_voting-0.9.7/pref_voting/probabilistic_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/profiles.py` & `pref_voting-0.9.7/pref_voting/profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/profiles_with_ties.py` & `pref_voting-0.9.7/pref_voting/profiles_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/rankings.py` & `pref_voting-0.9.7/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/scoring_methods.py` & `pref_voting-0.9.7/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/social_welfare_function.py` & `pref_voting-0.9.7/pref_voting/social_welfare_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/spatial_profiles.py` & `pref_voting-0.9.7/pref_voting/spatial_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/conftest.py` & `pref_voting-0.9.7/pref_voting/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_c1_methods.py` & `pref_voting-0.9.7/pref_voting/tests/test_c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_combined_methods.py` & `pref_voting-0.9.7/pref_voting/tests/test_combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_generate_profiles.py` & `pref_voting-0.9.7/pref_voting/tests/test_generate_profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,40 +262,56 @@
                              probmodel="euclidean")
     assert type(prof) == Profile
     assert len(prof.candidates) == 4
     assert len(prof.rankings) == 3
 
     prof = generate_profile(4, 3, 
                              dim=2,
-                             space='uniform',
+                             space='gaussian_ball',
                              probmodel="euclidean")
     assert type(prof) == Profile
     assert len(prof.candidates) == 4
     assert len(prof.rankings) == 3
 
     prof = generate_profile(4, 3, 
                              dim=2,
-                             space='ball',
+                             space='gaussian_cube',
                              probmodel="euclidean")
     assert type(prof) == Profile
     assert len(prof.candidates) == 4
     assert len(prof.rankings) == 3
 
     prof = generate_profile(4, 3, 
                              dim=2,
-                             space='gaussian',
+                             space='unbounded_gaussian',
                              probmodel="euclidean")
     assert type(prof) == Profile
     assert len(prof.candidates) == 4
     assert len(prof.rankings) == 3
 
 
     prof = generate_profile(4, 3, 
                              dim=4,
-                             space='sphere',
+                             space='uniform_ball',
+                             probmodel="euclidean")
+    assert type(prof) == Profile
+    assert len(prof.candidates) == 4
+    assert len(prof.rankings) == 3
+
+    prof = generate_profile(4, 3, 
+                             dim=2,
+                             space='uniform_cube',
+                             probmodel="euclidean")
+    assert type(prof) == Profile
+    assert len(prof.candidates) == 4
+    assert len(prof.rankings) == 3
+
+    prof = generate_profile(4, 3, 
+                             dim=2,
+                             space='uniform_sphere',
                              probmodel="euclidean")
     assert type(prof) == Profile
     assert len(prof.candidates) == 4
     assert len(prof.rankings) == 3
 
 
 def test_generate_multiple_profiles():
```

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_generate_spatial_profile.py` & `pref_voting-0.9.7/pref_voting/tests/test_generate_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_io.py` & `pref_voting-0.9.7/pref_voting/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_iterative_methods.py` & `pref_voting-0.9.7/pref_voting/tests/test_iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_majority_graph.py` & `pref_voting-0.9.7/pref_voting/tests/test_majority_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_mapping.py` & `pref_voting-0.9.7/pref_voting/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_margin_based_methods.py` & `pref_voting-0.9.7/pref_voting/tests/test_margin_based_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_margin_graph.py` & `pref_voting-0.9.7/pref_voting/tests/test_margin_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_other_methods.py` & `pref_voting-0.9.7/pref_voting/tests/test_other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_prob_voting_method.py` & `pref_voting-0.9.7/pref_voting/tests/test_prob_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_profile.py` & `pref_voting-0.9.7/pref_voting/tests/test_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_profile_with_ties.py` & `pref_voting-0.9.7/pref_voting/tests/test_profile_with_ties.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_ranking.py` & `pref_voting-0.9.7/pref_voting/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_scoring_rules.py` & `pref_voting-0.9.7/pref_voting/tests/test_scoring_rules.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_social_welfare_functions.py` & `pref_voting-0.9.7/pref_voting/tests/test_social_welfare_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_spatial_profile.py` & `pref_voting-0.9.7/pref_voting/tests/test_spatial_profile.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_support_graph.py` & `pref_voting-0.9.7/pref_voting/tests/test_support_graph.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_utility_function.py` & `pref_voting-0.9.7/pref_voting/tests/test_utility_function.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_utility_functions.py` & `pref_voting-0.9.7/pref_voting/tests/test_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/tests/test_voting_method.py` & `pref_voting-0.9.7/pref_voting/tests/test_voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/utility_functions.py` & `pref_voting-0.9.7/pref_voting/utility_functions.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/utility_methods.py` & `pref_voting-0.9.7/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/utility_profiles.py` & `pref_voting-0.9.7/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/variable_candidate_axioms.py` & `pref_voting-0.9.7/pref_voting/variable_candidate_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/variable_voter_axioms.py` & `pref_voting-0.9.7/pref_voting/variable_voter_axioms.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     
     Variable voter axioms 
 """
 
 from pref_voting.axiom import Axiom
 from pref_voting.axiom_helpers import *
 import numpy as np
-from itertools import product, combinations
+from itertools import product, combinations, permutations
+from helper import weak_orders
 
 def divide_electorate(prof):
     """Given a Profile or ProfileWithTies object, yield all possible ways to divide the electorate into two nonempty electorates."""
 
     R, C = prof.rankings_counts
 
     ranges = [range(count+1) for count in C]
@@ -952,14 +953,15 @@
     return witnesses
                     
 tolerant_positive_involvement = Axiom(
     "Tolerant Positive Involvement",
     has_violation = has_tolerant_positive_involvement_violation,
     find_all_violations = find_all_tolerant_positive_involvement_violations, 
 )
+    
 
 def has_bullet_vote_positive_involvement_violation(prof, vm, verbose=False, coalition_size = 1, require_resoluteness = False, require_uniquely_weighted = False, check_probabilities = False):
     """
     Returns True if it is possible to cause a winner A to lose by adding coalition_size-many new voters who bullet vote for A.
 
     If require_resoluteness = True, then only profiles with a unique winner are considered.
 
@@ -1124,14 +1126,145 @@
 
 bullet_vote_positive_involvement = Axiom(
     "Bullet Vote Positive Involvement",
     has_violation = has_bullet_vote_positive_involvement_violation,
     find_all_violations = find_all_bullet_vote_positive_involvement_violations, 
 )
 
+def has_single_voter_resolvability_violation(prof, vm, verbose=False):
+    """
+    If prof is a Profile, returns True if there are multiple vm winners in prof and for one such winner A, there is no linear ballot that can be added to prof to make A the unique winner.
+
+    If prof is a ProfileWithTies, returns True if there are multiple vm winners in prof and for one such winner A, there is no Ranking (allowing ties) that can be added to prof to make A the unique winner. 
+
+    Args:
+        prof: a Profile or ProfileWithTies object.
+        vm (VotingMethod): A voting method to test.
+        verbose (bool, default=False): If a violation is found, display the violation.
+
+    Returns:
+        Result of the test (bool): Returns True if there is a violation and False otherwise.
+    """
+
+    winners = vm(prof)
+
+    if isinstance(prof,ProfileWithTies):
+        prof.use_extended_strict_preference()
+
+    if len(winners) > 1:
+        for winner in winners:
+
+            found_voter_to_add = False
+
+            if isinstance(prof,Profile):
+                for r in permutations(prof.candidates):
+                    new_prof = Profile(prof.rankings + [r])
+                    if vm(new_prof) == [winner]:
+                        found_voter_to_add = True
+                        break
+                   
+            if isinstance(prof,ProfileWithTies):
+                for _r in weak_orders(prof.candidates):
+                    r = Ranking(_r)
+                    new_prof = ProfileWithTies(prof.rankings + [r], candidates = prof.candidates)
+                    new_prof.use_extended_strict_preference()
+                    if vm(new_prof) == [winner]:
+                        found_voter_to_add = True
+                        break
+        
+            if not found_voter_to_add:
+
+                if verbose:
+                    if isinstance(prof,Profile):
+                        print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a linear ballot.")
+                    if isinstance(prof,ProfileWithTies):
+                        print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a Ranking.")
+                    print("")
+                    print("Profile:")
+                    prof.display()
+                    print(prof.description())
+                    print("")
+                    vm.display(prof)
+                    prof.display_margin_graph()
+                    print("")
+
+                return True
+            
+        return False
+
+def find_all_single_voter_resolvability_violations(prof, vm, verbose=False):
+    """
+    If prof is a Profile, returns a list of candidates who win in prof but who cannot be made the unique winner by adding a linear ballot.
+
+    If prof is a ProfileWithTies, returns a list of candidates who win in prof but who cannot be made the unique winner by adding a Ranking (allowing ties).
+
+    Args:
+        prof: a Profile or ProfileWithTies object.
+        vm (VotingMethod): A voting method to test.
+        verbose (bool, default=False): If a violation is found, display the violation.
+
+    Returns:
+        A List of candidates who win in the given profile but who cannot be made the unique winner by adding a ballot.
+    """
+
+    winners = vm(prof)
+
+    if isinstance(prof,ProfileWithTies):
+        prof.use_extended_strict_preference()
+
+    violations = list()
+
+    if len(winners) > 1:
+        for winner in winners:
+
+            found_voter_to_add = False
+
+            if isinstance(prof,Profile):
+                for r in permutations(prof.candidates):
+                    new_prof = Profile(prof.rankings + [r])
+                    if vm(new_prof) == [winner]:
+                        found_voter_to_add = True
+                        break
+                   
+            if isinstance(prof,ProfileWithTies):
+                for _r in weak_orders(prof.candidates):
+                    r = Ranking(_r)
+                    new_prof = ProfileWithTies(prof.rankings + [r], candidates = prof.candidates)
+                    new_prof.use_extended_strict_preference()
+                    if vm(new_prof) == [winner]:
+                        found_voter_to_add = True
+                        break
+        
+            if not found_voter_to_add:
+
+                if verbose:
+                    if isinstance(prof,Profile):
+                        print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a linear ballot.")
+                    if isinstance(prof,ProfileWithTies):
+                        print(f"Violation of Single-Voter Resolvability for {vm.name}: cannot make {winner} the unique winner by adding a Ranking.")
+                    print("")
+                    print("Profile:")
+                    prof.display()
+                    print(prof.description())
+                    print("")
+                    vm.display(prof)
+                    prof.display_margin_graph()
+                    print("")
+
+                violations.append(winner)
+            
+    return violations
+
+single_voter_resolvability = Axiom(
+    "Single-Voter Resolvability",
+    has_violation = has_single_voter_resolvability_violation,
+    find_all_violations = find_all_single_voter_resolvability_violations, 
+)
+
 variable_voter_axioms = [
     reinforcement,
     positive_involvement,
     negative_involvement,
     tolerant_positive_involvement,
-    bullet_vote_positive_involvement
+    bullet_vote_positive_involvement,
+    single_voter_resolvability,
 ]
```

### Comparing `pref_voting-0.9.6/pref_voting/voting_method.py` & `pref_voting-0.9.7/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.9.7/pref_voting/weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.9.6/pyproject.toml` & `pref_voting-0.9.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.9.6"
+version = "0.9.7"
 description = "pref_voting is a Python package that contains tools to reason about elections and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
 
@@ -21,10 +21,10 @@
 networkx = "^3.0"
 tabulate = "^0.9.0"
 random2 = "^1.0.1"
 matplotlib = "^3.5.2"
 nashpy = "^0.0.40"
 numba = "^0.58.0"
 ortools = "^9.8.0"
-prefsampling = "^0.1.0"
+prefsampling = "0.1.9"
 
 [tool.poetry.dev-dependencies]
```

