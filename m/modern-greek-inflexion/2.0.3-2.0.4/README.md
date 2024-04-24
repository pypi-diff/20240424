# Comparing `tmp/modern_greek_inflexion-2.0.3.tar.gz` & `tmp/modern_greek_inflexion-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modern_greek_inflexion-2.0.3.tar", last modified: Mon Apr 15 10:33:41 2024, max compression
+gzip compressed data, was "modern_greek_inflexion-2.0.4.tar", last modified: Wed Apr 24 19:13:35 2024, max compression
```

## Comparing `modern_greek_inflexion-2.0.3.tar` & `modern_greek_inflexion-2.0.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12917 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.048667 modern_greek_inflexion-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.052667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/create_all_adj.py
--rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/create_all_alt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/basic/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adverb/
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adverb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/article/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/article/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38618 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/create_noun_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    28146 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/create_noun_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/
--rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/create_num_decl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/create_num_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.056667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/create_pron_basic.py
--rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/create_pron_decl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.060667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/adj.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/adv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/article.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.096667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-15 10:33:35.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/el_GR.pickle
--rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
--rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
--rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/noun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/numerals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/prefixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/pronouns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    33779 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/verb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.096667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/
--rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.096667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.096667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.096667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.100667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.100667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.100667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
--rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
--rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13924 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 10:33:41.000000 modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:41.104667 modern_greek_inflexion-2.0.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:33:36.000000 modern_greek_inflexion-2.0.3/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13006 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 19:13:35.597038 modern_greek_inflexion-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.541038 modern_greek_inflexion-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31016 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10896 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_alt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18381 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.545038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38636 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28303 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_decl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_basic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11934 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_decl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.549038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/article.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10077 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127) 29309847 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/el_GR.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)   347390 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)    31261 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle
+-rw-r--r--   0 runner    (1001) docker     (127)     5954 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/noun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3386 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/numerals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5945 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/prefixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/pronouns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4777 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33779 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/verb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/
+-rw-r--r--   0 runner    (1001) docker     (127)    11070 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.589038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17670 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5051 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7476 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6978 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3427 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13709 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11534 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8856 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14013 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5222 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-24 19:13:35.000000 modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:35.593038 modern_greek_inflexion-2.0.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 19:13:30.000000 modern_greek_inflexion-2.0.4/test/test_case.py
```

### Comparing `modern_greek_inflexion-2.0.3/LICENSE` & `modern_greek_inflexion-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/PKG-INFO` & `modern_greek_inflexion-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
```

### Comparing `modern_greek_inflexion-2.0.3/README.md` & `modern_greek_inflexion-2.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
```

### Comparing `modern_greek_inflexion-2.0.3/setup.cfg` & `modern_greek_inflexion-2.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modern-greek-inflexion
-version = 2.0.3
+version = 2.0.4
 description = Python 3 library for creating inflected forms given basic forms of Modern Greek words
 long_description_content_type = text/markdown
 long_description = file: README.md
 license = MIT
 url = https://github.com/PicusZeus/modern-greek-inflexion
 author = Krzysztof H
 author_email = krzysztof.hilman@gmail.com
```

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/_helpers.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/_helpers.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/create_all_adj.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/all/create_all_alt.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/all/create_all_alt.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adjective/basic/create_basic_adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/adverb/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/adverb/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/article/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/article/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/create_noun_basic.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     :param proper_name: If you know that the noun is actually a proper name, set it to True. The flag by default is False.
     :return: dictionary with the following keys: NOM_SG, GEN_SG, NOM_PL, GENDERS, PROPER_NAME
     """
 
     noun = convert_to_monotonic(noun, one_syllable_rule=False)
     if not greek_pattern.match(noun):
         raise NotInGreekException
-    noun_temp = {NOM_SG: noun, GEN_SG: '', NOM_PL: '', GENDERS: []}
+    noun_temp = {NOM_SG: noun, GEN_SG: '', NOM_PL: '', GENDERS: [], "aklito": aklito}
 
     if not gender:
         if noun in nouns_masc_fem:
             gender = MASC_FEM
         elif noun in plur_tant_neut:
             gender = NEUT_PL
         elif noun.endswith('ικα') or noun.endswith('ικά'):
```

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/noun/create_noun_decl.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/noun/create_noun_decl.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from ..resources import greek_corpus
 from ..resources.typing import genders_declensions_type, genderBasicType
 from ..resources.variables import *
 from ..resources.noun import irregular_gen_sg, irregular_voc_sg, noun_grammar_lists
 
 
 def create_all_noun_forms(nom_sg: str, gen_sg: str, nom_pl: str, genders: list[genderBasicType],
-                          proper_name: bool = False) -> genders_declensions_type:
+                          proper_name: bool = False, aklito=False) -> genders_declensions_type:
     """
     :param nom_sg: nominative singular
     :param gen_sg: genitive singular
     :param nom_pl: nominative plural
     :param genders: a list with gender variables (FEM, MASC, NEUT)
     :param proper_name: flag useful for creation of vocatives in proper names
+    :param aklito: noun is indeclinable
     :return: A dictionary {MASC: {SG: {NOM: str, ...}, ...}, ...}
     """
 
     accent = where_is_accent(nom_sg, true_syllabification=False)
     number_of_syllables = count_syllables(nom_sg)
     multiple_plurals = ',' in nom_pl
     noun_all = {}
@@ -326,15 +327,15 @@
 
                     elif n_pl:
                         pl_accent = where_is_accent(n_pl, true_syllabification=False)
                         gen_pl.append(put_accent(n_pl[:-2] + 'ων', pl_accent, true_syllabification=False))
 
                 noun_all[gender][PL][GEN] = ','.join(gen_pl)
 
-            elif nom_sg[-1:] == 'α' and gender == NEUT and nom_sg != nom_pl:
+            elif nom_sg[-1:] == 'α' and gender == NEUT and nom_sg != nom_pl and not aklito:
                 noun_all[gender][SG][ACC] = nom_sg
                 gen_pl = ''
                 if nom_pl:
                     # there can be alternative roots like gala
                     gen_pl = ','.join([put_accent(n_pl[:-1] + 'ων', PENULTIMATE) for n_pl in nom_pl.split(',')])
                 noun_all[gender][PL][GEN] = gen_pl
 
@@ -529,14 +530,17 @@
                         gen_pl = put_accent(gen_pl, ULTIMATE)
                     noun_all[gender][PL][GEN] = gen_pl
                 else:
                     noun_all[gender][SG][ACC] = nom_sg
                     gen_pl = put_accent(nom_pl[:-1] + 'ων', PENULTIMATE)
                     noun_all[gender][PL][GEN] = gen_pl
 
+            elif aklito and nom_pl:
+                noun_all[gender][PL][GEN] = nom_pl
+
             elif not nom_sg and (nom_pl[-2:] in ['ες', 'οι', 'ές', 'οί', 'αι', 'αί'] or
                                  nom_pl[-1:] in ['α', 'η', 'ά', 'ή'] or
                                  nom_pl.endswith('εις')):
                 accent = where_is_accent(nom_pl, true_syllabification=False)
                 if nom_pl[-2:] in ['οι', 'οί']:
 
                     acc_pl = put_accent(nom_pl[:-2] + 'ους', accent, true_syllabification=False)
```

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/create_num_decl.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_decl.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/numeral/create_num_list.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/numeral/create_num_list.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/create_pron_basic.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_basic.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/pronoun/create_pron_decl.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/pronoun/create_pron_decl.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/adj.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/adj.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/article.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/article.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/adj_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/el_GR.pickle` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/el_GR.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/noun_grammar_lists.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/lists/nouns_masc_fem.pickle`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/noun.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/noun.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/numerals.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/numerals.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/prefixes.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/prefixes.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/pronouns.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/pronouns.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/typing.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/typing.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/variables.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/variables.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/resources/verb.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/resources/verb.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/__init__.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/__init__.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_past_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_pers_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_present_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_all_subjunctive_personal_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/all/persons/create_imp_pass.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_all_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_active.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_aorist_passive.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_conjunctive_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_active.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_paratatikos_passive.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/create_basic_present_forms.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_aorist_participles.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_passive_perfect_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_active_participle_arch.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/forms/basic/participles/create_present_passive_participle.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_active_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_passive_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_regular_perf_root.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/create/roots/create_roots_from_past.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/helpers.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/helpers.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_active_non_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_past_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_passive_present_continuous_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion/verb/recognize/recognize_past_conjugation.py`

 * *Files identical despite different names*

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/PKG-INFO` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modern-greek-inflexion
-Version: 2.0.3
+Version: 2.0.4
 Summary: Python 3 library for creating inflected forms given basic forms of Modern Greek words
 Home-page: https://github.com/PicusZeus/modern-greek-inflexion
 Author: Krzysztof H
 Author-email: krzysztof.hilman@gmail.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -56,14 +56,15 @@
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
 
 
 ## Change Log
+ * 2.0.4 Fixed bug that caused incorrect creation of gen pl for some indeclinable nouns.
  * 2.0.3 Fixed issue with augmentation of dimotic verbs prefixed with 'para'. Also forcibly removed katharevousan types from such verbs. Fixed issue with indeclinable nouns ending on 'a', for which previously erroneously gen pl with ων ending was being created.
  * 2.0.2 Fixed issue, when sigmatic aorist stem is created when it exists only for passive imperative (ζέστανα but ζεστάσου).
  * 2.0.1 Fixed inconsistencies in the format of the output (in pronouns, where in some cases forms were given as string and not as set of strings)
  * 2.0.0 Major code refactoring with changes that break previous API. Code is quicker by about 25%, better readability, new docs, before migrating, read usage docs.
  * 1.0.6 Minor fixes and dependency update
  * 1.0.5 A bug, that caused problems in aorist formation for compound verbs from βαίνω fixed.
  * 1.0.4 Added logic for multiple root formation in verbs on -άρω (σοκάρω, σοκαρίζω, σοκαρίσω), now the app will try to create also imperfect forms with a root on 'ιζ'. The Experiment with extending the core language check corpus failed miserably, as all the corpora I tried (even these from the EU) are unfortunately full of typos and orthographic errors, which, when used, introduced into the app huge problems. Next time I will try to use some NLTK magic and frequency lists to try them again.
```

### Comparing `modern_greek_inflexion-2.0.3/src/modern_greek_inflexion.egg-info/SOURCES.txt` & `modern_greek_inflexion-2.0.4/src/modern_greek_inflexion.egg-info/SOURCES.txt`

 * *Files identical despite different names*

