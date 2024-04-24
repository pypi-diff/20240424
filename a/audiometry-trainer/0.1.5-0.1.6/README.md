# Comparing `tmp/audiometry_trainer-0.1.5.tar.gz` & `tmp/audiometry_trainer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiometry_trainer-0.1.5.tar", last modified: Wed Apr 10 13:24:59 2024, max compression
+gzip compressed data, was "audiometry_trainer-0.1.6.tar", last modified: Wed Apr 24 18:44:34 2024, max compression
```

## Comparing `audiometry_trainer-0.1.5.tar` & `audiometry_trainer-0.1.6.tar`

### file list

```diff
@@ -1,325 +1,366 @@
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:59.130517 audiometry_trainer-0.1.5/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      109 2024-02-04 15:42:31.000000 audiometry_trainer-0.1.5/.gitignore
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1060 2024-02-05 09:52:05.000000 audiometry_trainer-0.1.5/.readthedocs.yaml
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 audiometry_trainer-0.1.5/COPYING.txt
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      965 2024-04-10 08:34:28.000000 audiometry_trainer-0.1.5/MANIFEST.in
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41838 2024-04-10 13:24:59.130517 audiometry_trainer-0.1.5/PKG-INFO
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      182 2024-04-10 08:51:32.000000 audiometry_trainer-0.1.5/README.md
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:56.550504 audiometry_trainer-0.1.5/audiometry_trainer/
--rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/__init__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7941 2024-04-10 13:20:51.000000 audiometry_trainer-0.1.5/audiometry_trainer/__main__.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      113 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/audiometry_trainer/_version_info.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    29257 2024-03-05 12:04:25.000000 audiometry_trainer-0.1.5/audiometry_trainer/acoust_values.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    10595 2024-02-25 20:55:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/audio_markers.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.570509 audiometry_trainer-0.1.5/audiometry_trainer/case_files/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3780 2024-04-08 10:56:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/danesh_et_al_2018.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      254 2024-04-08 10:56:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/danesh_et_al_2018_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      263 2024-04-09 18:17:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/danesh_et_al_2018_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3855 2024-04-08 10:56:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/hamad_et_al_2002_case_3.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      275 2024-04-08 10:56:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/hamad_et_al_2002_case_3_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      281 2024-04-09 18:18:37.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/hamad_et_al_2002_case_3_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4540 2024-04-08 10:57:00.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      245 2024-04-08 10:57:00.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      251 2024-04-09 18:19:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4781 2024-04-08 10:57:42.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      331 2024-04-09 18:20:57.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      339 2024-04-09 18:20:39.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5548 2024-04-08 10:57:49.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      334 2024-04-09 18:21:45.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      339 2024-04-09 18:21:36.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5224 2024-04-08 10:57:57.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      331 2024-04-09 18:21:52.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      338 2024-04-09 18:22:26.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4462 2024-04-08 10:58:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_2.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_2_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      315 2024-04-09 18:23:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_2_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4665 2024-04-08 10:58:12.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_3.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:12.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_3_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      315 2024-04-09 18:24:12.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_3_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5021 2024-04-08 10:58:19.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_4.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      308 2024-04-08 10:58:19.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_4_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      313 2024-04-09 18:24:46.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_4_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3814 2024-04-08 10:58:25.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_otosclerosis.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-08 10:58:25.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_otosclerosis_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      418 2024-04-09 18:25:40.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_otosclerosis_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4528 2024-04-08 10:58:31.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_1.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:31.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_1_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      313 2024-04-09 18:26:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_1_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4300 2024-04-08 10:58:37.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_2.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      302 2024-04-08 10:58:37.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_2_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      312 2024-04-09 18:27:19.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_2_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5539 2024-04-08 10:57:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_2.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      195 2024-04-08 10:57:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_2_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      203 2024-04-09 18:27:57.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_2_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4223 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_5.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      188 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_5_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_5_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5161 2024-04-08 10:57:25.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_6.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      188 2024-04-08 10:57:26.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_6_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-09 18:28:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_6_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5136 2024-04-08 10:57:34.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_7.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-08 10:57:34.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_7_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      204 2024-04-09 18:29:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_7_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4523 2024-04-08 10:58:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_2.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      176 2024-04-08 10:58:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_2_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      185 2024-04-09 18:30:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_2_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4168 2024-04-08 10:58:50.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_3.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      173 2024-04-08 10:58:50.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_3_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      184 2024-04-09 18:30:40.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_3_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4083 2024-04-08 10:59:01.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_6.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      168 2024-04-08 10:59:01.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_6_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      174 2024-04-09 18:31:12.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_6_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4548 2024-04-08 10:59:07.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_7.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      176 2024-04-08 10:59:07.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_7_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      185 2024-04-09 18:31:50.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_7_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3781 2024-04-08 10:59:13.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_8.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      172 2024-04-08 10:59:13.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_8_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      183 2024-04-09 18:32:24.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_8_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3873 2024-04-08 10:59:20.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_fig_5-8.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      186 2024-04-08 10:59:20.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_fig_5-8_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      197 2024-04-09 18:33:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_fig_5-8_info_fr.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4530 2024-04-08 18:23:23.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_2015_fig_6-6.csv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      231 2024-04-08 18:16:40.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_2015_fig_6-6_info.md
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      237 2024-04-09 18:33:37.000000 audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_2015_fig_6-6_info_fr.md
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2357 2024-02-28 11:04:46.000000 audiometry_trainer-0.1.5/audiometry_trainer/dialog_change_frequencies.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    25348 2024-02-13 16:28:50.000000 audiometry_trainer-0.1.5/audiometry_trainer/dialog_edit_preferences.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1862 2024-02-27 10:18:55.000000 audiometry_trainer-0.1.5/audiometry_trainer/dialog_set_value.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.662510 audiometry_trainer-0.1.5/audiometry_trainer/doc/
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/Makefile
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:56.202502 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.666509 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2024-04-10 13:24:15.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/.buildinfo
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.690510 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_images/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_images/audiometry_trainer.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    49340 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_images/logistic_psy.png
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.822510 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/generate_case.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1383 2024-04-07 17:43:49.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/installation.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/internals.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3940 2024-04-08 19:04:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/intro.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/masking.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/references.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/threshold_search.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/user_interface.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/virtual_listener.rst.txt
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.966511 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/basic.css
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:57.978511 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/css/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/css/badge_only.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/css/theme.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/doctools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/documentation_options.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/file.png
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.278513 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   683116 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   208512 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   714640 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   221928 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   693228 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   219592 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   661592 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   203936 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    52828 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    52532 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   165742 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   444379 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   165548 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    98024 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    77160 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/jquery.js
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.294513 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/js/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/js/theme.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/language_data.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/minus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/plus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/pygments.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/underscore.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    13380 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/generate_case.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4275 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/genindex.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     6967 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/index.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7450 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/installation.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7055 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/internals.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    12866 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/intro.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    23862 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/masking.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1097 2024-04-10 13:24:15.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/objects.inv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    10580 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/references.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4674 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/search.html
--rw-r--r--   0 sam       (1000) extdrive  (1777)    16747 2024-04-10 13:24:15.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/searchindex.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    10553 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/threshold_search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5310 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/user_interface.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    13604 2024-04-10 13:24:14.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/virtual_listener.html
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.314513 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/.buildinfo
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.354513 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    86961 2024-04-08 18:55:51.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.fr.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    50516 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/logistic_psy.fr.png
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.502514 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/generate_case.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/index.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1383 2024-04-07 17:43:49.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/installation.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/internals.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3940 2024-04-08 19:04:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/intro.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/masking.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/references.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/threshold_search.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/user_interface.rst.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/virtual_listener.rst.txt
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.634514 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/_sphinx_javascript_frameworks_compat.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     8133 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/base-stemmer.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/basic.css
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.642514 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/css/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/css/badge_only.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/css/theme.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/doctools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/documentation_options.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/file.png
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.870515 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   683116 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   208512 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   714640 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   221928 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   693228 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   219592 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   661592 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   203936 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    52828 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Bold.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    52532 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Regular.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   165742 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   444379 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   165548 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    98024 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    77160 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    42080 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/french-stemmer.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/jquery.js
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.890516 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/js/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/js/theme.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    17016 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/language_data.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/minus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/plus.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/pygments.css
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/searchtools.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/sphinx_highlight.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4311 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/translations.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/underscore.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    15081 2024-04-10 13:24:30.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/generate_case.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4395 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/genindex.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7198 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/index.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7747 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/installation.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     7266 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/internals.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    13909 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/intro.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    25598 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/masking.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1215 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/objects.inv
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    10763 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/references.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     4799 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/search.html
--rw-r--r--   0 sam       (1000) extdrive  (1777)    26400 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/searchindex.js
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    11539 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/threshold_search.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5527 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/user_interface.html
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14530 2024-04-10 13:24:32.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/virtual_listener.html
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.910516 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   388642 2024-04-10 13:24:23.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:58.910516 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex_fr/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)   400955 2024-04-10 13:24:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    86961 2024-04-08 18:55:51.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/audiometry_trainer.fr.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/audiometry_trainer.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     2743 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/conf.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/generate_case.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/index.rst
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1383 2024-04-07 17:43:49.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/installation.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/internals.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3940 2024-04-08 19:04:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/intro.rst
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:56.202502 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:56.206502 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:59.038516 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    12494 2024-04-07 11:37:06.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    15141 2024-04-07 11:37:06.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      582 2024-04-01 09:25:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     1060 2024-04-01 09:25:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2971 2024-04-07 08:32:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3727 2024-04-07 08:32:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      413 2024-04-01 09:30:24.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2148 2024-04-01 09:30:24.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     8802 2024-04-08 17:15:39.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9626 2024-04-08 17:15:39.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    16939 2024-04-08 18:45:29.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    22572 2024-04-08 18:45:29.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-08 18:25:24.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3738 2024-04-08 18:25:24.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     8125 2024-04-10 09:54:20.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     8986 2024-04-10 09:54:20.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      454 2024-04-05 16:38:12.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      824 2024-04-05 16:38:11.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    11689 2024-04-09 18:08:42.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.mo
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    14744 2024-04-09 18:08:42.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.po
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    50516 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/logistic_psy.fr.png
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    49340 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/logistic_psy.png
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/make.bat
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/masking.rst
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      344 2024-04-05 16:38:04.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/mkdoc.sh
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/references.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:44:53.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/requirements.txt
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/threshold_search.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/user_interface.rst
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.5/audiometry_trainer/doc/virtual_listener.rst
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8792 2024-03-03 09:53:17.000000 audiometry_trainer-0.1.5/audiometry_trainer/global_parameters.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     6708 2024-03-12 17:28:52.000000 audiometry_trainer-0.1.5/audiometry_trainer/hughson_westlake.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)   116146 2024-04-10 12:33:29.000000 audiometry_trainer-0.1.5/audiometry_trainer/main_window.py
--rw-rw-r--   0 sam       (1000) extdrive  (1777)       41 2024-04-10 13:24:25.000000 audiometry_trainer-0.1.5/audiometry_trainer/pyqtver.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)    27269 2023-08-12 08:58:20.000000 audiometry_trainer-0.1.5/audiometry_trainer/pysdt.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)  4097671 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/qrc_resources.py
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1772 2024-03-17 10:12:44.000000 audiometry_trainer-0.1.5/audiometry_trainer/utility_functions.py
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)    39142 2024-04-08 10:55:33.000000 audiometry_trainer-0.1.5/audiometry_trainer/window_generate_case.py
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:59.130517 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/
--rw-r--r--   0 sam       (1000) extdrive  (1777)    41838 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/PKG-INFO
--rw-r--r--   0 sam       (1000) extdrive  (1777)    15853 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)        1 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)       68 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/entry_points.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)      101 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/requires.txt
--rw-r--r--   0 sam       (1000) extdrive  (1777)       19 2024-04-10 13:24:56.000000 audiometry_trainer-0.1.5/audiometry_trainer.egg-info/top_level.txt
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:59.086517 audiometry_trainer-0.1.5/icons/
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      450 2024-02-04 12:03:41.000000 audiometry_trainer-0.1.5/icons/arrow-down-solid.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      445 2024-02-04 12:03:48.000000 audiometry_trainer-0.1.5/icons/arrow-up-solid.svg
--rw-r--r--   0 sam       (1000) extdrive  (1777)   129626 2024-04-09 21:21:24.000000 audiometry_trainer-0.1.5/icons/audiometry_trainer_icon.ico
--rw-rw-r--   0 sam       (1000) extdrive  (1777)     5335 2024-03-15 17:09:28.000000 audiometry_trainer-0.1.5/icons/audiometry_trainer_icon.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      786 2024-02-14 00:12:24.000000 audiometry_trainer-0.1.5/icons/dice-solid.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    16622 2011-11-01 10:05:06.000000 audiometry_trainer-0.1.5/icons/exit.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      623 2024-02-14 00:18:35.000000 audiometry_trainer-0.1.5/icons/folder-open-regular.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      538 2024-02-04 12:06:27.000000 audiometry_trainer-0.1.5/icons/headphones-solid.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7056 2012-08-13 00:59:09.000000 audiometry_trainer-0.1.5/icons/help-about.svgz
--rw-rwxr--   0 sam       (1000) extdrive  (1777)   679822 2015-11-04 09:40:24.000000 audiometry_trainer-0.1.5/icons/help-contents.svgz
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)   255671 2012-08-13 01:04:33.000000 audiometry_trainer-0.1.5/icons/help-contextual.svgz
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    11683 2024-04-01 18:29:50.000000 audiometry_trainer-0.1.5/icons/insert.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      468 2024-02-04 12:05:03.000000 audiometry_trainer-0.1.5/icons/lock-open-solid.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      443 2024-02-04 12:04:56.000000 audiometry_trainer-0.1.5/icons/lock-solid.svg
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      527 2024-02-04 12:05:24.000000 audiometry_trainer-0.1.5/icons/mask-solid.svg
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)    10662 2012-08-13 00:56:47.000000 audiometry_trainer-0.1.5/icons/preferences-other.svgz
--rw-rw-r--   0 sam       (1000) extdrive  (1777)      592 2024-02-04 12:07:12.000000 audiometry_trainer-0.1.5/icons/skull-solid.svg
-drwxr-sr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-10 13:24:59.130517 audiometry_trainer-0.1.5/prep-release/
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      586 2024-02-28 11:52:04.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer.pro
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    48315 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_el.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    48315 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_GB.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    48315 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_US.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    48315 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_es.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    52717 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_fr.ts
--rw-rw-r--   0 sam       (1000) extdrive  (1777)    48338 2024-04-10 13:23:44.000000 audiometry_trainer-0.1.5/prep-release/audiometry_trainer_it.ts
--rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/prep-release/minor_minor_number.txt
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      187 2024-01-28 08:31:37.000000 audiometry_trainer-0.1.5/prep-release/mkupdate_pyqt5.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)      681 2024-02-28 11:50:55.000000 audiometry_trainer-0.1.5/prep-release/mkupdate_pyqt6.sh
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      219 2024-02-20 09:58:08.000000 audiometry_trainer-0.1.5/prep-release/pypi_build.sh
--rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3929 2024-04-10 13:23:35.000000 audiometry_trainer-0.1.5/prep-release/release.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      946 2024-01-28 08:29:08.000000 audiometry_trainer-0.1.5/prep-release/switch_pyqt5.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      946 2024-01-28 08:29:19.000000 audiometry_trainer-0.1.5/prep-release/switch_pyqt6.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     4012 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/prep-release/win_audiometry_trainer.iss
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      219 2024-02-19 16:03:44.000000 audiometry_trainer-0.1.5/prep-release/win_installer_readme.md
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      152 2024-02-19 11:39:38.000000 audiometry_trainer-0.1.5/prep-release/win_launch_iss_compiler.bat
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      128 2024-02-19 15:32:46.000000 audiometry_trainer-0.1.5/prep-release/win_launch_iss_compiler.sh
--rwxrwxr-x   0 sam       (1000) extdrive  (1777)      796 2024-02-18 21:59:33.000000 audiometry_trainer-0.1.5/prep-release/winbuild.py
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1337 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/pyproject.toml
--rw-rwxr--   0 sam       (1000) extdrive  (1777)     1328 2024-04-01 18:27:56.000000 audiometry_trainer-0.1.5/resources.qrc
--rw-r--r--   0 sam       (1000) extdrive  (1777)       38 2024-04-10 13:24:59.130517 audiometry_trainer-0.1.5/setup.cfg
--rw-rwxr--   0 sam       (1000) extdrive  (1777)      962 2024-04-10 13:22:55.000000 audiometry_trainer-0.1.5/setup_cx.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.310624 audiometry_trainer-0.1.6/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      109 2024-02-04 15:42:31.000000 audiometry_trainer-0.1.6/.gitignore
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1060 2024-02-05 09:52:05.000000 audiometry_trainer-0.1.6/.readthedocs.yaml
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    35147 2010-06-04 09:15:48.000000 audiometry_trainer-0.1.6/COPYING.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      626 2024-04-24 18:25:47.000000 audiometry_trainer-0.1.6/CREDITS.txt
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      965 2024-04-10 08:34:28.000000 audiometry_trainer-0.1.6/MANIFEST.in
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41838 2024-04-24 18:44:34.310624 audiometry_trainer-0.1.6/PKG-INFO
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      182 2024-04-10 08:51:32.000000 audiometry_trainer-0.1.6/README.md
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:32.836379 audiometry_trainer-0.1.6/audiometry_trainer/
+-rwxrwsrwx   0 sam       (1000) extdrive  (1777)        0 2008-10-28 02:30:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/__init__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     7941 2024-04-10 13:20:51.000000 audiometry_trainer-0.1.6/audiometry_trainer/__main__.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      113 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/audiometry_trainer/_version_info.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    29257 2024-03-05 12:04:25.000000 audiometry_trainer-0.1.6/audiometry_trainer/acoust_values.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    10595 2024-02-25 20:55:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/audio_markers.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.336462 audiometry_trainer-0.1.6/audiometry_trainer/case_files/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3780 2024-04-08 10:56:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/danesh_et_al_2018.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      254 2024-04-08 10:56:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/danesh_et_al_2018_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      263 2024-04-09 18:17:32.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/danesh_et_al_2018_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3855 2024-04-08 10:56:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/hamad_et_al_2002_case_3.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      275 2024-04-08 10:56:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/hamad_et_al_2002_case_3_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      281 2024-04-09 18:18:37.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/hamad_et_al_2002_case_3_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4540 2024-04-08 10:57:00.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      245 2024-04-08 10:57:00.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      251 2024-04-09 18:19:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4664 2024-04-10 18:57:49.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/lee_et_al_2021_case_1.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      317 2024-04-10 18:57:49.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/lee_et_al_2021_case_1_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      317 2024-04-10 18:57:49.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/lee_et_al_2021_case_1_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5660 2024-04-11 11:00:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/manzari_2010.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      359 2024-04-11 11:00:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/manzari_2010_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      392 2024-04-11 11:00:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/manzari_2010_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4781 2024-04-08 10:57:42.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      331 2024-04-09 18:20:57.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      339 2024-04-09 18:20:39.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5548 2024-04-08 10:57:49.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      334 2024-04-09 18:21:45.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      339 2024-04-09 18:21:36.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5224 2024-04-08 10:57:57.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      331 2024-04-09 18:21:52.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      338 2024-04-09 18:22:26.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4462 2024-04-08 10:58:04.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_2.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:04.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_2_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      315 2024-04-09 18:23:32.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_2_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4665 2024-04-08 10:58:12.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_3.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:12.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_3_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      315 2024-04-09 18:24:12.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_3_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5021 2024-04-08 10:58:19.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_4.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      308 2024-04-08 10:58:19.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_4_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      313 2024-04-09 18:24:46.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_4_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3814 2024-04-08 10:58:25.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_otosclerosis.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-08 10:58:25.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_otosclerosis_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      418 2024-04-09 18:25:40.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_otosclerosis_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4528 2024-04-08 10:58:31.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_1.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      305 2024-04-08 10:58:31.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_1_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      313 2024-04-09 18:26:44.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_1_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4300 2024-04-08 10:58:37.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_2.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      302 2024-04-08 10:58:37.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_2_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      312 2024-04-09 18:27:19.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_2_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5539 2024-04-08 10:57:11.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_2.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      195 2024-04-08 10:57:11.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_2_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      203 2024-04-09 18:27:57.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_2_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4223 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_5.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      188 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_5_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-08 10:57:17.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_5_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5161 2024-04-08 10:57:25.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_6.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      188 2024-04-08 10:57:26.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_6_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-09 18:28:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_6_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5136 2024-04-08 10:57:34.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_7.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      193 2024-04-08 10:57:34.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_7_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      204 2024-04-09 18:29:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_7_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4523 2024-04-08 10:58:44.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_2.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      176 2024-04-08 10:58:44.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_2_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      185 2024-04-09 18:30:04.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_2_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4168 2024-04-08 10:58:50.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_3.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      173 2024-04-08 10:58:50.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_3_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      184 2024-04-09 18:30:40.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_3_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4083 2024-04-08 10:59:01.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_6.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      168 2024-04-08 10:59:01.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_6_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      174 2024-04-09 18:31:12.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_6_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4548 2024-04-08 10:59:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_7.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      176 2024-04-08 10:59:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_7_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      185 2024-04-09 18:31:50.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_7_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3781 2024-04-08 10:59:13.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_8.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      172 2024-04-08 10:59:13.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_8_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      183 2024-04-09 18:32:24.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_8_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3873 2024-04-08 10:59:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_fig_5-8.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      186 2024-04-08 10:59:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_fig_5-8_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      197 2024-04-09 18:33:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_fig_5-8_info_fr.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4530 2024-04-08 18:23:23.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_2015_fig_6-6.csv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      231 2024-04-08 18:16:40.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_2015_fig_6-6_info.md
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      237 2024-04-09 18:33:37.000000 audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_2015_fig_6-6_info_fr.md
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     2357 2024-02-28 11:04:46.000000 audiometry_trainer-0.1.6/audiometry_trainer/dialog_change_frequencies.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)    25348 2024-02-13 16:28:50.000000 audiometry_trainer-0.1.6/audiometry_trainer/dialog_edit_preferences.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1862 2024-02-27 10:18:55.000000 audiometry_trainer-0.1.6/audiometry_trainer/dialog_set_value.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.363467 audiometry_trainer-0.1.6/audiometry_trainer/doc/
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      634 2023-02-23 15:00:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/Makefile
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:32.802373 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.368467 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.369468 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/audiometry_trainer.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7249 2024-04-12 09:10:01.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/file_menu.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    49340 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/logistic_psy.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.512492 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/generate_case.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1539 2024-04-12 09:39:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/installation.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/internals.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4186 2024-04-24 18:39:47.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/intro.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/masking.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/references.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/threshold_search.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/user_interface.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/virtual_listener.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.574502 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/basic.css
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.588504 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/css/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/css/badge_only.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/css/theme.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/doctools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.799539 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   683116 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   208512 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   714640 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   221928 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   693228 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   219592 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   661592 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   203936 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    52828 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    52532 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   165742 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   444379 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   165548 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    98024 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    77160 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.799539 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/js/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/js/theme.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4758 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/language_data.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/minus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/plus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/pygments.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/underscore.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    13380 2024-04-24 18:44:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/generate_case.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4275 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/genindex.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6967 2024-04-24 18:44:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/index.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7648 2024-04-24 18:44:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/installation.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7055 2024-04-24 18:44:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/internals.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    13503 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/intro.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    23862 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/masking.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1115 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/objects.inv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    10580 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/references.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4674 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    16882 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/searchindex.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    10553 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/threshold_search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5310 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/user_interface.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    13604 2024-04-24 18:44:09.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/virtual_listener.html
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.823543 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      230 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/.buildinfo
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.854549 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    86961 2024-04-08 18:55:51.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.fr.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8078 2024-04-12 09:19:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/file_menu.fr.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7249 2024-04-12 09:10:01.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/file_menu.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    50516 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/logistic_psy.fr.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:33.979569 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/generate_case.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/index.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1539 2024-04-12 09:39:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/installation.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/internals.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4186 2024-04-24 18:39:47.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/intro.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/masking.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/references.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/threshold_search.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/user_interface.rst.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/virtual_listener.rst.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.043580 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4418 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/_sphinx_javascript_frameworks_compat.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8133 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/base-stemmer.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14810 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/basic.css
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.064583 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/css/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3303 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/css/badge_only.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   138354 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/css/theme.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4472 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/doctools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      420 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/documentation_options.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      286 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/file.png
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.227611 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   683116 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   208512 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   714640 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   221928 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   693228 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   219592 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   661592 2014-02-27 03:42:28.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   203936 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    52828 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Bold.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    52532 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Regular.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   165742 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   444379 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   165548 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    98024 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    77160 2016-10-24 15:52:54.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    42080 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/french-stemmer.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   289782 2022-08-29 08:27:59.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/jquery.js
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.227611 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/js/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9478 2023-02-08 21:25:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/js/theme.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    17016 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/language_data.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/minus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       90 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/plus.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4819 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/pygments.css
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    18747 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/searchtools.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5097 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/sphinx_highlight.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4311 2023-03-29 08:31:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/translations.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    68416 2022-06-02 12:39:04.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/underscore.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    15081 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/generate_case.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4395 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/genindex.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7198 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/index.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7955 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/installation.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7266 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/internals.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14571 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/intro.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    25598 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/masking.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1234 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/objects.inv
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    10763 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/references.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4799 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    26597 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/searchindex.js
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11539 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/threshold_search.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5527 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/user_interface.html
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14530 2024-04-24 18:44:14.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/virtual_listener.html
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.228611 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   396555 2024-04-24 18:44:11.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.228611 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex_fr/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)   410492 2024-04-24 18:44:17.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    86961 2024-04-08 18:55:51.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/audiometry_trainer.fr.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    84996 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/audiometry_trainer.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     2743 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/conf.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8078 2024-04-12 09:19:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/file_menu.fr.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     7249 2024-04-12 09:10:01.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/file_menu.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5478 2024-04-07 10:56:43.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/generate_case.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      608 2024-04-03 10:32:00.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/index.rst
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1539 2024-04-12 09:39:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/installation.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1241 2024-03-30 12:44:16.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/internals.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4186 2024-04-24 18:39:47.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/intro.rst
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:32.803373 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:32.803373 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.235612 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    12494 2024-04-07 11:37:06.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    15141 2024-04-07 11:37:06.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      582 2024-04-01 09:25:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1060 2024-04-01 09:25:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3307 2024-04-12 09:39:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4108 2024-04-12 09:39:27.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      413 2024-04-01 09:30:24.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2148 2024-04-01 09:30:24.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9157 2024-04-24 18:40:35.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11775 2024-04-24 18:40:35.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    16939 2024-04-08 18:45:29.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    22572 2024-04-08 18:45:29.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-08 18:25:24.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3738 2024-04-08 18:25:24.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8125 2024-04-10 09:54:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8986 2024-04-10 09:54:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      454 2024-04-05 16:38:12.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      824 2024-04-05 16:38:11.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11689 2024-04-09 18:08:42.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    14744 2024-04-09 18:08:42.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.po
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:32.803373 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.241613 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/generate_case.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6712 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/generate_case.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      567 2024-04-14 08:38:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/index.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1045 2024-04-14 08:38:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/index.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      407 2024-04-17 07:11:03.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/installation.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2557 2024-04-17 07:11:03.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/installation.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/internals.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2134 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/internals.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5874 2024-04-24 18:40:58.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/intro.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     8158 2024-04-24 18:40:58.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/intro.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/masking.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    13713 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/masking.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/references.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3721 2024-04-14 08:33:21.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/references.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/threshold_search.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4748 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/threshold_search.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/user_interface.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      794 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/user_interface.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      441 2024-04-14 08:33:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/virtual_listener.mo
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     6891 2024-04-14 08:33:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/it/LC_MESSAGES/virtual_listener.po
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    50516 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/logistic_psy.fr.png
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    49340 2024-04-09 17:41:45.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/logistic_psy.png
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      795 2023-02-23 15:00:48.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/make.bat
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     9891 2024-04-08 17:52:36.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/masking.rst
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      586 2024-04-14 08:43:38.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/mkdoc.sh
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2835 2024-04-10 09:21:56.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/references.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       18 2024-02-05 09:44:53.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/requirements.txt
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     3613 2024-04-07 22:58:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/threshold_search.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      143 2024-04-05 15:55:02.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/user_interface.rst
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     5570 2024-04-09 18:06:18.000000 audiometry_trainer-0.1.6/audiometry_trainer/doc/virtual_listener.rst
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     8792 2024-03-03 09:53:17.000000 audiometry_trainer-0.1.6/audiometry_trainer/global_parameters.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     6708 2024-03-12 17:28:52.000000 audiometry_trainer-0.1.6/audiometry_trainer/hughson_westlake.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)   117452 2024-04-24 18:30:07.000000 audiometry_trainer-0.1.6/audiometry_trainer/main_window.py
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       41 2024-04-24 18:44:06.000000 audiometry_trainer-0.1.6/audiometry_trainer/pyqtver.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)    27269 2023-08-12 08:58:20.000000 audiometry_trainer-0.1.6/audiometry_trainer/pysdt.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)   185291 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/audiometry_trainer/qrc_resources.py
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     1772 2024-03-17 10:12:44.000000 audiometry_trainer-0.1.6/audiometry_trainer/utility_functions.py
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)    39251 2024-04-13 07:35:10.000000 audiometry_trainer-0.1.6/audiometry_trainer/window_generate_case.py
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.308624 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    41838 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 sam       (1000) extdrive  (1777)    17841 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 sam       (1000) extdrive  (1777)        1 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 sam       (1000) extdrive  (1777)       68 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/entry_points.txt
+-rw-r--r--   0 sam       (1000) extdrive  (1777)      101 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/requires.txt
+-rw-r--r--   0 sam       (1000) extdrive  (1777)       19 2024-04-24 18:44:32.000000 audiometry_trainer-0.1.6/audiometry_trainer.egg-info/top_level.txt
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.271618 audiometry_trainer-0.1.6/icons/
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      450 2024-02-04 12:03:41.000000 audiometry_trainer-0.1.6/icons/arrow-down-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      445 2024-02-04 12:03:48.000000 audiometry_trainer-0.1.6/icons/arrow-up-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     4286 2024-04-13 06:38:09.000000 audiometry_trainer-0.1.6/icons/audiometry_trainer_icon.ico
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2395 2024-04-12 08:11:12.000000 audiometry_trainer-0.1.6/icons/audiometry_trainer_icon.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      508 2024-04-13 07:08:22.000000 audiometry_trainer-0.1.6/icons/book-bookmark-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      594 2024-04-13 07:08:05.000000 audiometry_trainer-0.1.6/icons/book-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      483 2024-04-13 06:49:47.000000 audiometry_trainer-0.1.6/icons/circle-info-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      786 2024-02-14 00:12:24.000000 audiometry_trainer-0.1.6/icons/dice-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     1144 2024-04-24 18:24:46.000000 audiometry_trainer-0.1.6/icons/film-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      527 2024-04-13 07:33:48.000000 audiometry_trainer-0.1.6/icons/floppy-disk-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      623 2024-02-14 00:18:35.000000 audiometry_trainer-0.1.6/icons/folder-open-regular.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2204 2024-04-11 11:05:41.000000 audiometry_trainer-0.1.6/icons/gears-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      538 2024-02-04 12:06:27.000000 audiometry_trainer-0.1.6/icons/headphones-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    11683 2024-04-01 18:29:50.000000 audiometry_trainer-0.1.6/icons/insert.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      468 2024-02-04 12:05:03.000000 audiometry_trainer-0.1.6/icons/lock-open-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      443 2024-02-04 12:04:56.000000 audiometry_trainer-0.1.6/icons/lock-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)     2017 2024-04-13 07:25:09.000000 audiometry_trainer-0.1.6/icons/mask-solid-off.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      527 2024-02-04 12:05:24.000000 audiometry_trainer-0.1.6/icons/mask-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      903 2024-04-13 07:29:32.000000 audiometry_trainer-0.1.6/icons/person-running-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      595 2024-04-13 06:49:08.000000 audiometry_trainer-0.1.6/icons/question-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      680 2024-04-11 11:10:14.000000 audiometry_trainer-0.1.6/icons/right-from-bracket-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      845 2024-04-13 06:58:05.000000 audiometry_trainer-0.1.6/icons/robot-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      592 2024-02-04 12:07:12.000000 audiometry_trainer-0.1.6/icons/skull-solid.svg
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)      958 2024-04-13 06:40:39.000000 audiometry_trainer-0.1.6/icons/sliders-solid.svg
+drwxrwsr-x   0 sam       (1000) extdrive  (1777)        0 2024-04-24 18:44:34.308624 audiometry_trainer-0.1.6/prep-release/
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      586 2024-02-28 11:52:04.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer.pro
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    48887 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_el.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    48887 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_GB.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    48887 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_US.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    48887 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_es.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    53298 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_fr.ts
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)    50730 2024-04-24 18:43:40.000000 audiometry_trainer-0.1.6/prep-release/audiometry_trainer_it.ts
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)        1 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/prep-release/minor_minor_number.txt
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      187 2024-01-28 08:31:37.000000 audiometry_trainer-0.1.6/prep-release/mkupdate_pyqt5.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)      681 2024-02-28 11:50:55.000000 audiometry_trainer-0.1.6/prep-release/mkupdate_pyqt6.sh
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      219 2024-02-20 09:58:08.000000 audiometry_trainer-0.1.6/prep-release/pypi_build.sh
+-rwxrwxrwx   0 sam       (1000) extdrive  (1777)     3929 2024-04-10 13:23:35.000000 audiometry_trainer-0.1.6/prep-release/release.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      946 2024-01-28 08:29:08.000000 audiometry_trainer-0.1.6/prep-release/switch_pyqt5.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      946 2024-01-28 08:29:19.000000 audiometry_trainer-0.1.6/prep-release/switch_pyqt6.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     4012 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/prep-release/win_audiometry_trainer.iss
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      219 2024-02-19 16:03:44.000000 audiometry_trainer-0.1.6/prep-release/win_installer_readme.md
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      152 2024-02-19 11:39:38.000000 audiometry_trainer-0.1.6/prep-release/win_launch_iss_compiler.bat
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      128 2024-02-19 15:32:46.000000 audiometry_trainer-0.1.6/prep-release/win_launch_iss_compiler.sh
+-rwxrwxr-x   0 sam       (1000) extdrive  (1777)      796 2024-02-18 21:59:33.000000 audiometry_trainer-0.1.6/prep-release/winbuild.py
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1337 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/pyproject.toml
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)     1797 2024-04-24 18:25:32.000000 audiometry_trainer-0.1.6/resources.qrc
+-rw-rw-r--   0 sam       (1000) extdrive  (1777)       38 2024-04-24 18:44:34.310624 audiometry_trainer-0.1.6/setup.cfg
+-rw-rwxr--   0 sam       (1000) extdrive  (1777)      962 2024-04-24 18:42:46.000000 audiometry_trainer-0.1.6/setup_cx.py
```

### Comparing `audiometry_trainer-0.1.5/.readthedocs.yaml` & `audiometry_trainer-0.1.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/COPYING.txt` & `audiometry_trainer-0.1.6/COPYING.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/MANIFEST.in` & `audiometry_trainer-0.1.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/PKG-INFO` & `audiometry_trainer-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiometry_trainer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Clinical audiometry simulator
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/__main__.py` & `audiometry_trainer-0.1.6/audiometry_trainer/__main__.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/acoust_values.py` & `audiometry_trainer-0.1.6/audiometry_trainer/acoust_values.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/audio_markers.py` & `audiometry_trainer-0.1.6/audiometry_trainer/audio_markers.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/danesh_et_al_2018.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/danesh_et_al_2018.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/hamad_et_al_2002_case_3.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/hamad_et_al_2002_case_3.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_2.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_2.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_3.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_3.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_case_4.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_case_4.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/stat_pearls_otosclerosis.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/stat_pearls_otosclerosis.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_1.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_1.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/suryakant_et_al_2021_case_2.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/suryakant_et_al_2021_case_2.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_2.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_2.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_5.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_5.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_6.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_6.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/valente_and_valente_2020_case_7.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/valente_and_valente_2020_case_7.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_2.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_2.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_3.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_3.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_6.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_6.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_7.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_7.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_case_8.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_case_8.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_1997_fig_5-8.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_1997_fig_5-8.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/case_files/yacullo_2015_fig_6-6.csv` & `audiometry_trainer-0.1.6/audiometry_trainer/case_files/yacullo_2015_fig_6-6.csv`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/dialog_change_frequencies.py` & `audiometry_trainer-0.1.6/audiometry_trainer/dialog_change_frequencies.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/dialog_edit_preferences.py` & `audiometry_trainer-0.1.6/audiometry_trainer/dialog_edit_preferences.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/dialog_set_value.py` & `audiometry_trainer-0.1.6/audiometry_trainer/dialog_set_value.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/Makefile` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/Makefile`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_images/audiometry_trainer.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/audiometry_trainer.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_images/logistic_psy.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_images/logistic_psy.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/generate_case.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/generate_case.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/index.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/installation.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/installation.rst.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .. _sec-installation:
 
 ************
 Installation
 ************
 
-``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. A dedicated installer is provided for Windows. On Linux and Mac (and Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
+``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. For Windows, a dedicated installer can be downloaded from `SourceForge <https://sourceforge.net/projects/audiometry-trainer/files/>`_.
+
+On Linux and Mac (but also on Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
 
 .. code-block:: bash
 
 		pip install audiometry-trainer
 
 ``audiometry_trainer`` depends on a few Python modules including:
 
@@ -20,14 +22,14 @@
 
 depending on your Python distribution you may want to install these dependecies before installing ``audiometry_trainer`` via ``pip`` (e.g. through ``conda`` if you're using the Anaconda Python distribution, or through your Linux distribution package manager if you're using the Python installation that comes with your Linux distribution), otherwise ``pip`` will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:
 
 .. code-block:: bash
 
 	audiometry_trainer
 
-You need to ensure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
+If you use multiple Python installations/environnments, you need to make sure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/internals.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/internals.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/intro.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/intro.rst.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 .. _sec-intro:
 
 *************
 Introduction
 *************
 
-``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``.
+``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``. Online video tutorials are available on `Youtube. <https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4>`_
 
 .. _fig-audiometry_trainer_screenshot:
 
 .. figure:: audiometry_trainer.png
    :scale: 50%
    :alt: Screenshot of the ``audiometry_trainer`` interface
 
    Screenshot of the ``audiometry_trainer`` interface
 
-At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``). The ``S`` marker in the audiogram window shows the current stimulus level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrows to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
+At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``).
+
+.. _fig-file_menu:
+
+.. figure:: file_menu.png
+   :scale: 100%
+   :alt: File menu
+
+   File menu
+   
+The ``S`` marker in the audiogram window shows the current stimulus frequency and level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrow keys to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
 
 You can compare the thresholds that you've estimated with the actual expected thresholds by using the ``Show actual thresholds`` checkboxes at the bottom of the left panel. Virtual patients are modeled via psychometric functions and the "actual" thresholds are computed via Monte Carlo simulations: they are the median thresholds obtained over a large number of simulations; 95% confidence intervals can be shown by checking the ``CI`` checkboxes.
 
-You can move from right to left era and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the left panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
+You can move from right to left ear and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the right panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
 
 A detailed description of all the features of ``audiometry_trainer`` will be given in the next sections. Section :ref:`sec-installation` tells how to obtain and install ``audiometry_trainer``. Sections :ref:`sec-threshold_search` and :ref:`sec-masking` explain how to perform a threshold search and how to use masking, respectively.
 
 ``audiometry_trainer`` uses psychometric functions to model virtual patient responses. Responses are not deterministic (always yes/no above/below a given stimulus level) but probabilistic, with the probability of a response increasing with the stimulus level. This adds realism to the software because in real life the responses of patients are not deterministic. Section :ref:`sec-virtual_listener` details the psychometric function model used by ``audiometry_trainer``.
 
 ``audiometry_trainer`` allows you to create and use your own case files. This functionality can be accessed via the ``Generate case`` button under the ``File menu`` and will be described in detail in Section :ref:`sec-generate_case`. Some knowledge of the psychometric function model used by ``audiometry_trainer`` will be needed to create your own case files.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/masking.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/masking.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/references.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/references.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/threshold_search.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/threshold_search.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_sources/virtual_listener.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_sources/virtual_listener.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/basic.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/css/badge_only.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/css/theme.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/doctools.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/RobotoSlab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.eot` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.svg` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/jquery.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/js/theme.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/language_data.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/pygments.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/searchtools.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/sphinx_highlight.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/_static/underscore.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/generate_case.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/generate_case.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Generating case files &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Generating case files &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/genindex.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Index &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/index.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Welcome to audiometry_trainer’s documentation! &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Welcome to audiometry_trainer’s documentation! &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/installation.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/installation.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 <!DOCTYPE html>
-<html class="writer-html5" lang="en" >
+<html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Installation &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
+        <script src="_static/translations.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Search" href="search.html" />
-    <link rel="next" title="Threshold search" href="threshold_search.html" />
+    <link rel="search" title="Recherche" href="search.html" />
+    <link rel="next" title="Recherche du seuil" href="threshold_search.html" />
     <link rel="prev" title="Introduction" href="intro.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
@@ -29,35 +30,35 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
+    <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Table des matières :</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="intro.html">Introduction</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="threshold_search.html">Threshold search</a></li>
-<li class="toctree-l1"><a class="reference internal" href="masking.html">Masking</a></li>
-<li class="toctree-l1"><a class="reference internal" href="virtual_listener.html">Virtual listener</a></li>
-<li class="toctree-l1"><a class="reference internal" href="generate_case.html">Generating case files</a></li>
-<li class="toctree-l1"><a class="reference internal" href="user_interface.html">User interface</a></li>
-<li class="toctree-l1"><a class="reference internal" href="internals.html">Internals</a></li>
-<li class="toctree-l1"><a class="reference internal" href="references.html">References</a></li>
+<li class="toctree-l1"><a class="reference internal" href="threshold_search.html">Recherche du seuil</a></li>
+<li class="toctree-l1"><a class="reference internal" href="masking.html">Masquage</a></li>
+<li class="toctree-l1"><a class="reference internal" href="virtual_listener.html">Sujet virtuel</a></li>
+<li class="toctree-l1"><a class="reference internal" href="generate_case.html">Générer des fichiers de cas</a></li>
+<li class="toctree-l1"><a class="reference internal" href="user_interface.html">Interface utilisateur</a></li>
+<li class="toctree-l1"><a class="reference internal" href="internals.html">Fonctionnement interne</a></li>
+<li class="toctree-l1"><a class="reference internal" href="references.html">Références</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -68,62 +69,63 @@
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
       <li class="breadcrumb-item active">Installation</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/installation.rst.txt" rel="nofollow"> View page source</a>
+            <a href="_sources/installation.rst.txt" rel="nofollow"> Afficher la source de la page</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="installation">
-<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Permalink to this heading"></a></h1>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. A dedicated installer is provided for Windows. On Linux and Mac (and Windows if you do not wish to use the dedicated installer) <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, which is written in Python, can be installed via the Python package installer <code class="docutils literal notranslate"><span class="pre">pip</span></code>:</p>
+<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Lien permanent vers cette rubrique"></a></h1>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> a été installé et utilisé avec succès sur Linux et Windows. Il devrait aussi marcher sur des ordinateurs Mac, mais cela n’a pas été testé. Pour Windows, vous pouvez télécharger un programme d’installation dédié sur <a class="reference external" href="https://sourceforge.net/projects/audiometry-trainer/files/">SourceForge</a>.</p>
+<p>Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser le programme d’installation dédié) <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, qui est écrit en Python, peut être installé à travers <code class="docutils literal notranslate"><span class="pre">pip</span></code>:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>pip<span class="w"> </span>install<span class="w"> </span>audiometry-trainer
 </pre></div>
 </div>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> depends on a few Python modules including:</p>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> dépend d’un petit nombre de modules Python y compris :</p>
 <blockquote>
 <div><ul class="simple">
 <li><p>PyQt5</p></li>
 <li><p>numpy</p></li>
 <li><p>scipy</p></li>
 <li><p>matplotlib</p></li>
 <li><p>pandas</p></li>
 </ul>
 </div></blockquote>
-<p>depending on your Python distribution you may want to install these dependecies before installing <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> via <code class="docutils literal notranslate"><span class="pre">pip</span></code> (e.g. through <code class="docutils literal notranslate"><span class="pre">conda</span></code> if you’re using the Anaconda Python distribution, or through your Linux distribution package manager if you’re using the Python installation that comes with your Linux distribution), otherwise <code class="docutils literal notranslate"><span class="pre">pip</span></code> will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:</p>
+<p>selon votre distribution il pourrait être souhaitable d’installer ces dépendances avant d’installer <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> à travers <code class="docutils literal notranslate"><span class="pre">pip</span></code> (par exemple à travers <code class="docutils literal notranslate"><span class="pre">conda</span></code> si vous utilisez la distribution de Python Anaconda, ou à travers votre gestionnaire de paquets de Linux si vous utilisez l’installation de Python de votre distribution Linux), sinon <code class="docutils literal notranslate"><span class="pre">pip</span></code> essayera de télécharger et installer ces dépendances de façon automatique. Si le programme est installé avec succès vous devriez pouvoir le lancer depuis un terminal bash/DOS avec la commande :</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>audiometry_trainer
 </pre></div>
 </div>
-<p>You need to ensure that the Python environment you’re using when you call the above command matches the one you used when you installed the application.</p>
+<p>Si vous utilisez plusieurs installations/environnements de Python, vous devez vous assurer que l’environnement de Python que vous employez quand vous utilisez la commande ci-dessus correspond à celui que vous aviez utilisé lors de l’installation de l’application.</p>
 </section>
 
 
            </div>
           </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
-        <a href="intro.html" class="btn btn-neutral float-left" title="Introduction" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
-        <a href="threshold_search.html" class="btn btn-neutral float-right" title="Threshold search" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Pied de page">
+        <a href="intro.html" class="btn btn-neutral float-left" title="Introduction" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Précédent</a>
+        <a href="threshold_search.html" class="btn btn-neutral float-right" title="Recherche du seuil" accesskey="n" rel="next">Suivant <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023-2024, Samuele Carcagno.</p>
   </div>
 
-  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
-    provided by <a href="https://readthedocs.org">Read the Docs</a>.
+  Compilé avec <a href="https://www.sphinx-doc.org/">Sphinx</a> en utilisant un
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">thème</a>
+    fourni par <a href="https://readthedocs.org">Read the Docs</a>.
    
 
 </footer>
         </div>
       </div>
     </section>
   </div>
```

#### html2text {}

```diff
@@ -1,44 +1,49 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
-Contents:
+Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
-    * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
-    * _M_a_s_k_i_n_g
-    * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
-    * _G_e_n_e_r_a_t_i_n_g_ _c_a_s_e_ _f_i_l_e_s
-    * _U_s_e_r_ _i_n_t_e_r_f_a_c_e
-    * _I_n_t_e_r_n_a_l_s
-    * _R_e_f_e_r_e_n_c_e_s
+    * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
+    * _M_a_s_q_u_a_g_e
+    * _S_u_j_e_t_ _v_i_r_t_u_e_l
+    * _G_é_n_é_r_e_r_ _d_e_s_ _f_i_c_h_i_e_r_s_ _d_e_ _c_a_s
+    * _I_n_t_e_r_f_a_c_e_ _u_t_i_l_i_s_a_t_e_u_r
+    * _F_o_n_c_t_i_o_n_n_e_m_e_n_t_ _i_n_t_e_r_n_e
+    * _R_é_f_é_r_e_n_c_e_s
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
     * Installation
-    * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
+    * _A_f_f_i_c_h_e_r_ _l_a_ _s_o_u_r_c_e_ _d_e_ _l_a_ _p_a_g_e
 ===============================================================================
 ************ IInnssttaallllaattiioonn_? ************
-audiometry_trainer has been successfully installed and used on Linux and
-Windows. It should also work on Mac platforms, but this has not been tested. A
-dedicated installer is provided for Windows. On Linux and Mac (and Windows if
-you do not wish to use the dedicated installer) audiometry_trainer, which is
-written in Python, can be installed via the Python package installer pip:
+audiometry_trainer a été installé et utilisé avec succès sur Linux et Windows.
+Il devrait aussi marcher sur des ordinateurs Mac, mais cela n’a pas été testé.
+Pour Windows, vous pouvez télécharger un programme d’installation dédié sur
+_S_o_u_r_c_e_F_o_r_g_e.
+Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser le
+programme d’installation dédié) audiometry_trainer, qui est écrit en Python,
+peut être installé à travers pip:
 pip install audiometry-trainer
-audiometry_trainer depends on a few Python modules including:
+audiometry_trainer dépend d’un petit nombre de modules Python y compris :
          * PyQt5
          * numpy
          * scipy
          * matplotlib
          * pandas
-depending on your Python distribution you may want to install these dependecies
-before installing audiometry_trainer via pip (e.g. through conda if you’re
-using the Anaconda Python distribution, or through your Linux distribution
-package manager if you’re using the Python installation that comes with your
-Linux distribution), otherwise pip will attempt to automatically pull in and
-install these dependencies. If the program is successfully installed you should
-be able to start it from a bash/DOS terminal with the command:
+selon votre distribution il pourrait être souhaitable d’installer ces
+dépendances avant d’installer audiometry_trainer à travers pip (par exemple à
+travers conda si vous utilisez la distribution de Python Anaconda, ou à travers
+votre gestionnaire de paquets de Linux si vous utilisez l’installation de
+Python de votre distribution Linux), sinon pip essayera de télécharger et
+installer ces dépendances de façon automatique. Si le programme est installé
+avec succès vous devriez pouvoir le lancer depuis un terminal bash/DOS avec la
+commande :
 audiometry_trainer
-You need to ensure that the Python environment you’re using when you call the
-above command matches the one you used when you installed the application.
-_P_r_e_v_i_o_u_s _N_e_x_t
+Si vous utilisez plusieurs installations/environnements de Python, vous devez
+vous assurer que l’environnement de Python que vous employez quand vous
+utilisez la commande ci-dessus correspond à celui que vous aviez utilisé lors
+de l’installation de l’application.
+_P_r_é_c_é_d_e_n_t _S_u_i_v_a_n_t
 ===============================================================================
 © Copyright 2023-2024, Samuele Carcagno.
-Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
+Compilé avec _S_p_h_i_n_x en utilisant un _t_h_è_m_e fourni par _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/internals.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/internals.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Internals &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Internals &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/intro.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/intro.html`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Introduction &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Introduction &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -78,24 +78,31 @@
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="introduction">
 <span id="sec-intro"></span><h1>Introduction<a class="headerlink" href="#introduction" title="Permalink to this heading"></a></h1>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> is a software for practicing clinical audiometry. The software simulates patient’s responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure <a class="reference internal" href="#fig-audiometry-trainer-screenshot"><span class="std std-ref">Screenshot of the audiometry_trainer interface</span></a> shows the main window of <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>.</p>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> is a software for practicing clinical audiometry. The software simulates patient’s responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure <a class="reference internal" href="#fig-audiometry-trainer-screenshot"><span class="std std-ref">Screenshot of the audiometry_trainer interface</span></a> shows the main window of <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>. Online video tutorials are available on <a class="reference external" href="https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4">Youtube.</a></p>
 <figure class="align-default" id="id1">
 <span id="fig-audiometry-trainer-screenshot"></span><a class="reference internal image-reference" href="_images/audiometry_trainer.png"><img alt="Screenshot of the ``audiometry_trainer`` interface" src="_images/audiometry_trainer.png" style="width: 639.0px; height: 392.0px;" /></a>
 <figcaption>
 <p><span class="caption-number">Fig. 1 </span><span class="caption-text">Screenshot of the <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> interface</span><a class="headerlink" href="#id1" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
-<p>At startup <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> selects a random virtual patient case file (you can load other case files from the <code class="docutils literal notranslate"><span class="pre">File</span> <span class="pre">menu</span></code>). The <code class="docutils literal notranslate"><span class="pre">S</span></code> marker in the audiogram window shows the current stimulus level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the <code class="docutils literal notranslate"><span class="pre">Stimulus</span> <span class="pre">light</span></code> at the bottom will light up). If the virtual patient heard the stimulus the <code class="docutils literal notranslate"><span class="pre">Response</span> <span class="pre">light</span></code> on the left side will light up. Use the up/down arrows to change the stimulus level. Once you’ve found the threshold, press the <code class="docutils literal notranslate"><span class="pre">T</span></code> key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.</p>
+<p>At startup <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> selects a random virtual patient case file (you can load other case files from the <code class="docutils literal notranslate"><span class="pre">File</span> <span class="pre">menu</span></code>).</p>
+<figure class="align-default" id="id2">
+<span id="fig-file-menu"></span><a class="reference internal image-reference" href="_images/file_menu.png"><img alt="File menu" src="_images/file_menu.png" style="width: 203.0px; height: 148.0px;" /></a>
+<figcaption>
+<p><span class="caption-number">Fig. 2 </span><span class="caption-text">File menu</span><a class="headerlink" href="#id2" title="Permalink to this image"></a></p>
+</figcaption>
+</figure>
+<p>The <code class="docutils literal notranslate"><span class="pre">S</span></code> marker in the audiogram window shows the current stimulus frequency and level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the <code class="docutils literal notranslate"><span class="pre">Stimulus</span> <span class="pre">light</span></code> at the bottom will light up). If the virtual patient heard the stimulus the <code class="docutils literal notranslate"><span class="pre">Response</span> <span class="pre">light</span></code> on the left side will light up. Use the up/down arrow keys to change the stimulus level. Once you’ve found the threshold, press the <code class="docutils literal notranslate"><span class="pre">T</span></code> key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.</p>
 <p>You can compare the thresholds that you’ve estimated with the actual expected thresholds by using the <code class="docutils literal notranslate"><span class="pre">Show</span> <span class="pre">actual</span> <span class="pre">thresholds</span></code> checkboxes at the bottom of the left panel. Virtual patients are modeled via psychometric functions and the “actual” thresholds are computed via Monte Carlo simulations: they are the median thresholds obtained over a large number of simulations; 95% confidence intervals can be shown by checking the <code class="docutils literal notranslate"><span class="pre">CI</span></code> checkboxes.</p>
-<p>You can move from right to left era and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">1</span></code> at the top of the left panel. <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> is used to deliver masking noise. To turn on <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> check the <code class="docutils literal notranslate"><span class="pre">Chan.</span> <span class="pre">2</span> <span class="pre">ON</span></code> check box on the right panel, a <code class="docutils literal notranslate"><span class="pre">M</span></code> marker on the audiogram window will indicate the masking noise level. You can use the <code class="docutils literal notranslate"><span class="pre">Chan.</span> <span class="pre">2</span> <span class="pre">level</span></code> box and the up/down arrows on its right to set the masker level. You can also <code class="docutils literal notranslate"><span class="pre">lock</span></code> the <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">1</span></code> and <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> levels using the <code class="docutils literal notranslate"><span class="pre">Lock</span> <span class="pre">Channels</span></code> checkbox on the left panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.</p>
+<p>You can move from right to left ear and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">1</span></code> at the top of the left panel. <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> is used to deliver masking noise. To turn on <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> check the <code class="docutils literal notranslate"><span class="pre">Chan.</span> <span class="pre">2</span> <span class="pre">ON</span></code> check box on the right panel, a <code class="docutils literal notranslate"><span class="pre">M</span></code> marker on the audiogram window will indicate the masking noise level. You can use the <code class="docutils literal notranslate"><span class="pre">Chan.</span> <span class="pre">2</span> <span class="pre">level</span></code> box and the up/down arrows on its right to set the masker level. You can also <code class="docutils literal notranslate"><span class="pre">lock</span></code> the <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">1</span></code> and <code class="docutils literal notranslate"><span class="pre">Channel</span> <span class="pre">2</span></code> levels using the <code class="docutils literal notranslate"><span class="pre">Lock</span> <span class="pre">Channels</span></code> checkbox on the right panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.</p>
 <p>A detailed description of all the features of <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> will be given in the next sections. Section <a class="reference internal" href="installation.html#sec-installation"><span class="std std-ref">Installation</span></a> tells how to obtain and install <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>. Sections <a class="reference internal" href="threshold_search.html#sec-threshold-search"><span class="std std-ref">Threshold search</span></a> and <a class="reference internal" href="masking.html#sec-masking"><span class="std std-ref">Masking</span></a> explain how to perform a threshold search and how to use masking, respectively.</p>
 <p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> uses psychometric functions to model virtual patient responses. Responses are not deterministic (always yes/no above/below a given stimulus level) but probabilistic, with the probability of a response increasing with the stimulus level. This adds realism to the software because in real life the responses of patients are not deterministic. Section <a class="reference internal" href="virtual_listener.html#sec-virtual-listener"><span class="std std-ref">Virtual listener</span></a> details the psychometric function model used by <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>.</p>
 <p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> allows you to create and use your own case files. This functionality can be accessed via the <code class="docutils literal notranslate"><span class="pre">Generate</span> <span class="pre">case</span></code> button under the <code class="docutils literal notranslate"><span class="pre">File</span> <span class="pre">menu</span></code> and will be described in detail in Section <a class="reference internal" href="generate_case.html#sec-generate-case"><span class="std std-ref">Generating case files</span></a>. Some knowledge of the psychometric function model used by <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> will be needed to create your own case files.</p>
 <p>Section <a class="reference internal" href="user_interface.html#sec-user-interface"><span class="std std-ref">User interface</span></a> covers in details all the user interface. Section <a class="reference internal" href="internals.html#sec-internals"><span class="std std-ref">Internals</span></a> describes some of the internals of the software and is mainly intended for developers rather than for end users.</p>
 </section>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
@@ -17,39 +17,43 @@
 ===============================================================================
 ************ IInnttrroodduuccttiioonn_? ************
 audiometry_trainer is a software for practicing clinical audiometry. The
 software simulates patient’s responses loaded from case files, and allows
 practicing essential aspects of the procedure including air/bone conduction
 threshold search and clinical masking. Figure _S_c_r_e_e_n_s_h_o_t_ _o_f_ _t_h_e
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r_ _i_n_t_e_r_f_a_c_e shows the main window of audiometry_trainer.
+Online video tutorials are available on _Y_o_u_t_u_b_e_.
 _[_S_c_r_e_e_n_s_h_o_t_ _o_f_ _t_h_e_ _`_`_a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r_`_`_ _i_n_t_e_r_f_a_c_e_]
 Fig. 1 Screenshot of the audiometry_trainer interface_
 At startup audiometry_trainer selects a random virtual patient case file (you
-can load other case files from the File menu). The S marker in the audiogram
-window shows the current stimulus level. The threshold search is more
-conveniently conducted using the keyboard rather than via mouse button presses.
-Press the space bar to play the stimulus (the Stimulus light at the bottom will
-light up). If the virtual patient heard the stimulus the Response light on the
-left side will light up. Use the up/down arrows to change the stimulus level.
-Once you’ve found the threshold, press the T key to mark it on the audiogram
-plot. Use the right/left arrow keys to move to another frequency.
+can load other case files from the File menu).
+_[_F_i_l_e_ _m_e_n_u_]
+Fig. 2 File menu_
+The S marker in the audiogram window shows the current stimulus frequency and
+level. The threshold search is more conveniently conducted using the keyboard
+rather than via mouse button presses. Press the space bar to play the stimulus
+(the Stimulus light at the bottom will light up). If the virtual patient heard
+the stimulus the Response light on the left side will light up. Use the up/down
+arrow keys to change the stimulus level. Once you’ve found the threshold, press
+the T key to mark it on the audiogram plot. Use the right/left arrow keys to
+move to another frequency.
 You can compare the thresholds that you’ve estimated with the actual expected
 thresholds by using the Show actual thresholds checkboxes at the bottom of the
 left panel. Virtual patients are modeled via psychometric functions and the
 “actual” thresholds are computed via Monte Carlo simulations: they are the
 median thresholds obtained over a large number of simulations; 95% confidence
 intervals can be shown by checking the CI checkboxes.
-You can move from right to left era and from air to bone conduction stimulation
+You can move from right to left ear and from air to bone conduction stimulation
 by selecting the desired options in the drop-down menus for Channel 1 at the
 top of the left panel. Channel 2 is used to deliver masking noise. To turn on
 Channel 2 check the Chan. 2 ON check box on the right panel, a M marker on the
 audiogram window will indicate the masking noise level. You can use the Chan. 2
 level box and the up/down arrows on its right to set the masker level. You can
 also lock the Channel 1 and Channel 2 levels using the Lock Channels checkbox
-on the left panel; when the channels are locked increasing/decreasing the
+on the right panel; when the channels are locked increasing/decreasing the
 stimulus level by a given amount will automatically change the masker level by
 the the same amount.
 A detailed description of all the features of audiometry_trainer will be given
 in the next sections. Section _I_n_s_t_a_l_l_a_t_i_o_n tells how to obtain and install
 audiometry_trainer. Sections _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h and _M_a_s_k_i_n_g explain how to
 perform a threshold search and how to use masking, respectively.
 audiometry_trainer uses psychometric functions to model virtual patient
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/masking.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/masking.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Masking &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Masking &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
           o _I_n_t_e_r_a_u_r_a_l_ _a_t_t_e_n_u_a_t_i_o_n
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/references.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/references.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>References &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>References &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/search.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Search &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/searchindex.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -74,15 +74,15 @@
         "start": [2, 5],
         "from": [0, 2, 4, 5, 7, 9],
         "bash": 2,
         "do": [0, 2, 7],
         "termin": 2,
         "command": 2,
         "need": [2, 4, 5, 7],
-        "ensur": [2, 7],
+        "ensur": 7,
         "environ": 2,
         "when": [0, 2, 3, 4, 5, 6, 7, 9],
         "call": 2,
         "abov": [2, 3, 4, 9],
         "match": [2, 7],
         "one": [2, 5, 7],
         "applic": [2, 6],
@@ -217,15 +217,15 @@
         "95": [0, 4, 7, 9],
         "confid": [0, 4, 7],
         "interv": [0, 4, 6, 7],
         "shown": [0, 4, 5, 7],
         "check": [4, 5, 7],
         "ci": [4, 7],
         "rihgt": [],
-        "era": 4,
+        "era": [],
         "stimul": [4, 6],
         "desir": [0, 4, 5, 9],
         "option": [0, 4],
         "drop": 4,
         "channel": [4, 5, 7],
         "1": [4, 6, 7, 9],
         "top": 4,
@@ -240,15 +240,15 @@
         "its": [0, 4, 9],
         "set": [0, 4, 5],
         "masker": 4,
         "lock": [4, 5],
         "increas": [4, 5, 9],
         "decreas": 4,
         "amount": [4, 5],
-        "A": [0, 2, 4, 5, 6, 9],
+        "A": [0, 4, 5, 6, 9],
         "detail": [0, 4],
         "descript": 4,
         "all": [0, 4, 7, 9],
         "featur": [4, 7],
         "next": 4,
         "section": [0, 4, 7, 8],
         "tell": 4,
@@ -304,15 +304,15 @@
         "intuit": 9,
         "width": [0, 9],
         "invers": 9,
         "correl": 9,
         "ask": [7, 9],
         "90": 9,
         "order": [0, 5, 9],
-        "For": [0, 9],
+        "For": [0, 2, 9],
         "exampl": [0, 5, 7, 9],
         "5": [0, 5, 6, 9],
         "db": [0, 5, 9],
         "0": [0, 5, 9],
         "goe": 9,
         "within": [0, 9],
         "evalu": 9,
@@ -489,15 +489,15 @@
         "presenc": 9,
         "randomli": [5, 9],
         "drawn": [5, 9],
         "normal": [5, 9],
         "mean": [0, 5, 9],
         "standard": [5, 9],
         "deviat": [5, 9],
-        "ear": [5, 6, 7, 9],
+        "ear": [4, 5, 6, 7, 9],
         "combin": 9,
         "These": [5, 9],
         "fact": [5, 9],
         "interindividu": 9,
         "rang": [5, 9],
         "either": [5, 7, 9],
         "posit": [6, 9],
@@ -616,15 +616,15 @@
         "formula": [5, 9],
         "observ": 5,
         "stimuli": [0, 5],
         "mastoid": [5, 6],
         "placement": 5,
         "studebaker1967": [5, 6],
         "nuanc": 5,
-        "avail": [5, 7],
+        "avail": [4, 5, 7],
         "stenfelt2012": [5, 6],
         "integr": 5,
         "futur": [0, 5],
         "version": 5,
         "stenfelt": 6,
         "2012": 6,
         "transcrani": 6,
@@ -650,16 +650,16 @@
         "non": [5, 7],
         "nte": 5,
         "ani": [0, 5],
         "condit": 5,
         "those": [0, 5],
         "magnitud": 5,
         "deliveri": 5,
-        "make": 5,
-        "sure": 5,
+        "make": [2, 5],
+        "sure": [2, 5],
         "unchek": 5,
         "wai": 5,
         "type": [0, 5],
         "later": [0, 5],
         "dure": [5, 6],
         "additionn": 5,
         "On": [2, 7],
@@ -769,15 +769,15 @@
         "specifi": 0,
         "spreadsheet": 0,
         "like": 0,
         "row": 0,
         "remov": 0,
         "discret": 0,
         "khz": 0,
-        "multipl": 0,
+        "multipl": [0, 2],
         "cell": 0,
         "copi": 0,
         "cut": 0,
         "past": 0,
         "well": 0,
         "abbrevi": 0,
         "column": 0,
@@ -840,15 +840,15 @@
         "certain": 0,
         "wide": 0,
         "rel": 0,
         "realist": 0,
         "filenam": 0,
         "reload": 0,
         "text": 0,
-        "provid": [0, 2],
+        "provid": 0,
         "directori": 0,
         "dedic": 2,
         "iter": 0,
         "trainer": 2,
         "ia_supra": 5,
         "ia_insert": 5,
         "48": 5,
@@ -897,15 +897,24 @@
         "color": 9,
         "b": 9,
         "vertic": 9,
         "line": 9,
         "denot": 9,
         "horizont": 9,
         "dot": 9,
-        "psychometruc": []
+        "psychometruc": [],
+        "download": 2,
+        "sourceforg": 2,
+        "net": [],
+        "project": [],
+        "environn": 2,
+        "onlin": 4,
+        "video": 4,
+        "tutori": 4,
+        "youtub": 4
     },
     "objects": {},
     "objtypes": {},
     "objnames": {},
     "titleterms": {
         "gener": 0,
         "case": 0,
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/threshold_search.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/threshold_search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Threshold search &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Threshold search &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/user_interface.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/user_interface.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>User interface &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>User interface &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html/virtual_listener.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/virtual_listener.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Virtual listener &mdash; audiometry_trainer 0.1.5 documentation</title>
+  <title>Virtual listener &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -87,15 +87,15 @@
 <div class="math notranslate nohighlight" id="logistic-psychometric-function">
 <span id="equation-logistic-psychometric-function"></span><span class="eqno">(2)<a class="headerlink" href="#logistic-psychometric-function" title="Permalink to this equation"></a></span>\[\psi(x;\alpha,\beta,\gamma,\lambda)  = \gamma + (1-\gamma - \lambda) \left(\frac{1}{1+e^{\beta(\alpha-x)}}\right)\]</div>
 <p>where <span class="math notranslate nohighlight">\(\alpha\)</span> is the midpoint, <span class="math notranslate nohighlight">\(\beta\)</span> the slope, <span class="math notranslate nohighlight">\(\gamma\)</span> the lower asymptote, and <span class="math notranslate nohighlight">\(\lambda\)</span> the upper asymptote of the PF; <span class="math notranslate nohighlight">\(x\)</span> is the stimulus level at which the function is evaluated.</p>
 <p>Figure <a class="reference internal" href="#fig-logistic-psy"><span class="std std-ref">Logistic psychometric functions</span></a> shows some examples of logistic PFs representing the proportion of a “Yes” response as a function of stimulus level. All four panels show the same PF in black together with a function in a different color that has A) a different midpoint, B) a different slope and hence a different width, C) a different lower asymptote, or D) a different upper asymptote. The vertical lines in A) denote the midpoints of the functions, while in B) they denote the “width” from 5% to 95% of “Yes” responses for the two functions. The horizontal dotted lines in all panels denote the probability of correct responses at the midpoint, note that this changes in C) and D) as a function of the asymptote.</p>
 <figure class="align-default" id="id8">
 <span id="fig-logistic-psy"></span><a class="reference internal image-reference" href="_images/logistic_psy.png"><img alt="Logistic psychometric functions" src="_images/logistic_psy.png" style="width: 675.0px; height: 675.0px;" /></a>
 <figcaption>
-<p><span class="caption-number">Fig. 2 </span><span class="caption-text">Logistic psychometric functions</span><a class="headerlink" href="#id8" title="Permalink to this image"></a></p>
+<p><span class="caption-number">Fig. 3 </span><span class="caption-text">Logistic psychometric functions</span><a class="headerlink" href="#id8" title="Permalink to this image"></a></p>
 </figcaption>
 </figure>
 <p>The midpoint is the stimulus level at which the PF reaches half of its amplitude, so for a virtual listener with <span class="math notranslate nohighlight">\(\gamma = 0\)</span> and <span class="math notranslate nohighlight">\(\lambda=0\)</span>, the midpoint <span class="math notranslate nohighlight">\(\alpha\)</span> is the stimulus level at which the listener gives (on the long run) 50% of “Yes” responses. The Hughson-Westlake procedure declares the threshold as the lowest point at which the listener gives at least 50% “Yes” responses (over at least 3 trials). Therefore, the threshold (as defined with the Hughson-Westlake procedure) will be generally found at or above the midpoint <span class="math notranslate nohighlight">\(\alpha\)</span> <a class="reference internal" href="references.html#marshallandjesteadt1986" id="id3"><span>[MarshallAndJesteadt1986]</span></a>. Obviously it is possible that on occasion the threshold will be found at a lower level because the proportion of “Yes” responses found over a small number of trials may differ from the proportion of “Yes” responses expected over the long run.</p>
 <p>The slope <span class="math notranslate nohighlight">\(\beta\)</span> controls the speed at which the PF goes from its lowest to its highest value as the stimulus level increases. Rather than reasoning in terms of slope, it is often more intuitive to reason in terms of “width” of the PF (<a class="reference internal" href="references.html#alcala-quintanaandgarcia-perez2004" id="id4"><span>[Alcalá-QuintanaAndGarcía-Pérez2004]</span></a>; <a class="reference internal" href="references.html#kussetal2005" id="id5"><span>[KussEtAl2005]</span></a>), which is inversely correlated with the slope. <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> asks the user the desired 90% width of the PF in order to generate case files. For example, a width of 5 dB indicates that the function (for a virtual listener with <span class="math notranslate nohighlight">\(\gamma = 0\)</span> and <span class="math notranslate nohighlight">\(\lambda=0\)</span>) goes from 5% to 95% probability of a “Yes” response within a change in stimulus level of 5 dB.</p>
 <p>The lower asymptote, <span class="math notranslate nohighlight">\(\gamma\)</span>, represents the propensity of the listener to respond “Yes”, even in the absence of a stimulus. This propensity is not formally measured in the clinical audiometry procedure <a class="reference internal" href="references.html#barr-hamiltonetal1969" id="id6"><span>[Barr-HamiltonEtAl1969]</span></a> <a class="reference internal" href="references.html#marshallandjesteadt1986" id="id7"><span>[MarshallAndJesteadt1986]</span></a>. In a Yes/No task with temporally marked trials, in which a signal is presented or not, it would correspond to the false alarm rate. For example, a listener with a <span class="math notranslate nohighlight">\(\gamma\)</span> of 0.1 would respond “Yes” in 1 out of 10 trials in which no stimulus was presented. Under the perspective of signal detection theory this propensity of the listener to say “Yes” reflects an internal criterion which can be more or less conservative. Although the actual measurement of <span class="math notranslate nohighlight">\(\gamma\)</span> requires “blank” trials without a signal, the criterion determines the decision process also when a signal is present, hence the value of <span class="math notranslate nohighlight">\(\gamma\)</span> will affect the PF underlying the clinical audiometry procedure.</p>
 <p>The upper asymptote, <span class="math notranslate nohighlight">\(\lambda\)</span> is the lapse rate, it represents the tendency of the listener to fail responding because of attentional lapses, even for a stimulus that is clearly audible.</p>
 <p>When performing clinical masking with <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, the effect of the noise is to shift the midpoint of the PF, <em>if</em> the noise level arriving at the cochlea, in dB of effective masking (EM) units, exceeds the midpoint of the PF. The shift is equal to the level by which the noise exceeds the midpoint. For example, if the noise level is 5 dB above the unmasked midpoint, the masked midpoint will be 5 dB higher.</p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
     * _M_a_s_k_i_n_g
     * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
@@ -32,15 +32,15 @@
 hence a different width, C) a different lower asymptote, or D) a different
 upper asymptote. The vertical lines in A) denote the midpoints of the
 functions, while in B) they denote the “width” from 5% to 95% of “Yes”
 responses for the two functions. The horizontal dotted lines in all panels
 denote the probability of correct responses at the midpoint, note that this
 changes in C) and D) as a function of the asymptote.
 _[_L_o_g_i_s_t_i_c_ _p_s_y_c_h_o_m_e_t_r_i_c_ _f_u_n_c_t_i_o_n_s_]
-Fig. 2 Logistic psychometric functions_
+Fig. 3 Logistic psychometric functions_
 The midpoint is the stimulus level at which the PF reaches half of its
 amplitude, so for a virtual listener with \(\gamma = 0\) and \(\lambda=0\), the
 midpoint \(\alpha\) is the stimulus level at which the listener gives (on the
 long run) 50% of “Yes” responses. The Hughson-Westlake procedure declares the
 threshold as the lowest point at which the listener gives at least 50% “Yes”
 responses (over at least 3 trials). Therefore, the threshold (as defined with
 the Hughson-Westlake procedure) will be generally found at or above the
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.fr.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.fr.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_images/logistic_psy.fr.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_images/logistic_psy.fr.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/generate_case.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/generate_case.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/index.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/installation.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/installation.rst.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .. _sec-installation:
 
 ************
 Installation
 ************
 
-``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. A dedicated installer is provided for Windows. On Linux and Mac (and Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
+``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. For Windows, a dedicated installer can be downloaded from `SourceForge <https://sourceforge.net/projects/audiometry-trainer/files/>`_.
+
+On Linux and Mac (but also on Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
 
 .. code-block:: bash
 
 		pip install audiometry-trainer
 
 ``audiometry_trainer`` depends on a few Python modules including:
 
@@ -20,14 +22,14 @@
 
 depending on your Python distribution you may want to install these dependecies before installing ``audiometry_trainer`` via ``pip`` (e.g. through ``conda`` if you're using the Anaconda Python distribution, or through your Linux distribution package manager if you're using the Python installation that comes with your Linux distribution), otherwise ``pip`` will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:
 
 .. code-block:: bash
 
 	audiometry_trainer
 
-You need to ensure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
+If you use multiple Python installations/environnments, you need to make sure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/internals.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/internals.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/intro.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/intro.rst.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 .. _sec-intro:
 
 *************
 Introduction
 *************
 
-``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``.
+``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``. Online video tutorials are available on `Youtube. <https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4>`_
 
 .. _fig-audiometry_trainer_screenshot:
 
 .. figure:: audiometry_trainer.png
    :scale: 50%
    :alt: Screenshot of the ``audiometry_trainer`` interface
 
    Screenshot of the ``audiometry_trainer`` interface
 
-At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``). The ``S`` marker in the audiogram window shows the current stimulus level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrows to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
+At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``).
+
+.. _fig-file_menu:
+
+.. figure:: file_menu.png
+   :scale: 100%
+   :alt: File menu
+
+   File menu
+   
+The ``S`` marker in the audiogram window shows the current stimulus frequency and level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrow keys to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
 
 You can compare the thresholds that you've estimated with the actual expected thresholds by using the ``Show actual thresholds`` checkboxes at the bottom of the left panel. Virtual patients are modeled via psychometric functions and the "actual" thresholds are computed via Monte Carlo simulations: they are the median thresholds obtained over a large number of simulations; 95% confidence intervals can be shown by checking the ``CI`` checkboxes.
 
-You can move from right to left era and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the left panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
+You can move from right to left ear and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the right panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
 
 A detailed description of all the features of ``audiometry_trainer`` will be given in the next sections. Section :ref:`sec-installation` tells how to obtain and install ``audiometry_trainer``. Sections :ref:`sec-threshold_search` and :ref:`sec-masking` explain how to perform a threshold search and how to use masking, respectively.
 
 ``audiometry_trainer`` uses psychometric functions to model virtual patient responses. Responses are not deterministic (always yes/no above/below a given stimulus level) but probabilistic, with the probability of a response increasing with the stimulus level. This adds realism to the software because in real life the responses of patients are not deterministic. Section :ref:`sec-virtual_listener` details the psychometric function model used by ``audiometry_trainer``.
 
 ``audiometry_trainer`` allows you to create and use your own case files. This functionality can be accessed via the ``Generate case`` button under the ``File menu`` and will be described in detail in Section :ref:`sec-generate_case`. Some knowledge of the psychometric function model used by ``audiometry_trainer`` will be needed to create your own case files.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/masking.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/masking.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/references.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/references.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/threshold_search.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/threshold_search.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_sources/virtual_listener.rst.txt` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_sources/virtual_listener.rst.txt`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/_sphinx_javascript_frameworks_compat.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/_sphinx_javascript_frameworks_compat.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/base-stemmer.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/base-stemmer.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/basic.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/basic.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/css/badge_only.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/css/theme.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/doctools.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Bold.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Italic.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/Lato-Regular.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Bold.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Regular.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/RobotoSlab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.eot` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.svg` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.ttf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff2` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/french-stemmer.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/french-stemmer.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/jquery.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/js/theme.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/language_data.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/pygments.css` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/searchtools.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/sphinx_highlight.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/translations.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/translations.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/_static/underscore.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/generate_case.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/generate_case.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Générer des fichiers de cas &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Générer des fichiers de cas &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/genindex.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/genindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Index &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -27,15 +27,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/index.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Bienvenus à la documentation de audiometry_trainer ! &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Bienvenus à la documentation de audiometry_trainer ! &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/installation.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html/installation.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 <!DOCTYPE html>
-<html class="writer-html5" lang="fr" >
+<html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Installation &mdash; audiometry_trainer 0.1.6 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
         <script src="_static/doctools.js"></script>
         <script src="_static/sphinx_highlight.js"></script>
-        <script src="_static/translations.js"></script>
     <script src="_static/js/theme.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
-    <link rel="search" title="Recherche" href="search.html" />
-    <link rel="next" title="Recherche du seuil" href="threshold_search.html" />
+    <link rel="search" title="Search" href="search.html" />
+    <link rel="next" title="Threshold search" href="threshold_search.html" />
     <link rel="prev" title="Introduction" href="intro.html" /> 
 </head>
 
 <body class="wy-body-for-nav"> 
   <div class="wy-grid-for-nav">
     <nav data-toggle="wy-nav-shift" class="wy-nav-side">
       <div class="wy-side-scroll">
@@ -30,35 +29,35 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
-    <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
+    <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
 </div>
         </div><div class="wy-menu wy-menu-vertical" data-spy="affix" role="navigation" aria-label="Navigation menu">
-              <p class="caption" role="heading"><span class="caption-text">Table des matières :</span></p>
+              <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="intro.html">Introduction</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Installation</a></li>
-<li class="toctree-l1"><a class="reference internal" href="threshold_search.html">Recherche du seuil</a></li>
-<li class="toctree-l1"><a class="reference internal" href="masking.html">Masquage</a></li>
-<li class="toctree-l1"><a class="reference internal" href="virtual_listener.html">Sujet virtuel</a></li>
-<li class="toctree-l1"><a class="reference internal" href="generate_case.html">Générer des fichiers de cas</a></li>
-<li class="toctree-l1"><a class="reference internal" href="user_interface.html">Interface utilisateur</a></li>
-<li class="toctree-l1"><a class="reference internal" href="internals.html">Fonctionnement interne</a></li>
-<li class="toctree-l1"><a class="reference internal" href="references.html">Références</a></li>
+<li class="toctree-l1"><a class="reference internal" href="threshold_search.html">Threshold search</a></li>
+<li class="toctree-l1"><a class="reference internal" href="masking.html">Masking</a></li>
+<li class="toctree-l1"><a class="reference internal" href="virtual_listener.html">Virtual listener</a></li>
+<li class="toctree-l1"><a class="reference internal" href="generate_case.html">Generating case files</a></li>
+<li class="toctree-l1"><a class="reference internal" href="user_interface.html">User interface</a></li>
+<li class="toctree-l1"><a class="reference internal" href="internals.html">Internals</a></li>
+<li class="toctree-l1"><a class="reference internal" href="references.html">References</a></li>
 </ul>
 
         </div>
       </div>
     </nav>
 
     <section data-toggle="wy-nav-shift" class="wy-nav-content-wrap"><nav class="wy-nav-top" aria-label="Mobile navigation menu" >
@@ -69,62 +68,63 @@
       <div class="wy-nav-content">
         <div class="rst-content">
           <div role="navigation" aria-label="Page navigation">
   <ul class="wy-breadcrumbs">
       <li><a href="index.html" class="icon icon-home" aria-label="Home"></a></li>
       <li class="breadcrumb-item active">Installation</li>
       <li class="wy-breadcrumbs-aside">
-            <a href="_sources/installation.rst.txt" rel="nofollow"> Afficher la source de la page</a>
+            <a href="_sources/installation.rst.txt" rel="nofollow"> View page source</a>
       </li>
   </ul>
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="installation">
-<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Lien permanent vers cette rubrique"></a></h1>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> a été installé et utilisé avec succès sur Linux et Windows. Il devrait aussi marcher sur des ordinateurs Mac, mais cela n’a pas été testé. Pour Windows il y a un programme d’installation dédié. Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser le programme d’installation dédié) <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, qui est écrit en Python, peut être installé à travers <code class="docutils literal notranslate"><span class="pre">pip</span></code>:</p>
+<span id="sec-installation"></span><h1>Installation<a class="headerlink" href="#installation" title="Permalink to this heading"></a></h1>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. For Windows, a dedicated installer can be downloaded from <a class="reference external" href="https://sourceforge.net/projects/audiometry-trainer/files/">SourceForge</a>.</p>
+<p>On Linux and Mac (but also on Windows if you do not wish to use the dedicated installer) <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, which is written in Python, can be installed via the Python package installer <code class="docutils literal notranslate"><span class="pre">pip</span></code>:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>pip<span class="w"> </span>install<span class="w"> </span>audiometry-trainer
 </pre></div>
 </div>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> dépend d’un petit nombre de modules Python y compris :</p>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> depends on a few Python modules including:</p>
 <blockquote>
 <div><ul class="simple">
 <li><p>PyQt5</p></li>
 <li><p>numpy</p></li>
 <li><p>scipy</p></li>
 <li><p>matplotlib</p></li>
 <li><p>pandas</p></li>
 </ul>
 </div></blockquote>
-<p>selon votre distribution il pourrait être souhaitable d’installer ces dépendances avant d’installer <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> à travers <code class="docutils literal notranslate"><span class="pre">pip</span></code> (par exemple à travers <code class="docutils literal notranslate"><span class="pre">conda</span></code> si vous utilisez la distribution de Python Anaconda, ou à travers votre gestionnaire de paquets de Linux si vous utilisez l’installation de Python de votre distribution Linux), sinon <code class="docutils literal notranslate"><span class="pre">pip</span></code> essayera de télécharger et installer ces dépendances de façon automatique. Si le programme est installé avec succès vous devriez pouvoir le lancer depuis un terminal bash/DOS avec la commande :</p>
+<p>depending on your Python distribution you may want to install these dependecies before installing <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> via <code class="docutils literal notranslate"><span class="pre">pip</span></code> (e.g. through <code class="docutils literal notranslate"><span class="pre">conda</span></code> if you’re using the Anaconda Python distribution, or through your Linux distribution package manager if you’re using the Python installation that comes with your Linux distribution), otherwise <code class="docutils literal notranslate"><span class="pre">pip</span></code> will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>audiometry_trainer
 </pre></div>
 </div>
-<p>Vous devez vous assurer que l’environnement de Python que vous employez quand vous utilisez la commande ci-dessus correspond à celui   que vous aviez utilisé lors de l’installation de l’application.</p>
+<p>If you use multiple Python installations/environnments, you need to make sure that the Python environment you’re using when you call the above command matches the one you used when you installed the application.</p>
 </section>
 
 
            </div>
           </div>
-          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Pied de page">
-        <a href="intro.html" class="btn btn-neutral float-left" title="Introduction" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Précédent</a>
-        <a href="threshold_search.html" class="btn btn-neutral float-right" title="Recherche du seuil" accesskey="n" rel="next">Suivant <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
+          <footer><div class="rst-footer-buttons" role="navigation" aria-label="Footer">
+        <a href="intro.html" class="btn btn-neutral float-left" title="Introduction" accesskey="p" rel="prev"><span class="fa fa-arrow-circle-left" aria-hidden="true"></span> Previous</a>
+        <a href="threshold_search.html" class="btn btn-neutral float-right" title="Threshold search" accesskey="n" rel="next">Next <span class="fa fa-arrow-circle-right" aria-hidden="true"></span></a>
     </div>
 
   <hr/>
 
   <div role="contentinfo">
     <p>&#169; Copyright 2023-2024, Samuele Carcagno.</p>
   </div>
 
-  Compilé avec <a href="https://www.sphinx-doc.org/">Sphinx</a> en utilisant un
-    <a href="https://github.com/readthedocs/sphinx_rtd_theme">thème</a>
-    fourni par <a href="https://readthedocs.org">Read the Docs</a>.
+  Built with <a href="https://www.sphinx-doc.org/">Sphinx</a> using a
+    <a href="https://github.com/readthedocs/sphinx_rtd_theme">theme</a>
+    provided by <a href="https://readthedocs.org">Read the Docs</a>.
    
 
 </footer>
         </div>
       </div>
     </section>
   </div>
```

#### html2text {}

```diff
@@ -1,47 +1,46 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
-Table des matières :
+Contents:
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
-    * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
-    * _M_a_s_q_u_a_g_e
-    * _S_u_j_e_t_ _v_i_r_t_u_e_l
-    * _G_é_n_é_r_e_r_ _d_e_s_ _f_i_c_h_i_e_r_s_ _d_e_ _c_a_s
-    * _I_n_t_e_r_f_a_c_e_ _u_t_i_l_i_s_a_t_e_u_r
-    * _F_o_n_c_t_i_o_n_n_e_m_e_n_t_ _i_n_t_e_r_n_e
-    * _R_é_f_é_r_e_n_c_e_s
+    * _T_h_r_e_s_h_o_l_d_ _s_e_a_r_c_h
+    * _M_a_s_k_i_n_g
+    * _V_i_r_t_u_a_l_ _l_i_s_t_e_n_e_r
+    * _G_e_n_e_r_a_t_i_n_g_ _c_a_s_e_ _f_i_l_e_s
+    * _U_s_e_r_ _i_n_t_e_r_f_a_c_e
+    * _I_n_t_e_r_n_a_l_s
+    * _R_e_f_e_r_e_n_c_e_s
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
     * Installation
-    * _A_f_f_i_c_h_e_r_ _l_a_ _s_o_u_r_c_e_ _d_e_ _l_a_ _p_a_g_e
+    * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ IInnssttaallllaattiioonn_? ************
-audiometry_trainer a été installé et utilisé avec succès sur Linux et Windows.
-Il devrait aussi marcher sur des ordinateurs Mac, mais cela n’a pas été testé.
-Pour Windows il y a un programme d’installation dédié. Sur Linux et Mac (mais
-aussi sur Windows si vous ne souhaitez pas utiliser le programme d’installation
-dédié) audiometry_trainer, qui est écrit en Python, peut être installé à
-travers pip:
+audiometry_trainer has been successfully installed and used on Linux and
+Windows. It should also work on Mac platforms, but this has not been tested.
+For Windows, a dedicated installer can be downloaded from _S_o_u_r_c_e_F_o_r_g_e.
+On Linux and Mac (but also on Windows if you do not wish to use the dedicated
+installer) audiometry_trainer, which is written in Python, can be installed via
+the Python package installer pip:
 pip install audiometry-trainer
-audiometry_trainer dépend d’un petit nombre de modules Python y compris :
+audiometry_trainer depends on a few Python modules including:
          * PyQt5
          * numpy
          * scipy
          * matplotlib
          * pandas
-selon votre distribution il pourrait être souhaitable d’installer ces
-dépendances avant d’installer audiometry_trainer à travers pip (par exemple à
-travers conda si vous utilisez la distribution de Python Anaconda, ou à travers
-votre gestionnaire de paquets de Linux si vous utilisez l’installation de
-Python de votre distribution Linux), sinon pip essayera de télécharger et
-installer ces dépendances de façon automatique. Si le programme est installé
-avec succès vous devriez pouvoir le lancer depuis un terminal bash/DOS avec la
-commande :
+depending on your Python distribution you may want to install these dependecies
+before installing audiometry_trainer via pip (e.g. through conda if you’re
+using the Anaconda Python distribution, or through your Linux distribution
+package manager if you’re using the Python installation that comes with your
+Linux distribution), otherwise pip will attempt to automatically pull in and
+install these dependencies. If the program is successfully installed you should
+be able to start it from a bash/DOS terminal with the command:
 audiometry_trainer
-Vous devez vous assurer que l’environnement de Python que vous employez quand
-vous utilisez la commande ci-dessus correspond à celui que vous aviez utilisé
-lors de l’installation de l’application.
-_P_r_é_c_é_d_e_n_t _S_u_i_v_a_n_t
+If you use multiple Python installations/environnments, you need to make sure
+that the Python environment you’re using when you call the above command
+matches the one you used when you installed the application.
+_P_r_e_v_i_o_u_s _N_e_x_t
 ===============================================================================
 © Copyright 2023-2024, Samuele Carcagno.
-Compilé avec _S_p_h_i_n_x en utilisant un _t_h_è_m_e fourni par _R_e_a_d_ _t_h_e_ _D_o_c_s.
+Built with _S_p_h_i_n_x using a _t_h_e_m_e provided by _R_e_a_d_ _t_h_e_ _D_o_c_s.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/internals.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/internals.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Fonctionnement interne &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Fonctionnement interne &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/intro.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/intro.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Introduction &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Introduction &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -79,24 +79,31 @@
   <hr/>
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="introduction">
 <span id="sec-intro"></span><h1>Introduction<a class="headerlink" href="#introduction" title="Lien permanent vers cette rubrique"></a></h1>
-<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> est un logiciel pour s’entraîner à l’audiométrie clinique. Le logiciel simule les réponses de patients depuis des fichiers de cas et permet de pratiquer des aspects essentiels de la procédure, y compris la recherche de seuil par voie aérienne/osseuse et le masquage clinique. La figure <a class="reference internal" href="#fig-audiometry-trainer-screenshot"><span class="std std-ref">Capture d’écran de la fenêtre principale de audiometry_trainer</span></a> affiche la fenêtre principale de <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>.</p>
+<p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> est un logiciel pour s’entraîner à l’audiométrie clinique. Le logiciel simule les réponses de patients depuis des fichiers de cas et permet de pratiquer des aspects essentiels de la procédure, y compris la recherche de seuil par voie aérienne/osseuse et le masquage clinique. La figure <a class="reference internal" href="#fig-audiometry-trainer-screenshot"><span class="std std-ref">Capture d’écran de la fenêtre principale de audiometry_trainer</span></a> affiche la fenêtre principale de <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>. Des tutoriels vidéo sont disponible sur <a class="reference external" href="https://www.youtube.com/playlist?list=PLyfCl_MBfnRBh7CLE48BeawkZpKODle1X">Youtube.</a></p>
 <figure class="align-default" id="id1">
 <span id="fig-audiometry-trainer-screenshot"></span><a class="reference internal image-reference" href="_images/audiometry_trainer.fr.png"><img alt="Capture d'écran de la fenêtre principale de ``audiometry_trainer``" src="_images/audiometry_trainer.fr.png" style="width: 641.0px; height: 373.0px;" /></a>
 <figcaption>
 <p><span class="caption-number">Fig. 1 </span><span class="caption-text">Capture d’écran de la fenêtre principale de <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code></span><a class="headerlink" href="#id1" title="Lien permanent vers cette image"></a></p>
 </figcaption>
 </figure>
-<p>Au démarrage <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> sélectionne de façon aléatoire un fichier de cas d’un patient virtuel (vous pouvez charger d’autres cas depuis le menu <code class="docutils literal notranslate"><span class="pre">Fichier</span></code>). Le marqueur <code class="docutils literal notranslate"><span class="pre">S</span></code> affiché dans la fenêtre de l’audiogramme indique le niveau courant du stimulus. C’est plus pratique d’effectuer la recherche du seuil avec le clavier qu’un utilisant la souris pour cliquer sur des boutons. Appuyez sur la barre d’espace pour jouer le stimulus (le <code class="docutils literal notranslate"><span class="pre">Témoin</span> <span class="pre">du</span> <span class="pre">stimulus</span></code> en bas s’allumera). Si le patient virtuel a entendu le stimulus le <code class="docutils literal notranslate"><span class="pre">Témoin</span> <span class="pre">de</span> <span class="pre">réponse</span></code> sur la gauche s’allumera. Utilisez les flèches haut/bas pour changer le niveau du stimulus. Lorsque vous avez trouvé le seuil marquez-le en appuyant sur la touche <code class="docutils literal notranslate"><span class="pre">T</span></code> (de l’anglais « Threshold »). Utilisez les flèches droite/gauche pour vous déplacer sur une autre fréquence.</p>
+<p>Au démarrage <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> sélectionne de façon aléatoire un fichier de cas de patient virtuel (vous pouvez charger d’autres cas depuis le menu <code class="docutils literal notranslate"><span class="pre">Fichier</span></code>).</p>
+<figure class="align-default" id="id2">
+<span id="fig-file-menu"></span><a class="reference internal image-reference" href="_images/file_menu.fr.png"><img alt="Fichier menu" src="_images/file_menu.fr.png" style="width: 246.0px; height: 147.0px;" /></a>
+<figcaption>
+<p><span class="caption-number">Fig. 2 </span><span class="caption-text">Fichier menu</span><a class="headerlink" href="#id2" title="Lien permanent vers cette image"></a></p>
+</figcaption>
+</figure>
+<p>Le marqueur <code class="docutils literal notranslate"><span class="pre">S</span></code> affiché dans la fenêtre de l’audiogramme indique la fréquence et le niveau courants du stimulus. C’est plus pratique d’effectuer la recherche du seuil avec le clavier qu’en cliquant sur des boutons avec la souris. Appuyez sur la barre d’espace pour jouer le stimulus (le <code class="docutils literal notranslate"><span class="pre">Témoin</span> <span class="pre">du</span> <span class="pre">stimulus</span></code> en bas s’allumera). Si le patient virtuel a entendu le son le <code class="docutils literal notranslate"><span class="pre">Témoin</span> <span class="pre">de</span> <span class="pre">réponse</span></code> sur la gauche s’allumera. Utilisez les flèches haut/bas du clavier pour changer le niveau du stimulus. Lorsque vous avez trouvé le seuil, marquez-le en appuyant sur la touche <code class="docutils literal notranslate"><span class="pre">T</span></code> (de l’anglais « Threshold »). Utilisez les flèches droite/gauche du clavier pour vous déplacer sur une autre fréquence.</p>
 <p>Vous pouvez comparer les seuils que vous avez mesuré avec les seuils attendus en cochant les cases sous <code class="docutils literal notranslate"><span class="pre">Affichage</span> <span class="pre">des</span> <span class="pre">vrais</span> <span class="pre">seuils</span></code> dans la partie basse du panneau de gauche. Les patients virtuels sont modelés à travers des courbes psychométriques et les « vrais » seuils sont calculés à travers des méthodes de Monte-Carlo : ils sont les seuils médians obtenus sur un large nombre de simulations ; des intervalles de confiance de 95% peuvent être affichés en cochant les cases <code class="docutils literal notranslate"><span class="pre">CI</span></code>.</p>
-<p>Vous pouvez passer de l’oreille droite à la gauche et de la stimulation en conduction aérienne à celle en conduction osseuse en sélectionnant les options souhaitées dans les menus déroulant pour le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">1</span></code> en haut du panneau de gauche. Le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> est utilisé pour envoyer du bruit masquant. Pour allumer le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> cochez la case <code class="docutils literal notranslate"><span class="pre">Can.</span> <span class="pre">2</span> <span class="pre">ON</span></code> sur le panneau de droite, un marqueur <code class="docutils literal notranslate"><span class="pre">M</span></code> dans la fenêtre de l’audiogramme affichera le niveau courant du bruit masquant. Vous pouvez utiliser la case <code class="docutils literal notranslate"><span class="pre">Niveau</span> <span class="pre">du</span> <span class="pre">can.</span> <span class="pre">2</span></code> ainsi que les flèches haut/bas à sa droite pour saisir le niveau du bruit masquant. Vous pouvez aussi « verrouiller » le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> au <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">1</span></code> en cochant la case <code class="docutils literal notranslate"><span class="pre">Verrouiller</span> <span class="pre">les</span> <span class="pre">canaux</span></code> sur le panneau de gauche : lorsque les canaux sont verrouillés, des augmentations/baisses du niveau du stimulus d’une taille donné déclencheront automatiquement des changements du niveau du masqueur de la même taille.</p>
+<p>Vous pouvez passer de l’oreille droite à la gauche et de la stimulation en conduction aérienne à celle en conduction osseuse en sélectionnant les options souhaitées dans les menus déroulant pour le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">1</span></code> en haut du panneau de gauche. Le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> est utilisé pour envoyer du bruit masquant. Pour allumer le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> cochez la case <code class="docutils literal notranslate"><span class="pre">Can.</span> <span class="pre">2</span> <span class="pre">ON</span></code> sur le panneau de droite, un marqueur <code class="docutils literal notranslate"><span class="pre">M</span></code> dans la fenêtre de l’audiogramme affichera le niveau courant du bruit masquant. Vous pouvez utiliser la case <code class="docutils literal notranslate"><span class="pre">Niveau</span> <span class="pre">du</span> <span class="pre">can.</span> <span class="pre">2</span></code> ainsi que les flèches haut/bas à sa droite pour saisir le niveau du bruit masquant. Vous pouvez aussi « verrouiller » le <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">2</span></code> au <code class="docutils literal notranslate"><span class="pre">Canal</span> <span class="pre">1</span></code> en cochant la case <code class="docutils literal notranslate"><span class="pre">Verrouiller</span> <span class="pre">les</span> <span class="pre">canaux</span></code> sur le panneau de droite : lorsque les canaux sont verrouillés, des augmentations/baisses du niveau du stimulus d’une taille donné déclencheront automatiquement des changements du niveau du masqueur de la même taille.</p>
 <p>Une description détaillée de toutes les fonctionnalités de <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> sera donne dans les sections suivantes. La Section <a class="reference internal" href="installation.html#sec-installation"><span class="std std-ref">Installation</span></a> explique comment obtenir et installer <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>. Les sections <a class="reference internal" href="threshold_search.html#sec-threshold-search"><span class="std std-ref">Recherche du seuil</span></a> and <a class="reference internal" href="masking.html#sec-masking"><span class="std std-ref">Masquage</span></a> expliquent comment faire une recherche de seuil et comment utiliser le masquage, respectivement.</p>
 <p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> utilise des courbes psychométriques pour modéliser les réponses des patients virtuels. Les réponses ne sont pas déterministes (toujours oui/non au dessus/dessous d’un certain niveau de stimulation) mais probabilistes, avec une probabilité de réponse croissante en fonction du niveau de stimulation. Cela rends le logiciel plus réaliste car dans la vie réelle les réponses des patients ne sont pas déterministes. La section <a class="reference internal" href="virtual_listener.html#sec-virtual-listener"><span class="std std-ref">Sujet virtuel</span></a> détaille le modèle de courbe psychométrique utilisé par <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>.</p>
 <p><code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> vous permet de générer et utiliser vous propres fichiers de cas. Vous pouvez accéder à cette fonctionnalité à travers l’action <code class="docutils literal notranslate"><span class="pre">Générer</span> <span class="pre">un</span> <span class="pre">cas</span></code> sous le menu <code class="docutils literal notranslate"><span class="pre">Fichier</span></code> et ça sera illustré en détails dans la Section <a class="reference internal" href="generate_case.html#sec-generate-case"><span class="std std-ref">Générer des fichiers de cas</span></a>. Quelques connaissances du modèle de fonction psychométrique utilisé par <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> seront nécessaires pour la création de vos propres fichiers de cas.</p>
 <p>La Section <a class="reference internal" href="user_interface.html#sec-user-interface"><span class="std std-ref">Interface utilisateur</span></a> couvre en détail toute l’interface utilisateur. La Section <a class="reference internal" href="internals.html#sec-internals"><span class="std std-ref">Fonctionnement interne</span></a> décrits quelques aspects du fonctionnement interne du logiciel et est adressée aux développeurs plutôt qu’aux utilisateurs du logiciel.</p>
 </section>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
@@ -17,28 +17,32 @@
 ===============================================================================
 ************ IInnttrroodduuccttiioonn_? ************
 audiometry_trainer est un logiciel pour s’entraîner à l’audiométrie clinique.
 Le logiciel simule les réponses de patients depuis des fichiers de cas et
 permet de pratiquer des aspects essentiels de la procédure, y compris la
 recherche de seuil par voie aérienne/osseuse et le masquage clinique. La figure
 _C_a_p_t_u_r_e_ _d_’_é_c_r_a_n_ _d_e_ _l_a_ _f_e_n_ê_t_r_e_ _p_r_i_n_c_i_p_a_l_e_ _d_e_ _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r affiche la
-fenêtre principale de audiometry_trainer.
+fenêtre principale de audiometry_trainer. Des tutoriels vidéo sont disponible
+sur _Y_o_u_t_u_b_e_.
 _[_C_a_p_t_u_r_e_ _d_'_é_c_r_a_n_ _d_e_ _l_a_ _f_e_n_ê_t_r_e_ _p_r_i_n_c_i_p_a_l_e_ _d_e_ _`_`_a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r_`_`_]
 Fig. 1 Capture d’écran de la fenêtre principale de audiometry_trainer_
 Au démarrage audiometry_trainer sélectionne de façon aléatoire un fichier de
-cas d’un patient virtuel (vous pouvez charger d’autres cas depuis le menu
-Fichier). Le marqueur S affiché dans la fenêtre de l’audiogramme indique le
-niveau courant du stimulus. C’est plus pratique d’effectuer la recherche du
-seuil avec le clavier qu’un utilisant la souris pour cliquer sur des boutons.
-Appuyez sur la barre d’espace pour jouer le stimulus (le Témoin du stimulus en
-bas s’allumera). Si le patient virtuel a entendu le stimulus le Témoin de
-réponse sur la gauche s’allumera. Utilisez les flèches haut/bas pour changer le
-niveau du stimulus. Lorsque vous avez trouvé le seuil marquez-le en appuyant
+cas de patient virtuel (vous pouvez charger d’autres cas depuis le menu
+Fichier).
+_[_F_i_c_h_i_e_r_ _m_e_n_u_]
+Fig. 2 Fichier menu_
+Le marqueur S affiché dans la fenêtre de l’audiogramme indique la fréquence et
+le niveau courants du stimulus. C’est plus pratique d’effectuer la recherche du
+seuil avec le clavier qu’en cliquant sur des boutons avec la souris. Appuyez
+sur la barre d’espace pour jouer le stimulus (le Témoin du stimulus en bas
+s’allumera). Si le patient virtuel a entendu le son le Témoin de réponse sur la
+gauche s’allumera. Utilisez les flèches haut/bas du clavier pour changer le
+niveau du stimulus. Lorsque vous avez trouvé le seuil, marquez-le en appuyant
 sur la touche T (de l’anglais « Threshold »). Utilisez les flèches droite/
-gauche pour vous déplacer sur une autre fréquence.
+gauche du clavier pour vous déplacer sur une autre fréquence.
 Vous pouvez comparer les seuils que vous avez mesuré avec les seuils attendus
 en cochant les cases sous Affichage des vrais seuils dans la partie basse du
 panneau de gauche. Les patients virtuels sont modelés à travers des courbes
 psychométriques et les « vrais » seuils sont calculés à travers des méthodes de
 Monte-Carlo : ils sont les seuils médians obtenus sur un large nombre de
 simulations ; des intervalles de confiance de 95% peuvent être affichés en
 cochant les cases CI.
@@ -47,15 +51,15 @@
 souhaitées dans les menus déroulant pour le Canal 1 en haut du panneau de
 gauche. Le Canal 2 est utilisé pour envoyer du bruit masquant. Pour allumer le
 Canal 2 cochez la case Can. 2 ON sur le panneau de droite, un marqueur M dans
 la fenêtre de l’audiogramme affichera le niveau courant du bruit masquant. Vous
 pouvez utiliser la case Niveau du can. 2 ainsi que les flèches haut/bas à sa
 droite pour saisir le niveau du bruit masquant. Vous pouvez aussi
 « verrouiller » le Canal 2 au Canal 1 en cochant la case Verrouiller les canaux
-sur le panneau de gauche : lorsque les canaux sont verrouillés, des
+sur le panneau de droite : lorsque les canaux sont verrouillés, des
 augmentations/baisses du niveau du stimulus d’une taille donné déclencheront
 automatiquement des changements du niveau du masqueur de la même taille.
 Une description détaillée de toutes les fonctionnalités de audiometry_trainer
 sera donne dans les sections suivantes. La Section _I_n_s_t_a_l_l_a_t_i_o_n explique
 comment obtenir et installer audiometry_trainer. Les sections _R_e_c_h_e_r_c_h_e_ _d_u
 _s_e_u_i_l and _M_a_s_q_u_a_g_e expliquent comment faire une recherche de seuil et comment
 utiliser le masquage, respectivement.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/masking.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/masking.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Masquage &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Masquage &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -31,15 +31,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
           o _A_t_t_é_n_u_a_t_i_o_n_ _i_n_t_e_r_a_u_r_a_l_e
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/references.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/references.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Références &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Références &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/search.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Recherche &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Recherche &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/searchindex.js` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -979,15 +979,15 @@
         "\u00e9crit": 2,
         "peut": [0, 2, 5, 7, 9],
         "\u00eatre": [0, 2, 4, 5, 7, 9],
         "traver": [0, 2, 4, 7],
         "d\u00e9pend": 2,
         "pet": [2, 9],
         "nombr": [0, 2, 4, 7, 9],
-        "Vous": [0, 2, 4, 7],
+        "Vous": [0, 4, 7],
         "dev": [2, 5],
         "assur": [2, 5, 7],
         "environ": [0, 2, 5, 9],
         "emploi": [0, 2, 7],
         "quand": [0, 2, 5, 7, 9],
         "dessus": [2, 4, 9],
         "celui": [2, 5],
@@ -1056,15 +1056,15 @@
         "\u00e9dit": 0,
         "ensuit": [0, 5, 7],
         "seul": 0,
         "entre": [0, 5, 9],
         "En": [0, 7],
         "s\u00e9lection": [0, 4, 5],
         "sour": [0, 4],
-        "plusieur": [0, 5],
+        "plusieur": [0, 2, 5],
         "cellul": 0,
         "droit": [0, 4, 7],
         "copi": 0,
         "coup": 0,
         "coll": 0,
         "valeur": [0, 5, 9],
         "tout": [0, 4, 7, 9],
@@ -1079,15 +1079,15 @@
         "oss": 0,
         "inatt": 0,
         "gauch": [0, 4, 7],
         "quelqu": [0, 4],
         "pert": [0, 5],
         "audit": 0,
         "neurosensoriel": 0,
-        "pouv": [0, 4, 7],
+        "pouv": [0, 2, 4, 7],
         "fix": [0, 5],
         "autour": 0,
         "largeur": [0, 9],
         "z\u00e9ro": 0,
         "auquel": [0, 9],
         "r\u00e9pond": [0, 7],
         "oui": [0, 4, 9],
@@ -1145,15 +1145,15 @@
         "effet": [0, 1, 9],
         "obtenu": [0, 5],
         "casqu": 0,
         "Ces": [0, 5, 9],
         "champ": 0,
         "libr": 0,
         "instant": 0,
-        "disponibl": [0, 7],
+        "disponibl": [0, 4, 7],
         "elles": 0,
         "cod": 0,
         "laiss": 0,
         "d\u00e9faut": [0, 7],
         "\u00eate": 0,
         "satisf": 0,
         "sais": [0, 4],
@@ -1273,15 +1273,15 @@
         "sup\u00e9rieur": 9,
         "inf\u00e9rieur": 9,
         "sp\u00e9cif": 5,
         "publi": 5,
         "AI": 5,
         "n\u00e9": [],
         "jusqu": 5,
-        "Des": 5,
+        "Des": [4, 5],
         "nuanc": 5,
         "integr": 5,
         "ia_supr": 5,
         "ia_insert": 5,
         "48": 5,
         "74": 5,
         "44": 5,
@@ -1477,15 +1477,27 @@
         "montr": 9,
         "quatr": 9,
         "affichent": 9,
         "couleur": 9,
         "marquent": 9,
         "masquent": 9,
         "pointill": 9,
-        "veil": 9
+        "veil": 9,
+        "downloaded": [],
+        "sourceforg": 2,
+        "net": [],
+        "project": [],
+        "environnment": [],
+        "practicing": [],
+        "onlin": [],
+        "video": [],
+        "tutorial": [],
+        "youtub": 4,
+        "tutoriel": 4,
+        "vid\u00e9o": 4
     },
     "objects": {},
     "objtypes": {},
     "objnames": {},
     "titleterms": {
         "generating": [],
         "cas": 0,
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/threshold_search.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/threshold_search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Recherche du seuil &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Recherche du seuil &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/user_interface.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/user_interface.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Interface utilisateur &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Interface utilisateur &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -30,15 +30,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/html_fr/virtual_listener.html` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/html_fr/virtual_listener.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="fr" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Sujet virtuel &mdash; Documentation audiometry_trainer 0.1.5</title>
+  <title>Sujet virtuel &mdash; Documentation audiometry_trainer 0.1.6</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
         <script src="_static/jquery.js"></script>
         <script src="_static/underscore.js"></script>
         <script src="_static/_sphinx_javascript_frameworks_compat.js"></script>
@@ -31,15 +31,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             audiometry_trainer
           </a>
               <div class="version">
-                0.1.5
+                0.1.6
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Rechercher docs" aria-label="Rechercher docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -88,15 +88,15 @@
 <div class="math notranslate nohighlight" id="logistic-psychometric-function">
 <span id="equation-logistic-psychometric-function"></span><span class="eqno">(2)<a class="headerlink" href="#logistic-psychometric-function" title="Lien permanent vers cette équation"></a></span>\[\psi(x;\alpha,\beta,\gamma,\lambda)  = \gamma + (1-\gamma - \lambda) \left(\frac{1}{1+e^{\beta(\alpha-x)}}\right)\]</div>
 <p>où <span class="math notranslate nohighlight">\(\alpha\)</span> est le point médian, <span class="math notranslate nohighlight">\(\beta\)</span> la pente, <span class="math notranslate nohighlight">\(\gamma\)</span> l’asymptote inférieur, et <span class="math notranslate nohighlight">\(\lambda\)</span> l’asymptote supérieur de la CP; <span class="math notranslate nohighlight">\(x\)</span> est le niveau du stimulus auquel la fonction est évaluée.</p>
 <p>La figure <a class="reference internal" href="#fig-logistic-psy"><span class="std std-ref">Courbes psychométriques logistiques</span></a> montre des exemples de CPs logistiques qui représentent la proportion de réponses « Oui » en fonction du niveau du stimulus. Tous les quatre panneaux affichent la même CP en noise avec une CP de couleur différent qui a A) un point médian différent, B) une pente, et ainsi une largeur, différentes, C) un asymptote inférieur différent, ou D) un asymptote supérieur différent. Les lignes verticales dans A) marquent les points médians des courbes, tandis que dans B) elle masquent la « largeur » de 5% à 95% de réponses « Oui » pour les deux courbes. Les lignes horizontales en pointillé marquent dans tous les panneaux la proportion de réponses correctes au point médian, veillez noter que cela change dans C) et D) en fonction de l’asymptote.</p>
 <figure class="align-default" id="id8">
 <span id="fig-logistic-psy"></span><a class="reference internal image-reference" href="_images/logistic_psy.fr.png"><img alt="Courbes psychométriques logistiques" src="_images/logistic_psy.fr.png" style="width: 675.0px; height: 675.0px;" /></a>
 <figcaption>
-<p><span class="caption-number">Fig. 2 </span><span class="caption-text">Courbes psychométriques logistiques</span><a class="headerlink" href="#id8" title="Lien permanent vers cette image"></a></p>
+<p><span class="caption-number">Fig. 3 </span><span class="caption-text">Courbes psychométriques logistiques</span><a class="headerlink" href="#id8" title="Lien permanent vers cette image"></a></p>
 </figcaption>
 </figure>
 <p>Le point médian est le niveau du stimulus auquel la CP atteigne la moitié de son amplitude, donc pour un sujet virtuel avec <span class="math notranslate nohighlight">\(\gamma = 0\)</span> and <span class="math notranslate nohighlight">\(\lambda=0\)</span>, le point médian <span class="math notranslate nohighlight">\(\alpha\)</span> est le niveau du stimulus auquel le sujet donne (sur la longue durée) 50% de réponses « Oui ». La procédure Hughson-Westlake défini le seuil comme le point le plus bas auquel le sujet donne au moins 50% de réponses « Oui » (sur au moins 3 essais). Par conséquent, le seuil (comme défini avec la procédure Hughson-Westlake) se situera généralement à un point égal ou supérieur du point médian <span class="math notranslate nohighlight">\(\alpha\)</span> <a class="reference internal" href="references.html#marshallandjesteadt1986" id="id3"><span>[MarshallAndJesteadt1986]</span></a>. C’est tout à fait possible que occasionnellement un seuil soit mesuré à un niveau plus bas que ça car la proportion de réponses « Oui » qu’on retrouve sur un petit nombre d’essais peut être bien différente que la proportion de réponses « Oui » qui sont attendues sur le long terme.</p>
 <p>La pente <span class="math notranslate nohighlight">\(\beta\)</span> règle la vitesse à laquelle la CP augmente de sa valeur la plus basse à la plus haute avec l’augmenter du niveau du stimulus. Plutôt de raisonner en termes de pente c’est souvent plus intuitif de raisonner en termes de la « largeur » de la CP (<a class="reference internal" href="references.html#alcala-quintanaandgarcia-perez2004" id="id4"><span>[Alcalá-QuintanaAndGarcía-Pérez2004]</span></a>; <a class="reference internal" href="references.html#kussetal2005" id="id5"><span>[KussEtAl2005]</span></a>), qui est corrélée de façon inverse à la pente. <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code> requiert de l’utilisateur la largeur à 90% désirée de la CP pour la génération de fichiers de cas. Par exemple, une largeur de 5 dB indique que la fonction (pour un sujet virtuel avec  <span class="math notranslate nohighlight">\(\gamma = 0\)</span> and <span class="math notranslate nohighlight">\(\lambda=0\)</span>)  varie d’une probabilité de réponse « Oui » de 5% à 95% avec un changement du niveau du stimulus de 5 dB.</p>
 <p>L’asymptote inférieur, <span class="math notranslate nohighlight">\(\gamma\)</span>, représente la tendance du sujet à répondre « Oui », même en l’absence de stimulation. Cette tendance n’est pas mesurée de façon formelle dans l’audiométrie clinique <a class="reference internal" href="references.html#barr-hamiltonetal1969" id="id6"><span>[Barr-HamiltonEtAl1969]</span></a> <a class="reference internal" href="references.html#marshallandjesteadt1986" id="id7"><span>[MarshallAndJesteadt1986]</span></a>. Dans une tâche de type Oui/Non avec des essais marqués temporellement, dans lesquels un signal est présenté ou pas, elle serait équivalente au taux de fausses alarmes. Par exemple, un sujet avec un <span class="math notranslate nohighlight">\(\gamma\)</span> de 0.1 répondrait « Oui » dans 1 fois sur 10 dans des essais dans lesquels il n’y avait pas de stimulation. Sous la perspective de la théorie de la détection du signal cette tendance à répondre « Oui » traduit un critère interne qui peut être plus ou moins prudent. Bien que l’estimation de <span class="math notranslate nohighlight">\(\gamma\)</span> nécessite des essais sans signal, ce critère détermine le processus de décision aussi quand un signal est présent, donc la valeur de <span class="math notranslate nohighlight">\(\gamma\)</span> aura une influence sur la CP sous-jacente la procédure d’audiométrie clinique.</p>
 <p>L’asymptote supérieur, <span class="math notranslate nohighlight">\(\lambda\)</span>, est le taux d’inattention ; il représente la tendance du sujet à rater des réponses à cause de manques d’attention, même pour un stimulus qui est clairement audible.</p>
 <p>Lors du masquage clinique avec <code class="docutils literal notranslate"><span class="pre">audiometry_trainer</span></code>, l’effet du bruit est de déplacer le point médian de la CP, <em>si</em> le niveau du bruit qui arrive à la cochlée, en dB de masquage effectif (« effective masking »; EM), dépasse le point médian de la CP. Le déplacement est égal au niveau par lequel le bruit dépasse le point médian. Par exemple, si le niveau du bruit est 5 dB au dessus du point médian non masqué, le point médian masqué sera 5 dB plus haut.</p>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _a_u_d_i_o_m_e_t_r_y___t_r_a_i_n_e_r
-0.1.5
+0.1.6
 [q                   ]
 Table des matières :
     * _I_n_t_r_o_d_u_c_t_i_o_n
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _R_e_c_h_e_r_c_h_e_ _d_u_ _s_e_u_i_l
     * _M_a_s_q_u_a_g_e
     * _S_u_j_e_t_ _v_i_r_t_u_e_l
@@ -33,15 +33,15 @@
 un asymptote supérieur différent. Les lignes verticales dans A) marquent les
 points médians des courbes, tandis que dans B) elle masquent la « largeur » de
 5% à 95% de réponses « Oui » pour les deux courbes. Les lignes horizontales en
 pointillé marquent dans tous les panneaux la proportion de réponses correctes
 au point médian, veillez noter que cela change dans C) et D) en fonction de
 l’asymptote.
 _[_C_o_u_r_b_e_s_ _p_s_y_c_h_o_m_é_t_r_i_q_u_e_s_ _l_o_g_i_s_t_i_q_u_e_s_]
-Fig. 2 Courbes psychométriques logistiques_
+Fig. 3 Courbes psychométriques logistiques_
 Le point médian est le niveau du stimulus auquel la CP atteigne la moitié de
 son amplitude, donc pour un sujet virtuel avec \(\gamma = 0\) and \
 (\lambda=0\), le point médian \(\alpha\) est le niveau du stimulus auquel le
 sujet donne (sur la longue durée) 50% de réponses « Oui ». La procédure
 Hughson-Westlake défini le seuil comme le point le plus bas auquel le sujet
 donne au moins 50% de réponses « Oui » (sur au moins 3 essais). Par conséquent,
 le seuil (comme défini avec la procédure Hughson-Westlake) se situera
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf`

 * *Files 10% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex/audiometry_trainer.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20240410152419+02'00'"
+CreationDate: "D:20240424204410+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240410152419+02'00'"
+ModDate: "D:20240424204410+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'audiometry_trainer'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,13 +1,13 @@
 audiometry_trainer
-Release 0.1.5
+Release 0.1.6
 
 Samuele Carcagno
 
-Apr 10, 2024
+Apr 24, 2024
 
 Contents:
 
 1
 
 Introduction
 
@@ -70,39 +70,42 @@
 i
 
 1
 Introduction
 
 audiometry_trainer is a software for practicing clinical audiometry. The software simulates
 patient’s responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure Screenshot of
-the audiometry_trainer interface shows the main window of audiometry_trainer.
+the audiometry_trainer interface shows the main window of audiometry_trainer. Online
+video tutorials are available on Youtube.
 
 Fig. 1.1: Screenshot of the audiometry_trainer interface
 At startup audiometry_trainer selects a random virtual patient case file (you can load other
-case files from the File menu). The S marker in the audiogram window shows the current
-stimulus level. The threshold search is more conveniently conducted using the keyboard rather
-than via mouse button presses. Press the space bar to play the stimulus (the Stimulus light
-at the bottom will light up). If the virtual patient heard the stimulus the Response light on
-the left side will light up. Use the up/down arrows to change the stimulus level. Once you’ve
-found the threshold, press the T key to mark it on the audiogram plot. Use the right/left arrow
+case files from the File menu).
+The S marker in the audiogram window shows the current stimulus frequency and level. The
+threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the Stimulus light at the bottom will
 1
 
-audiometry_trainer, Release 0.1.5
-keys to move to another frequency.
+audiometry_trainer, Release 0.1.6
+
+Fig. 1.2: File menu
+light up). If the virtual patient heard the stimulus the Response light on the left side will light
+up. Use the up/down arrow keys to change the stimulus level. Once you’ve found the threshold,
+press the T key to mark it on the audiogram plot. Use the right/left arrow keys to move to another
+frequency.
 You can compare the thresholds that you’ve estimated with the actual expected thresholds by using the Show actual thresholds checkboxes at the bottom of the left panel. Virtual patients
 are modeled via psychometric functions and the “actual” thresholds are computed via Monte
 Carlo simulations: they are the median thresholds obtained over a large number of simulations;
 95% confidence intervals can be shown by checking the CI checkboxes.
-You can move from right to left era and from air to bone conduction stimulation by selecting the
+You can move from right to left ear and from air to bone conduction stimulation by selecting the
 desired options in the drop-down menus for Channel 1 at the top of the left panel. Channel 2
 is used to deliver masking noise. To turn on Channel 2 check the Chan. 2 ON check box on
 the right panel, a M marker on the audiogram window will indicate the masking noise level. You
 can use the Chan. 2 level box and the up/down arrows on its right to set the masker level.
 You can also lock the Channel 1 and Channel 2 levels using the Lock Channels checkbox
-on the left panel; when the channels are locked increasing/decreasing the stimulus level by a
+on the right panel; when the channels are locked increasing/decreasing the stimulus level by a
 given amount will automatically change the masker level by the the same amount.
 A detailed description of all the features of audiometry_trainer will be given in the next
 sections. Section Installation tells how to obtain and install audiometry_trainer. Sections
 Threshold search and Masking explain how to perform a threshold search and how to use masking, respectively.
 audiometry_trainer uses psychometric functions to model virtual patient responses. Responses are not deterministic (always yes/no above/below a given stimulus level) but probabilistic, with the probability of a response increasing with the stimulus level. This adds realism to
 the software because in real life the responses of patients are not deterministic. Section Virtual
 listener details the psychometric function model used by audiometry_trainer.
@@ -115,32 +118,34 @@
 
 2
 
 2
 Installation
 
 audiometry_trainer has been successfully installed and used on Linux and Windows. It
-should also work on Mac platforms, but this has not been tested. A dedicated installer is provided
-for Windows. On Linux and Mac (and Windows if you do not wish to use the dedicated installer)
+should also work on Mac platforms, but this has not been tested. For Windows, a dedicated
+installer can be downloaded from SourceForge.
+On Linux and Mac (but also on Windows if you do not wish to use the dedicated installer)
 audiometry_trainer, which is written in Python, can be installed via the Python package
 installer pip:
 pip install audiometry-trainer
 audiometry_trainer depends on a few Python modules including:
 • PyQt5
 • numpy
 • scipy
 • matplotlib
 • pandas
 depending on your Python distribution you may want to install these dependecies before installing audiometry_trainer via pip (e.g. through conda if you’re using the Anaconda
 Python distribution, or through your Linux distribution package manager if you’re using the
 Python installation that comes with your Linux distribution), otherwise pip will attempt to automatically pull in and install these dependencies. If the program is successfully installed you
 should be able to start it from a bash/DOS terminal with the command:
 audiometry_trainer
-You need to ensure that the Python environment you’re using when you call the above command
-matches the one you used when you installed the application.
+If you use multiple Python installations/environnments, you need to make sure that the Python
+environment you’re using when you call the above command matches the one you used when
+you installed the application.
 
 3
 
 3
 Threshold search
 
 The S marker in the audiogram window shows the current stimulus level. You can use the
@@ -171,15 +176,15 @@
 using the automatic thresholds to then move on to determine if masking is needed, and if so
 measure the masked thresholds.
 The Show estimated thresholds checkboxes can be used to show/hide the thresholds that
 have been measured. By default all the measured thresholds are shown on the audiogram, but
 sometimes this generates clutter (e.g. when masked thresholds are obtained after unmasked
 4
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 ones) and it may be useful to hide some of the estimated thresholds.
 You can compare the thresholds that you’ve estimated with the actual expected thresholds by using the Show actual thresholds checkboxes at the bottom of the left panel. Virtual patients
 are modeled via psychometric functions (see Section Virtual listener) and the “actual” thresholds are computed via Monte Carlo simulations (see Section Generating case files), therefore,
 exact matches to the estimated thresholds should not always be expected, but they should generally be very close.They “actual” thresholds are the median thresholds obtained over a large
 number of simulations; 95% confidence intervals for these thresholds can be shown by checking
 the CI checkboxes.
 
@@ -206,15 +211,15 @@
 Interaural attenuation (IA) values for supra-aural and insert earphones are drawn randomly for
 each case from a uniform distribution. The lower and upper limits of the distribution are frequency specific and are based on the min/max IA values reported by [MunroAndAgnew1999].
 For frquencies that were not tested in [MunroAndAgnew1999] the values of an adjacent frequency are used. The lower and upper values of the uniform distribution as a function of
 frequency are shown in Table table-IA_supra for supra-aural earphones and in Table tableIA_insert for insert earphones.
 
 6
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 
 Table 4.1: Lower and upper limits of the uniform distribution
 for IA for supra-aural headphones.
 Freq.
 Low High
 125 Hz
 48
@@ -279,15 +284,15 @@
 4000 Hz ([Studebaker1967]; [Gelfand2016]). More nuanced data on IA for BC are available
 [Stenfelt2012] and may be integrated to future versions of audiometry_trainer.
 
 4.1. Interaural attenuation
 
 7
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 
 Table 4.3: Lower and upper limits of the uniform distribution
 for IA for bone conduction.
 Freq.
 Low High
 125 Hz
 0
@@ -360,15 +365,15 @@
 10
 1000 Hz 2
 10
 4.2. Occlusion effect
 
 8
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 The OE is absent when a conductive/mixed hearing with an air-bone gap (ABG) >= 20 dB is
 present [MartinEtAl1974]. For this reason, if there is an ABG >= 20 dB the OE is set to zero.
 For ABGs between 0 and 20 dB the size of the OE is scaled by the ABG using the following
 equation:
 𝑂𝐸𝑜𝑢𝑡 = 𝑂𝐸𝑖𝑛𝑝 − 𝑂𝐸𝑖𝑛𝑝 (𝐴𝐵𝐺/20)
 
 (4.1)
@@ -409,15 +414,15 @@
 unmasked TE BC threshold is genuine, underestimating the OE will be of no consequence; the
 TE had the lowest threshold to start with, so undermasking will simply confirm, “in the wrong
 way”, a correct decision that that threshold was coming from the TE. If the estimated OE is used
 4.2. Occlusion effect
 
 9
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 for a full-blown masked threshold search, the masked TE BC threshold may be lower than the
 unmasked one because the NTE will be undermasked.
 
 4.3 Central masking
 audiometry_trainer simulates central masking effects by increasing the TE threshold when
 the level of the masking noise at the NTE is audible to the virtual patient. The size of the central
 masking effect drawn randomly for each virtual listener and each frequency from a folded normal
@@ -462,21 +467,21 @@
 stimulus level increases. Rather than reasoning in terms of slope, it is often more intuitive to reason in terms of “width” of the PF ([Alcalá-QuintanaAndGarcía-Pérez2004]; [KussEtAl2005]),
 which is inversely correlated with the slope. audiometry_trainer asks the user the desired
 90% width of the PF in order to generate case files. For example, a width of 5 dB indicates that
 the function (for a virtual listener with 𝛾 = 0 and 𝜆 = 0) goes from 5% to 95% probability of a
 “Yes” response within a change in stimulus level of 5 dB.
 11
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 
 Fig. 5.1: Logistic psychometric functions
 
 12
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 The lower asymptote, 𝛾, represents the propensity of the listener to respond “Yes”, even in the
 absence of a stimulus. This propensity is not formally measured in the clinical audiometry
 procedure [Barr-HamiltonEtAl1969] [MarshallAndJesteadt1986]. In a Yes/No task with temporally marked trials, in which a signal is presented or not, it would correspond to the false alarm
 rate. For example, a listener with a 𝛾 of 0.1 would respond “Yes” in 1 out of 10 trials in which
 no stimulus was presented. Under the perspective of signal detection theory this propensity of
 the listener to say “Yes” reflects an internal criterion which can be more or less conservative.
 Although the actual measurement of 𝛾 requires “blank” trials without a signal, the criterion determines the decision process also when a signal is present, hence the value of 𝛾 will affect the
@@ -531,15 +536,15 @@
 be found, on average, at 45 dB HL. This is simply an example and variations of each of the PF
 parameters (midpoint, width, F.A. rate and lapse rate) could be used to obtain a virtual listener
 with the same threshold but a different response behavior. Empirically, the region of uncertainty
 between inaudibility and certain detection in clinical audiometry has been found to be around
 10 dB wide [Barr-HamiltonEtAl1969], therefore PF widths of around 10 dB should result in
 14
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 relatively realistic virtual listeners.
 To simulate a conductive/mixed hearing loss simply set the ABG to the desired value of the
 conductive component. The AC PF midpoint will be shifted by the ABG with respect to the BC
 PF midpoint.
 In addition to the BC and ABG PF parameters there are two columns, Gain R and Gain L that
 represent the gain of a hearing aid worn by the virtual listener. The values in these columns do
 not have any influence on the listener’s responses to stimuli delivered via earphones or via the
@@ -640,15 +645,15 @@
 Speech and Hearing Disorders, 39(2), 148–152. https://doi.org/10.1044/jshd.3902.
 148
 [MunroAndAgnew1999] Munro, K. J., & Agnew, N. (1999). A comparison of inter-aural attenuation with the Etymotic ER-3A insert earphone and the Telephonies TDH39 supra-aural earphone. British Journal of Audiology, 33(4), 259–262. https:
 //doi.org/10.3109/03005369909090106
 [Stenfelt2012] Stenfelt, S. (2012). Transcranial Attenuation of Bone-Conducted Sound When
 Stimulation Is at the Mastoid and at the Bone Conduction Hearing Aid Po19
 
-audiometry_trainer, Release 0.1.5
+audiometry_trainer, Release 0.1.6
 sition. Otology & Neurotology, 33(2), 105–114. https://doi.org/10.1097/MAO.
 0b013e31823e28ab
 [Studebaker1967] Studebaker, G. A. (1967). Clinical masking of the nontest ear. The Journal of
 Speech and Hearing Disorders, 32(4), 360–371. https://doi.org/10.1044/jshd.3204.
 360
 [Turner2004] Turner, R. G. (2004). Masking Redux II: A Recommended Masking Protocol.
 Journal of the American Academy of Audiology, 15(01), 029–046. https://doi.org/
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf`

 * *Files 13% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/_build/latex_fr/audiometry_trainer.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: 'Samuele Carcagno'
-CreationDate: "D:20240410152438+02'00'"
+CreationDate: "D:20240424204416+02'00'"
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: "D:20240410152438+02'00'"
+ModDate: "D:20240424204416+02'00'"
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.24 (TeX Live 2022/Debian) kpathsea version 6.3.4'
 Producer: 'pdfTeX-1.40.24'
 Subject: ''
 Title: 'audiometry_trainer'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,111 +1,114 @@
 audiometry_trainer
-Version 0.1.5
+Version 0.1.6
 
 Samuele Carcagno
 
-avr. 10, 2024
+avr. 24, 2024
 
 Table des matières :
 
 1
 
 Introduction
 
 1
 
 2
 
 Installation
 
-3
+4
 
 3
 
 Recherche du seuil
 
-4
+5
 
 4
 
 Masquage
-6
-4.1 Atténuation interaurale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
-4.2 Effet d’occlusion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 8
-4.3 Masquage central . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
+7
+4.1 Atténuation interaurale . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
+4.2 Effet d’occlusion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
+4.3 Masquage central . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
 
 5
 
 Sujet virtuel
 
-11
+12
 
 6
 
 Générer des fichiers de cas
 
-14
+15
 
 7
 
 Interface utilisateur
 
-16
+17
 
 8
 
 Fonctionnement interne
 
-17
+18
 
 9
 
 Index et tableaux
 
-18
+19
 
 Bibliographie
 
-19
+20
 
 i
 
 1
 Introduction
 
 audiometry_trainer est un logiciel pour s’entraîner à l’audiométrie clinique. Le logiciel simule les réponses de patients depuis des fichiers de cas et permet de pratiquer des aspects essentiels de la procédure, y compris la recherche de seuil par voie aérienne/osseuse et le masquage
 clinique. La figure Capture d’écran de la fenêtre principale de audiometry_trainer affiche la
-fenêtre principale de audiometry_trainer.
+fenêtre principale de audiometry_trainer. Des tutoriels vidéo sont disponible sur Youtube.
 
 Fig. 1.1 – Capture d’écran de la fenêtre principale de audiometry_trainer
-Au démarrage audiometry_trainer sélectionne de façon aléatoire un fichier de cas d’un patient virtuel (vous pouvez charger d’autres cas depuis le menu Fichier). Le marqueur S affiché
-dans la fenêtre de l’audiogramme indique le niveau courant du stimulus. C’est plus pratique
-d’effectuer la recherche du seuil avec le clavier qu’un utilisant la souris pour cliquer sur des
-boutons. Appuyez sur la barre d’espace pour jouer le stimulus (le Témoin du stimulus en bas
-s’allumera). Si le patient virtuel a entendu le stimulus le Témoin de réponse sur la gauche
-s’allumera. Utilisez les flèches haut/bas pour changer le niveau du stimulus. Lorsque vous avez
+Au démarrage audiometry_trainer sélectionne de façon aléatoire un fichier de cas de patient
+virtuel (vous pouvez charger d’autres cas depuis le menu Fichier).
+Le marqueur S affiché dans la fenêtre de l’audiogramme indique la fréquence et le niveau courants du stimulus. C’est plus pratique d’effectuer la recherche du seuil avec le clavier qu’en
+cliquant sur des boutons avec la souris. Appuyez sur la barre d’espace pour jouer le stimulus
+(le Témoin du stimulus en bas s’allumera). Si le patient virtuel a entendu le son le Témoin
 1
 
-audiometry_trainer, Version 0.1.5
-trouvé le seuil marquez-le en appuyant sur la touche T (de l’anglais « Threshold »). Utilisez les
-flèches droite/gauche pour vous déplacer sur une autre fréquence.
+audiometry_trainer, Version 0.1.6
+
+Fig. 1.2 – Fichier menu
+de réponse sur la gauche s’allumera. Utilisez les flèches haut/bas du clavier pour changer le
+niveau du stimulus. Lorsque vous avez trouvé le seuil, marquez-le en appuyant sur la touche T
+(de l’anglais « Threshold »). Utilisez les flèches droite/gauche du clavier pour vous déplacer sur
+une autre fréquence.
 Vous pouvez comparer les seuils que vous avez mesuré avec les seuils attendus en cochant les
 cases sous Affichage des vrais seuils dans la partie basse du panneau de gauche. Les
 patients virtuels sont modelés à travers des courbes psychométriques et les « vrais » seuils sont
 calculés à travers des méthodes de Monte-Carlo : ils sont les seuils médians obtenus sur un large
 nombre de simulations ; des intervalles de confiance de 95% peuvent être affichés en cochant
 les cases CI.
 Vous pouvez passer de l’oreille droite à la gauche et de la stimulation en conduction aérienne
 à celle en conduction osseuse en sélectionnant les options souhaitées dans les menus déroulant
 pour le Canal 1 en haut du panneau de gauche. Le Canal 2 est utilisé pour envoyer du bruit
 masquant. Pour allumer le Canal 2 cochez la case Can. 2 ON sur le panneau de droite, un
 marqueur M dans la fenêtre de l’audiogramme affichera le niveau courant du bruit masquant.
 Vous pouvez utiliser la case Niveau du can. 2 ainsi que les flèches haut/bas à sa droite pour
 saisir le niveau du bruit masquant. Vous pouvez aussi « verrouiller » le Canal 2 au Canal 1 en
-cochant la case Verrouiller les canaux sur le panneau de gauche : lorsque les canaux sont
+cochant la case Verrouiller les canaux sur le panneau de droite : lorsque les canaux sont
 verrouillés, des augmentations/baisses du niveau du stimulus d’une taille donné déclencheront
 automatiquement des changements du niveau du masqueur de la même taille.
 Une description détaillée de toutes les fonctionnalités de audiometry_trainer sera donne
 dans les sections suivantes. La Section Installation explique comment obtenir et installer
 audiometry_trainer. Les sections Recherche du seuil and Masquage expliquent comment
 faire une recherche de seuil et comment utiliser le masquage, respectivement.
 audiometry_trainer utilise des courbes psychométriques pour modéliser les réponses des
@@ -114,43 +117,47 @@
 réelle les réponses des patients ne sont pas déterministes. La section Sujet virtuel détaille le
 modèle de courbe psychométrique utilisé par audiometry_trainer.
 audiometry_trainer vous permet de générer et utiliser vous propres fichiers de cas. Vous
 pouvez accéder à cette fonctionnalité à travers l’action Générer un cas sous le menu Fichier
 et ça sera illustré en détails dans la Section Générer des fichiers de cas. Quelques connaissances
 du modèle de fonction psychométrique utilisé par audiometry_trainer seront nécessaires
 pour la création de vos propres fichiers de cas.
+2
+
+audiometry_trainer, Version 0.1.6
 La Section Interface utilisateur couvre en détail toute l’interface utilisateur. La Section Fonctionnement interne décrits quelques aspects du fonctionnement interne du logiciel et est adressée
 aux développeurs plutôt qu’aux utilisateurs du logiciel.
 
-2
+3
 
 2
 Installation
 
-audiometry_trainer a été installé et utilisé avec succès sur Linux et Windows. Il devrait aussi
-marcher sur des ordinateurs Mac, mais cela n’a pas été testé. Pour Windows il y a un programme
-d’installation dédié. Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser
-le programme d’installation dédié) audiometry_trainer, qui est écrit en Python, peut être
-installé à travers pip :
+audiometry_trainer a été installé et utilisé avec succès sur Linux et Windows. Il devrait
+aussi marcher sur des ordinateurs Mac, mais cela n’a pas été testé. Pour Windows, vous pouvez
+télécharger un programme d’installation dédié sur SourceForge.
+Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser le programme
+d’installation dédié) audiometry_trainer, qui est écrit en Python, peut être installé à travers
+pip :
 pip install audiometry-trainer
 audiometry_trainer dépend d’un petit nombre de modules Python y compris :
 — PyQt5
 — numpy
 — scipy
 — matplotlib
 — pandas
 selon votre distribution il pourrait être souhaitable d’installer ces dépendances avant d’installer
 audiometry_trainer à travers pip (par exemple à travers conda si vous utilisez la distribution de Python Anaconda, ou à travers votre gestionnaire de paquets de Linux si vous utilisez
 l’installation de Python de votre distribution Linux), sinon pip essayera de télécharger et installer ces dépendances de façon automatique. Si le programme est installé avec succès vous devriez
 pouvoir le lancer depuis un terminal bash/DOS avec la commande :
 audiometry_trainer
-Vous devez vous assurer que l’environnement de Python que vous employez quand vous utilisez la commande ci-dessus correspond à celui que vous aviez utilisé lors de l’installation de
-l’application.
+Si vous utilisez plusieurs installations/environnements de Python, vous devez vous assurer que
+l’environnement de Python que vous employez quand vous utilisez la commande ci-dessus correspond à celui que vous aviez utilisé lors de l’installation de l’application.
 
-3
+4
 
 3
 Recherche du seuil
 
 Le marqueur S dans la fenêtre de l’audiogramme indique la niveau courant du stimulus. Vous
 pouvez utiliser les flèches haut/bas de votre clavier pour changer le niveau du stimulus et les
 flèches droit/gauche pour changer sa fréquence. Vous pouvez présenter le stimulus au sujet virtuel en appuyant sur la barre espace (le Témoin du stimulus en bas s’allumera). Si le sujet
@@ -175,32 +182,32 @@
 Le bouton Rech. seuil automatique exécute une recherche automatique du seuil avec la
 procédure Hughson-Westlake pour toutes les fréquences en utilisant le transducteur courant
 pour le canal 1. Cette recherche automatique du seuil est disponible uniquement pour la mesure
 des seuils non masqués. Cette fonctionnalité a été ajouté parce que l’aspect le plus intéressant
 de l’audiométrie est la mesure des seuils masqués (s’ils sont nécessaires), donc en utilisant la
 recherche automatique on peut vite obtenir les seuils non-masqués pour ensuite déterminer si
 le masquage est nécessaire et mesurer les seuils masqués le cas échéant.
-Les cases Afficher les seuils estimés peuvent être cochées/décochées pour affi4
+Les cases Afficher les seuils estimés peuvent être cochées/décochées pour affi5
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 cher/cacher les seuils qui ont été mesurés. Par défaut tous les seuils mesurés sont affichés sur
 l’audiogramme, mais parfois cela génère de l’encombrement (par ex. lorsque les seuils masqués
 sont obtenus après les seuils non-masqués) et il peut s’avérer utile de cacher certains des seuils
 mesurés.
 Vous pouvez cocher les cases Afficher les vrais seuils en bas du panneau gauche pour
 comparer les seuils que vous avez mesuré avec les « vrais » seuils attendus. Les patients virtuels
 sont modélisés à partir de courbes psychométriques (voir la section Sujet virtuel) et les « vrai »
 seuils sont calculés à travers une méthode de Monte-Carlo (voir la section Générer des fichiers
 de cas), par conséquent, on ne doit pas s’attendre que le seuils mesurés et le seuils attendus soit
 parfaitement égal, mais il devraient être généralement très proches. Les « vrais » seuils sont le
 seuils médians obtenus sur un grand nombre de simulations ; des intervalles de confiance de
 95% pour ces seuils peuvent être affichés en cochant les cases CI.
 
-5
+6
 
 4
 Masquage
 
 Pour masquer l’oreille non testée (ONT) pendant l’audiométrie par conduction aérienne fixez
 le Niveau du can. 2 à la valeur que vous souhaitez et assurez-vous que la case Can. 2 ON
 soit cochée.
@@ -217,17 +224,17 @@
 
 4.1 Atténuation interaurale
 Le valeurs d’atténuation interaurale (AI) pour le casque supra-aural et pour l” écouter de type
 insert sont tirés de façon aléatoire d’une distribution uniforme. Les limites inférieure et supérieure et de cette distribution sont spécifiques à chaque fréquence et sont basés sur les valeurs publiés par [MunroAndAgnew1999]. Pour les fréquences qui n’ont pas été testées par
 [MunroAndAgnew1999] les valeurs d’un fréquence proche ont été utilisées. Les limites inférieure et supérieure de cette distribution en fonction de la fréquence sont affichées dans le tableau
 table-IA_supra pour le casque supra-aural et dans le tableau table-IA_insert pour l’écouter insert.
 
-6
+7
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 Tableau 4.1 – Limites inférieure et supérieure de la distribution uniforme pour l’atténuation interaurale pour le casque
 supra-aural.
 Fréq.
 Inférieur Supérieur
 125 Hz
 48
@@ -290,17 +297,17 @@
 que l’AI pour la stimulation en CO est essentiellement néante à 250 Hz et augmente jusqu’à
 environ 15 dB à 4000 Hz ([Studebaker1967] ; [Gelfand2016]). Des données plus nuancées sur
 l’AI en CO ont été publiées [Stenfelt2012] et pourraient être intégrées à des versions futurs de
 audiometry_trainer.
 
 4.1. Atténuation interaurale
 
-7
+8
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 Tableau 4.3 – Limites inférieure et supérieure de la distribution uniforme pour l’atténuation interaurale en conduction
 osseuse.
 Fréq.
 Inférieur Supérieur
 125 Hz
 0
@@ -353,17 +360,17 @@
 8
 26
 1000 Hz 4
 12
 
 4.2. Effet d’occlusion
 
-8
+9
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 Tableau 4.5 – Limites inférieure et supérieure de la distribution uniforme pour l’effet d’occlusion pour l’écouter insert.
 Pour des fréquences > 1000 Hz l’effet d’occlusion est toujours zéro.
 Fréq.
 Inférieur Supérieur
 125 Hz
 2
@@ -410,17 +417,17 @@
 à celui obtenu avec l’ONT nue pour estimer la taille de l’EO [MartinEtAl1974]. Pour obtenir de seuils en CO avec l’ONT couverte par le casque, mais sans que ce dernier envoie du
 bruit, dans audiometry_trainer vous devez mettre l” État de l'oreille non testée
 sur l’option Écouter sur l'oreille et vous assurer que la case Can. 2 ON ne soit pas cochée. La taille de l’effet d’occlusion mesurée de cette façon dépendra du transducteur sélectionné
 pour le Canal 2 (casque supra-aural ou écouter insert), donc assurez-vous d’avoir sélectionné
 le même transducteur que vous allez utiliser plus tard pour le masquage.
 4.2. Effet d’occlusion
 
-9
+10
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 Une limitation de cette technique est que dans certains cas elle peut sous-estimer la taille de
 l’EO ([FagelsonAndMartin1994] ; [Yacullo1997]). Cela peut arriver dans le cas d’un sujet avec
 un seuil en CO pour l’ONT qui est proche de la limite inférieure de la sortie de l’ossivibrateur.
 Par exemple, si le sujet a un seuil en CO proche de 0 dB HL et l’ossivibrateur a une limite de
 sortie inférieure de -20 dB HL, des EOs supérieurs à 20 dB seraient sous-estimés. Cela peut aussi
 arriver si le seuil en CO de l’OT est inférieur au seuil en CO de l’ONT. Par exemple, supposez
@@ -440,15 +447,15 @@
 La taille de cet effet de masquage central est tirée de façon aléatoire pour chaque sujet virtuel et
 chaque fréquence d’une distribution normale repliée avec une moyenne de zéro et une déviation
 standard de 3. Cela est basé sur l’observation que les effets de masquage central sont typiquement
 petits, de l’ordre de 5 dB [Yacullo1997].
 
 4.3. Masquage central
 
-10
+11
 
 5
 Sujet virtuel
 
 Les réponses du sujet virtuel sont déterminées à partir d’une courbe psychométrique (CP) qui
 représente la proportion de réponses « Oui » (j’ai entendu un son) en fonction du niveau du
 stimulus. Une fonction logistique ([KussEtAl2005] ; [KingdomAndPrins2016]) est utilisée :
@@ -477,23 +484,23 @@
 mesuré à un niveau plus bas que ça car la proportion de réponses « Oui » qu’on retrouve sur un
 petit nombre d’essais peut être bien différente que la proportion de réponses « Oui » qui sont
 attendues sur le long terme.
 La pente 𝛽 règle la vitesse à laquelle la CP augmente de sa valeur la plus basse à
 la plus haute avec l’augmenter du niveau du stimulus. Plutôt de raisonner en termes
 de pente c’est souvent plus intuitif de raisonner en termes de la « largeur » de la CP
 ([Alcalá-QuintanaAndGarcía-Pérez2004] ; [KussEtAl2005]), qui est corrélée de façon inverse à
-11
+12
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 Fig. 5.1 – Courbes psychométriques logistiques
 
-12
+13
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 la pente. audiometry_trainer requiert de l’utilisateur la largeur à 90% désirée de la CP pour
 la génération de fichiers de cas. Par exemple, une largeur de 5 dB indique que la fonction (pour
 un sujet virtuel avec 𝛾 = 0 and 𝜆 = 0) varie d’une probabilité de réponse « Oui » de 5% à 95%
 avec un changement du niveau du stimulus de 5 dB.
 L’asymptote inférieur, 𝛾, représente la tendance du sujet à répondre « Oui », même en l’absence
 de stimulation. Cette tendance n’est pas mesurée de façon formelle dans l’audiométrie clinique
 [Barr-HamiltonEtAl1969] [MarshallAndJesteadt1986]. Dans une tâche de type Oui/Non avec
@@ -516,15 +523,15 @@
 marge de sécurité de 10 dB est généralement ajoutée pour le calcul du niveau de bruit dans les
 formules de masquage). Il faut remarquer que msk_diff peut être une valeur soit positive, soit
 négative. Une valeur de msk_diff positive signifie que l’effet de masquage est plus grand de
 l’effet moyen (le point médian de la CP est déplacé vers le haut), tandis qu’une valeur négative
 de msk_diff indique que l’effet de masquage est plus petit de l’effet moyen (le point médian
 de la CP est déplacé vers le bas).
 
-13
+14
 
 6
 Générer des fichiers de cas
 
 Pour générer un nouveau cas cliquez sur le menu Fichier et en suite sur Générer un cas.
 La fenêtre de génération de cas s’ouvrira. Les cas sont générés sur la base des paramètres
 de courbe psychométrique (CP) pour les seuils de conduction osseuse (CO) et du Rinne. Les
@@ -552,17 +559,17 @@
 réponses « Oui » entre 50% et 100%. Une largeur de 8 dB signifie que la CP ira de 5% à 95%
 dans l’espace de 8 dB, par conséquent elle ira du point médian (43 dB HL) à 95% de réponses
 « Oui » dans l’espace de 4 dB (la moitié de la largeur). Globalement, en utilisant ces paramètres
 le seuil se situera à 2 dB près de 45 dB HL. Vue que la taille de pas utilisée pour la recherche
 du seuil est de 5 dB, le seuil qu’en résultera se situera presque certainement, en moyenne, à 45
 dB HL. Ceci est juste un exemple et des variations de chacun des paramètres de la CP (point
 médian, largeur, taux de F.A. et taux d’inattention) pourraient êtres employées pour obtenir des
-14
+15
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 sujets virtuels avec le même seuils mais un comportement différent. Empiriquement, la région
 d’incertitude entre inaudibilité et détection certaine dans l’audiométrie clinique a été estimé être
 d’une largeur d’environ 10 dB [Barr-HamiltonEtAl1969], donc des largeurs de CP d’environ 10
 dB devrait résulter en des sujets virtuel assez réalistes.
 Pour simuler une perte de transmission/mixte vous pouvez simplement fixer le Rinne à la valeur
 souhaitée de la composante de transmission. Le point médian de la CP de CA sera déplacé de
@@ -593,22 +600,22 @@
 Les paramètres du sujet virtuel peuvent être enregistré pour ensuite être chargés à nouveau dans
 la fenêtre générer un cas en cliquant sur les actions Sauvegarder les paramètres et
 Charger les paramètres qui se trouvent sous le menu Fichier. Lorsque vous enregistré
 un fichier de paramètres, le texte qui se trouve dans la case Info du cas est enregistré dans
 un fichier de l’info du cas. Lorsque vous chargez un fichier de paramètres, le fichier de l’info du
 cas sera lui aussi chargé s’il se trouve dans le même dossier que le fichier de paramètres.
 
-15
+16
 
 7
 Interface utilisateur
 
 To be written. Please refer to the other sections for the time being.
 
-16
+17
 
 8
 Fonctionnement interne
 
 Estimated
 thresholds
 are
@@ -637,24 +644,24 @@
 these cases the stimulus level at which the cursor is located when marking the threshold will
 be stored in self.est_aud. The thresh_status key in the self.plot_prms dict allows to treat them
 differently according to the cases seen above.
 Another key stored in self.plot_prms is used to indicate whether points for a given transducer
 and masking status should be displayed on the plot or hidden :
 ` self.plot_prms['masked']['bone']['right']['visible'] `
 
-17
+18
 
 9
 Index et tableaux
 
 — genindex
 — modindex
 — search
 
-18
+19
 
 Bibliographie
 
 [Alcalá-QuintanaAndGarcía-Pérez2004] Alcalá-Quintana, R., & García-Pérez, M. A. (2004).
 The Role of Parametric Assumptions in Adaptive Bayesian Estimation. Psychological Methods, 9(2), 250–271. https://doi.org/10.1037/1082-989X.9.2.250
 [Barr-HamiltonEtAl1969] Barr-Hamilton, R. M., Bryan, M. E., & Tempest, W. (1969). Applications of Signal Detection Theory to Audiometry. International Audiology, 8(1),
 138–146. https://doi.org/10.3109/05384916909070201
@@ -674,25 +681,25 @@
 148
 [MunroAndAgnew1999] Munro, K. J., & Agnew, N. (1999). A comparison of inter-aural attenuation with the Etymotic ER-3A insert earphone and the Telephonies TDH-39
 supra-aural earphone. British Journal of Audiology, 33(4), 259–262. https://doi.org/
 10.3109/03005369909090106
 [Stenfelt2012] Stenfelt, S. (2012). Transcranial Attenuation of Bone-Conducted Sound When
 Stimulation Is at the Mastoid and at the Bone Conduction Hearing Aid Position. Otology & Neurotology, 33(2), 105–114. https://doi.org/10.1097/MAO.
 0b013e31823e28ab
-19
+20
 
-audiometry_trainer, Version 0.1.5
+audiometry_trainer, Version 0.1.6
 
 [Studebaker1967] Studebaker, G. A. (1967). Clinical masking of the nontest ear. The Journal of
 Speech and Hearing Disorders, 32(4), 360–371. https://doi.org/10.1044/jshd.3204.
 360
 [Turner2004] Turner, R. G. (2004). Masking Redux II : A Recommended Masking Protocol.
 Journal of the American Academy of Audiology, 15(01), 029–046. https://doi.org/
 10.3766/jaaa.15.1.5
 [Yacullo1997] Yacullo, W. S. (1997). Clinical masking procedures. Needham Heights : Allyn
 and Bacon.
 
 Bibliographie
 
-20
+21
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/audiometry_trainer.fr.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/audiometry_trainer.fr.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/audiometry_trainer.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/audiometry_trainer.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/conf.py` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 author = 'Samuele Carcagno'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = "0.1.5"
+version = "0.1.6"
 # The full version, including alpha/beta/rc tags.
-release = "0.1.5"
+release = "0.1.6"
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/generate_case.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/generate_case.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/index.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/index.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/installation.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/installation.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 .. _sec-installation:
 
 ************
 Installation
 ************
 
-``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. A dedicated installer is provided for Windows. On Linux and Mac (and Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
+``audiometry_trainer`` has been successfully installed and used on Linux and Windows. It should also work on Mac platforms, but this has not been tested. For Windows, a dedicated installer can be downloaded from `SourceForge <https://sourceforge.net/projects/audiometry-trainer/files/>`_.
+
+On Linux and Mac (but also on Windows if you do not wish to use the dedicated installer) ``audiometry_trainer``, which is written in Python, can be installed via the Python package installer ``pip``:
 
 .. code-block:: bash
 
 		pip install audiometry-trainer
 
 ``audiometry_trainer`` depends on a few Python modules including:
 
@@ -20,14 +22,14 @@
 
 depending on your Python distribution you may want to install these dependecies before installing ``audiometry_trainer`` via ``pip`` (e.g. through ``conda`` if you're using the Anaconda Python distribution, or through your Linux distribution package manager if you're using the Python installation that comes with your Linux distribution), otherwise ``pip`` will attempt to automatically pull in and install these dependencies. If the program is successfully installed you should be able to start it from a bash/DOS terminal with the command:
 
 .. code-block:: bash
 
 	audiometry_trainer
 
-You need to ensure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
+If you use multiple Python installations/environnments, you need to make sure that the Python environment you're using when you call the above command matches the one you used when you installed the application.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/internals.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/internals.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/intro.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/intro.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 .. _sec-intro:
 
 *************
 Introduction
 *************
 
-``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``.
+``audiometry_trainer`` is a software for practicing clinical audiometry. The software simulates patient's responses loaded from case files, and allows practicing essential aspects of the procedure including air/bone conduction threshold search and clinical masking. Figure :ref:`fig-audiometry_trainer_screenshot` shows the main window of ``audiometry_trainer``. Online video tutorials are available on `Youtube. <https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4>`_
 
 .. _fig-audiometry_trainer_screenshot:
 
 .. figure:: audiometry_trainer.png
    :scale: 50%
    :alt: Screenshot of the ``audiometry_trainer`` interface
 
    Screenshot of the ``audiometry_trainer`` interface
 
-At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``). The ``S`` marker in the audiogram window shows the current stimulus level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrows to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
+At startup ``audiometry_trainer`` selects a random virtual patient case file (you can load other case files from the ``File menu``).
+
+.. _fig-file_menu:
+
+.. figure:: file_menu.png
+   :scale: 100%
+   :alt: File menu
+
+   File menu
+   
+The ``S`` marker in the audiogram window shows the current stimulus frequency and level. The threshold search is more conveniently conducted using the keyboard rather than via mouse button presses. Press the space bar to play the stimulus (the ``Stimulus light`` at the bottom will light up). If the virtual patient heard the stimulus the ``Response light`` on the left side will light up. Use the up/down arrow keys to change the stimulus level. Once you've found the threshold, press the ``T`` key to mark it on the audiogram plot. Use the right/left arrow keys to move to another frequency.
 
 You can compare the thresholds that you've estimated with the actual expected thresholds by using the ``Show actual thresholds`` checkboxes at the bottom of the left panel. Virtual patients are modeled via psychometric functions and the "actual" thresholds are computed via Monte Carlo simulations: they are the median thresholds obtained over a large number of simulations; 95% confidence intervals can be shown by checking the ``CI`` checkboxes.
 
-You can move from right to left era and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the left panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
+You can move from right to left ear and from air to bone conduction stimulation by selecting the desired options in the drop-down menus for ``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box on the right panel, a ``M`` marker on the audiogram window will indicate the masking noise level. You can use the ``Chan. 2 level`` box and the up/down arrows on its right to set the masker level. You can also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox on the right panel; when the channels are locked increasing/decreasing the stimulus level by a given amount will automatically change the masker level by the the same amount.
 
 A detailed description of all the features of ``audiometry_trainer`` will be given in the next sections. Section :ref:`sec-installation` tells how to obtain and install ``audiometry_trainer``. Sections :ref:`sec-threshold_search` and :ref:`sec-masking` explain how to perform a threshold search and how to use masking, respectively.
 
 ``audiometry_trainer`` uses psychometric functions to model virtual patient responses. Responses are not deterministic (always yes/no above/below a given stimulus level) but probabilistic, with the probability of a response increasing with the stimulus level. This adds realism to the software because in real life the responses of patients are not deterministic. Section :ref:`sec-virtual_listener` details the psychometric function model used by ``audiometry_trainer``.
 
 ``audiometry_trainer`` allows you to create and use your own case files. This functionality can be accessed via the ``Generate case`` button under the ``File menu`` and will be described in detail in Section :ref:`sec-generate_case`. Some knowledge of the psychometric function model used by ``audiometry_trainer`` will be needed to create your own case files.
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.mo`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/generate_case.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.mo`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,52 +1,59 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: audiometry_trainer 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-04-07 10:32+0200\n"
+"PO-Revision-Date: 2024-04-12 11:39+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "Generated-By: Babel 2.10.3\n"
 "X-Generator: Poedit 3.2.2\n"
 
+msgid ""
+"If you use multiple Python installations/environnments, you need to make "
+"sure that the Python environment you're using when you call the above "
+"command matches the one you used when you installed the application."
+msgstr ""
+"Si vous utilisez plusieurs installations/environnements de Python, vous "
+"devez vous assurer que l'environnement de Python que vous employez quand "
+"vous utilisez la commande ci-dessus correspond à celui que vous aviez "
+"utilisé lors de l'installation de l'application."
+
 msgid "Installation"
 msgstr "Installation"
 
 msgid ""
-"You need to ensure that the Python environment you're using when you call "
-"the above command matches the one you used when you installed the "
-"application."
+"On Linux and Mac (but also on Windows if you do not wish to use the "
+"dedicated installer) ``audiometry_trainer``, which is written in Python, can "
+"be installed via the Python package installer ``pip``:"
 msgstr ""
-"Vous devez vous assurer que l'environnement de Python que vous employez "
-"quand vous utilisez la commande ci-dessus correspond à celui   que vous "
-"aviez utilisé lors de l'installation de l'application."
+"Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser "
+"le programme d'installation dédié) ``audiometry_trainer``, qui est écrit en "
+"Python, peut être installé à travers ``pip``:"
 
 msgid "``audiometry_trainer`` depends on a few Python modules including:"
 msgstr ""
 "``audiometry_trainer`` dépend d'un petit nombre de modules Python y compris :"
 
 msgid ""
 "``audiometry_trainer`` has been successfully installed and used on Linux and "
 "Windows. It should also work on Mac platforms, but this has not been tested. "
-"A dedicated installer is provided for Windows. On Linux and Mac (and Windows "
-"if you do not wish to use the dedicated installer) ``audiometry_trainer``, "
-"which is written in Python, can be installed via the Python package "
-"installer ``pip``:"
+"For Windows, a dedicated installer can be downloaded from `SourceForge "
+"<https://sourceforge.net/projects/audiometry-trainer/files/>`_."
 msgstr ""
 "``audiometry_trainer`` a été installé et utilisé avec succès sur Linux et "
 "Windows. Il devrait aussi marcher sur des ordinateurs Mac, mais cela n'a pas "
-"été testé. Pour Windows il y a un programme d'installation dédié. Sur Linux "
-"et Mac (mais aussi sur Windows si vous ne souhaitez pas utiliser le "
-"programme d'installation dédié) ``audiometry_trainer``, qui est écrit en "
-"Python, peut être installé à travers ``pip``:"
+"été testé. Pour Windows, vous pouvez télécharger un programme d'installation "
+"dédié sur `SourceForge <https://sourceforge.net/projects/audiometry-trainer/"
+"files/>`_."
 
 msgid ""
 "depending on your Python distribution you may want to install these "
 "dependecies before installing ``audiometry_trainer`` via ``pip`` (e.g. "
 "through ``conda`` if you're using the Anaconda Python distribution, or "
 "through your Linux distribution package manager if you're using the Python "
 "installation that comes with your Linux distribution), otherwise ``pip`` "
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/installation.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: audiometry_trainer 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-07 10:29+0200\n"
-"PO-Revision-Date: 2024-04-07 10:32+0200\n"
+"POT-Creation-Date: 2024-04-12 11:39+0200\n"
+"PO-Revision-Date: 2024-04-12 11:39+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -24,53 +24,61 @@
 msgid "Installation"
 msgstr "Installation"
 
 #: ../../installation.rst:7
 msgid ""
 "``audiometry_trainer`` has been successfully installed and used on Linux "
 "and Windows. It should also work on Mac platforms, but this has not been "
-"tested. A dedicated installer is provided for Windows. On Linux and Mac "
-"(and Windows if you do not wish to use the dedicated installer) "
-"``audiometry_trainer``, which is written in Python, can be installed via "
-"the Python package installer ``pip``:"
+"tested. For Windows, a dedicated installer can be downloaded from "
+"`SourceForge <https://sourceforge.net/projects/audiometry-trainer/files/"
+">`_."
 msgstr ""
 "``audiometry_trainer`` a été installé et utilisé avec succès sur Linux "
 "et Windows. Il devrait aussi marcher sur des ordinateurs Mac, mais cela "
-"n'a pas été testé. Pour Windows il y a un programme d'installation "
-"dédié. Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas "
+"n'a pas été testé. Pour Windows, vous pouvez télécharger un programme "
+"d'installation dédié sur `SourceForge <https://sourceforge.net/projects/"
+"audiometry-trainer/files/>`_."
+
+#: ../../installation.rst:9
+msgid ""
+"On Linux and Mac (but also on Windows if you do not wish to use the "
+"dedicated installer) ``audiometry_trainer``, which is written in Python, "
+"can be installed via the Python package installer ``pip``:"
+msgstr ""
+"Sur Linux et Mac (mais aussi sur Windows si vous ne souhaitez pas "
 "utiliser le programme d'installation dédié) ``audiometry_trainer``, qui "
 "est écrit en Python, peut être installé à travers ``pip``:"
 
-#: ../../installation.rst:13
+#: ../../installation.rst:15
 msgid "``audiometry_trainer`` depends on a few Python modules including:"
 msgstr ""
 "``audiometry_trainer`` dépend d'un petit nombre de modules Python y "
 "compris :"
 
-#: ../../installation.rst:15
+#: ../../installation.rst:17
 msgid "PyQt5"
 msgstr ""
 
-#: ../../installation.rst:16
+#: ../../installation.rst:18
 msgid "numpy"
 msgstr ""
 
-#: ../../installation.rst:17
+#: ../../installation.rst:19
 msgid "scipy"
 msgstr ""
 
-#: ../../installation.rst:18
+#: ../../installation.rst:20
 msgid "matplotlib"
 msgstr ""
 
-#: ../../installation.rst:19
+#: ../../installation.rst:21
 msgid "pandas"
 msgstr ""
 
-#: ../../installation.rst:21
+#: ../../installation.rst:23
 msgid ""
 "depending on your Python distribution you may want to install these "
 "dependecies before installing ``audiometry_trainer`` via ``pip`` (e.g. "
 "through ``conda`` if you're using the Anaconda Python distribution, or "
 "through your Linux distribution package manager if you're using the "
 "Python installation that comes with your Linux distribution), otherwise "
 "``pip`` will attempt to automatically pull in and install these "
@@ -82,16 +90,17 @@
 "(par exemple à travers ``conda`` si vous utilisez la distribution de "
 "Python Anaconda, ou à travers votre gestionnaire de paquets de Linux si "
 "vous utilisez l'installation de Python de votre distribution Linux), "
 "sinon ``pip`` essayera de télécharger et installer ces dépendances de "
 "façon automatique. Si le programme est installé avec succès vous devriez "
 "pouvoir le lancer depuis un terminal bash/DOS avec la commande :"
 
-#: ../../installation.rst:27
+#: ../../installation.rst:29
 msgid ""
-"You need to ensure that the Python environment you're using when you "
-"call the above command matches the one you used when you installed the "
-"application."
-msgstr ""
-"Vous devez vous assurer que l'environnement de Python que vous employez "
-"quand vous utilisez la commande ci-dessus correspond à celui   que vous "
-"aviez utilisé lors de l'installation de l'application."
+"If you use multiple Python installations/environnments, you need to make "
+"sure that the Python environment you're using when you call the above "
+"command matches the one you used when you installed the application."
+msgstr ""
+"Si vous utilisez plusieurs installations/environnements de Python, vous "
+"devez vous assurer que l'environnement de Python que vous employez quand "
+"vous utilisez la commande ci-dessus correspond à celui que vous aviez "
+"utilisé lors de l'installation de l'application."
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/internals.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: audiometry_trainer 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2024-04-08 19:15+0200\n"
+"PO-Revision-Date: 2024-04-24 20:40+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -25,36 +25,22 @@
 "ref:`sec-installation` explique comment obtenir et installer "
 "``audiometry_trainer``. Les sections :ref:`sec-threshold_search` and :ref:"
 "`sec-masking` expliquent comment faire une recherche de seuil et comment "
 "utiliser le masquage, respectivement."
 
 msgid ""
 "At startup ``audiometry_trainer`` selects a random virtual patient case file "
-"(you can load other case files from the ``File menu``). The ``S`` marker in "
-"the audiogram window shows the current stimulus level. The threshold search "
-"is more conveniently conducted using the keyboard rather than via mouse "
-"button presses. Press the space bar to play the stimulus (the ``Stimulus "
-"light`` at the bottom will light up). If the virtual patient heard the "
-"stimulus the ``Response light`` on the left side will light up. Use the up/"
-"down arrows to change the stimulus level. Once you've found the threshold, "
-"press the ``T`` key to mark it on the audiogram plot. Use the right/left "
-"arrow keys to move to another frequency."
+"(you can load other case files from the ``File menu``)."
 msgstr ""
 "Au démarrage ``audiometry_trainer`` sélectionne de façon aléatoire un "
-"fichier de cas d'un patient virtuel (vous pouvez charger d'autres cas depuis "
-"le menu ``Fichier``). Le marqueur ``S`` affiché dans la fenêtre de "
-"l'audiogramme indique le niveau courant du stimulus. C'est plus pratique "
-"d'effectuer la recherche du seuil avec le clavier qu'un utilisant la souris "
-"pour cliquer sur des boutons. Appuyez sur la barre d'espace pour jouer le "
-"stimulus (le ``Témoin du stimulus`` en bas s'allumera). Si le patient "
-"virtuel a entendu le stimulus le ``Témoin de réponse`` sur la gauche "
-"s'allumera. Utilisez les flèches haut/bas pour changer le niveau du "
-"stimulus. Lorsque vous avez trouvé le seuil marquez-le en appuyant sur la "
-"touche ``T`` (de l'anglais \"Threshold\"). Utilisez les flèches droite/"
-"gauche pour vous déplacer sur une autre fréquence."
+"fichier de cas de patient virtuel (vous pouvez charger d'autres cas depuis "
+"le menu ``Fichier``). "
+
+msgid "File menu"
+msgstr "Fichier menu"
 
 msgid "Introduction"
 msgstr "Introduction"
 
 msgid "Screenshot of the ``audiometry_trainer`` interface"
 msgstr "Capture d'écran de la fenêtre principale de ``audiometry_trainer``"
 
@@ -65,14 +51,35 @@
 msgstr ""
 "La Section :ref:`sec-user_interface` couvre en détail toute l'interface "
 "utilisateur. La Section :ref:`sec-internals` décrits quelques aspects du "
 "fonctionnement interne du logiciel et est adressée aux développeurs plutôt "
 "qu'aux utilisateurs du logiciel."
 
 msgid ""
+"The ``S`` marker in the audiogram window shows the current stimulus "
+"frequency and level. The threshold search is more conveniently conducted "
+"using the keyboard rather than via mouse button presses. Press the space bar "
+"to play the stimulus (the ``Stimulus light`` at the bottom will light up). "
+"If the virtual patient heard the stimulus the ``Response light`` on the left "
+"side will light up. Use the up/down arrow keys to change the stimulus level. "
+"Once you've found the threshold, press the ``T`` key to mark it on the "
+"audiogram plot. Use the right/left arrow keys to move to another frequency."
+msgstr ""
+"Le marqueur ``S`` affiché dans la fenêtre de l'audiogramme indique la "
+"fréquence et le niveau courants du stimulus. C'est plus pratique d'effectuer "
+"la recherche du seuil avec le clavier qu'en cliquant sur des boutons avec la "
+"souris. Appuyez sur la barre d'espace pour jouer le stimulus (le ``Témoin du "
+"stimulus`` en bas s'allumera). Si le patient virtuel a entendu le son le "
+"``Témoin de réponse`` sur la gauche s'allumera. Utilisez les flèches haut/"
+"bas du clavier pour changer le niveau du stimulus. Lorsque vous avez trouvé "
+"le seuil, marquez-le en appuyant sur la touche ``T`` (de l'anglais "
+"\"Threshold\"). Utilisez les flèches droite/gauche du clavier pour vous "
+"déplacer sur une autre fréquence."
+
+msgid ""
 "You can compare the thresholds that you've estimated with the actual "
 "expected thresholds by using the ``Show actual thresholds`` checkboxes at "
 "the bottom of the left panel. Virtual patients are modeled via psychometric "
 "functions and the \"actual\" thresholds are computed via Monte Carlo "
 "simulations: they are the median thresholds obtained over a large number of "
 "simulations; 95% confidence intervals can be shown by checking the ``CI`` "
 "checkboxes."
@@ -82,37 +89,37 @@
 "partie basse du panneau de gauche. Les patients virtuels sont modelés à "
 "travers des courbes psychométriques et les \"vrais\" seuils sont calculés à "
 "travers des méthodes de Monte-Carlo : ils sont les seuils médians obtenus "
 "sur un large nombre de simulations ; des intervalles de confiance de 95% "
 "peuvent être affichés en cochant les cases ``CI``."
 
 msgid ""
-"You can move from right to left era and from air to bone conduction "
+"You can move from right to left ear and from air to bone conduction "
 "stimulation by selecting the desired options in the drop-down menus for "
 "``Channel 1`` at the top of the left panel. ``Channel 2`` is used to deliver "
 "masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` check box "
 "on the right panel, a ``M`` marker on the audiogram window will indicate the "
 "masking noise level. You can use the ``Chan. 2 level`` box and the up/down "
 "arrows on its right to set the masker level. You can also ``lock`` the "
 "``Channel 1`` and ``Channel 2`` levels using the ``Lock Channels`` checkbox "
-"on the left panel; when the channels are locked increasing/decreasing the "
+"on the right panel; when the channels are locked increasing/decreasing the "
 "stimulus level by a given amount will automatically change the masker level "
 "by the the same amount."
 msgstr ""
 "Vous pouvez passer de l'oreille droite à la gauche et de la stimulation en "
 "conduction aérienne à celle en conduction osseuse en sélectionnant les "
 "options souhaitées dans les menus déroulant pour le ``Canal 1`` en haut du "
 "panneau de gauche. Le ``Canal 2`` est utilisé pour envoyer du bruit "
 "masquant. Pour allumer le ``Canal 2`` cochez la case ``Can. 2 ON`` sur le "
 "panneau de droite, un marqueur ``M`` dans la fenêtre de l'audiogramme "
 "affichera le niveau courant du bruit masquant. Vous pouvez utiliser la case "
 "``Niveau du can. 2`` ainsi que les flèches haut/bas à sa droite pour saisir "
 "le niveau du bruit masquant. Vous pouvez aussi \"verrouiller\" le ``Canal "
 "2`` au ``Canal 1`` en cochant la case ``Verrouiller les canaux`` sur le "
-"panneau de gauche : lorsque les canaux sont verrouillés, des augmentations/"
+"panneau de droite : lorsque les canaux sont verrouillés, des augmentations/"
 "baisses du niveau du stimulus d'une taille donné déclencheront "
 "automatiquement des changements du niveau du masqueur de la même taille."
 
 msgid ""
 "``audiometry_trainer`` allows you to create and use your own case files. "
 "This functionality can be accessed via the ``Generate case`` button under "
 "the ``File menu`` and will be described in detail in Section :ref:`sec-"
@@ -128,22 +135,25 @@
 
 msgid ""
 "``audiometry_trainer`` is a software for practicing clinical audiometry. The "
 "software simulates patient's responses loaded from case files, and allows "
 "practicing essential aspects of the procedure including air/bone conduction "
 "threshold search and clinical masking. Figure :ref:`fig-"
 "audiometry_trainer_screenshot` shows the main window of "
-"``audiometry_trainer``."
+"``audiometry_trainer``. Online video tutorials are available on `Youtube. "
+"<https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4>`_"
 msgstr ""
 "``audiometry_trainer`` est un logiciel pour s'entraîner à l'audiométrie "
 "clinique. Le logiciel simule les réponses de patients depuis des fichiers de "
 "cas et permet de pratiquer des aspects essentiels de la procédure, y compris "
 "la recherche de seuil par voie aérienne/osseuse et le masquage clinique. La "
 "figure :ref:`fig-audiometry_trainer_screenshot` affiche la fenêtre "
-"principale de ``audiometry_trainer``."
+"principale de ``audiometry_trainer``. Des tutoriels vidéo sont disponible "
+"sur `Youtube. <https://www.youtube.com/playlist?"
+"list=PLyfCl_MBfnRBh7CLE48BeawkZpKODle1X>`_"
 
 msgid ""
 "``audiometry_trainer`` uses psychometric functions to model virtual patient "
 "responses. Responses are not deterministic (always yes/no above/below a "
 "given stimulus level) but probabilistic, with the probability of a response "
 "increasing with the stimulus level. This adds realism to the software "
 "because in real life the responses of patients are not deterministic. "
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/intro.po`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2024.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: audiometry_trainer 0.0.1\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2024-04-07 18:29+0200\n"
-"PO-Revision-Date: 2024-04-08 19:15+0200\n"
+"POT-Creation-Date: 2024-04-24 20:39+0200\n"
+"PO-Revision-Date: 2024-04-24 20:40+0200\n"
 "Last-Translator: \n"
 "Language-Team: \n"
 "Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -27,56 +27,69 @@
 #: ../../intro.rst:7
 msgid ""
 "``audiometry_trainer`` is a software for practicing clinical audiometry. "
 "The software simulates patient's responses loaded from case files, and "
 "allows practicing essential aspects of the procedure including air/bone "
 "conduction threshold search and clinical masking. Figure :ref:`fig-"
 "audiometry_trainer_screenshot` shows the main window of "
-"``audiometry_trainer``."
+"``audiometry_trainer``. Online video tutorials are available on "
+"`Youtube. <https://www.youtube.com/playlist?"
+"list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4>`_"
 msgstr ""
 "``audiometry_trainer`` est un logiciel pour s'entraîner à l'audiométrie "
 "clinique. Le logiciel simule les réponses de patients depuis des "
 "fichiers de cas et permet de pratiquer des aspects essentiels de la "
 "procédure, y compris la recherche de seuil par voie aérienne/osseuse et "
 "le masquage clinique. La figure :ref:`fig-audiometry_trainer_screenshot` "
-"affiche la fenêtre principale de ``audiometry_trainer``."
+"affiche la fenêtre principale de ``audiometry_trainer``. Des tutoriels "
+"vidéo sont disponible sur `Youtube. <https://www.youtube.com/playlist?"
+"list=PLyfCl_MBfnRBh7CLE48BeawkZpKODle1X>`_"
 
 #: ../../intro.rst:15
 msgid "Screenshot of the ``audiometry_trainer`` interface"
 msgstr "Capture d'écran de la fenêtre principale de ``audiometry_trainer``"
 
 #: ../../intro.rst:17
 msgid ""
 "At startup ``audiometry_trainer`` selects a random virtual patient case "
-"file (you can load other case files from the ``File menu``). The ``S`` "
-"marker in the audiogram window shows the current stimulus level. The "
-"threshold search is more conveniently conducted using the keyboard "
-"rather than via mouse button presses. Press the space bar to play the "
-"stimulus (the ``Stimulus light`` at the bottom will light up). If the "
-"virtual patient heard the stimulus the ``Response light`` on the left "
-"side will light up. Use the up/down arrows to change the stimulus level. "
-"Once you've found the threshold, press the ``T`` key to mark it on the "
-"audiogram plot. Use the right/left arrow keys to move to another "
-"frequency."
+"file (you can load other case files from the ``File menu``)."
 msgstr ""
 "Au démarrage ``audiometry_trainer`` sélectionne de façon aléatoire un "
-"fichier de cas d'un patient virtuel (vous pouvez charger d'autres cas "
-"depuis le menu ``Fichier``). Le marqueur ``S`` affiché dans la fenêtre "
-"de l'audiogramme indique le niveau courant du stimulus. C'est plus "
-"pratique d'effectuer la recherche du seuil avec le clavier qu'un "
-"utilisant la souris pour cliquer sur des boutons. Appuyez sur la barre "
-"d'espace pour jouer le stimulus (le ``Témoin du stimulus`` en bas "
-"s'allumera). Si le patient virtuel a entendu le stimulus le ``Témoin de "
-"réponse`` sur la gauche s'allumera. Utilisez les flèches haut/bas pour "
-"changer le niveau du stimulus. Lorsque vous avez trouvé le seuil marquez-"
-"le en appuyant sur la touche ``T`` (de l'anglais \"Threshold\"). "
-"Utilisez les flèches droite/gauche pour vous déplacer sur une autre "
+"fichier de cas de patient virtuel (vous pouvez charger d'autres cas "
+"depuis le menu ``Fichier``). "
+
+#: ../../intro.rst:25
+msgid "File menu"
+msgstr "Fichier menu"
+
+#: ../../intro.rst:27
+msgid ""
+"The ``S`` marker in the audiogram window shows the current stimulus "
+"frequency and level. The threshold search is more conveniently conducted "
+"using the keyboard rather than via mouse button presses. Press the space "
+"bar to play the stimulus (the ``Stimulus light`` at the bottom will "
+"light up). If the virtual patient heard the stimulus the ``Response "
+"light`` on the left side will light up. Use the up/down arrow keys to "
+"change the stimulus level. Once you've found the threshold, press the "
+"``T`` key to mark it on the audiogram plot. Use the right/left arrow "
+"keys to move to another frequency."
+msgstr ""
+"Le marqueur ``S`` affiché dans la fenêtre de l'audiogramme indique la "
+"fréquence et le niveau courants du stimulus. C'est plus pratique "
+"d'effectuer la recherche du seuil avec le clavier qu'en cliquant sur des "
+"boutons avec la souris. Appuyez sur la barre d'espace pour jouer le "
+"stimulus (le ``Témoin du stimulus`` en bas s'allumera). Si le patient "
+"virtuel a entendu le son le ``Témoin de réponse`` sur la gauche "
+"s'allumera. Utilisez les flèches haut/bas du clavier pour changer le "
+"niveau du stimulus. Lorsque vous avez trouvé le seuil, marquez-le en "
+"appuyant sur la touche ``T`` (de l'anglais \"Threshold\"). Utilisez les "
+"flèches droite/gauche du clavier pour vous déplacer sur une autre "
 "fréquence."
 
-#: ../../intro.rst:19
+#: ../../intro.rst:29
 #, python-format
 msgid ""
 "You can compare the thresholds that you've estimated with the actual "
 "expected thresholds by using the ``Show actual thresholds`` checkboxes "
 "at the bottom of the left panel. Virtual patients are modeled via "
 "psychometric functions and the \"actual\" thresholds are computed via "
 "Monte Carlo simulations: they are the median thresholds obtained over a "
@@ -87,59 +100,59 @@
 "attendus en cochant les cases sous ``Affichage des vrais seuils`` dans "
 "la partie basse du panneau de gauche. Les patients virtuels sont modelés "
 "à travers des courbes psychométriques et les \"vrais\" seuils sont "
 "calculés à travers des méthodes de Monte-Carlo : ils sont les seuils "
 "médians obtenus sur un large nombre de simulations ; des intervalles de "
 "confiance de 95% peuvent être affichés en cochant les cases ``CI``."
 
-#: ../../intro.rst:21
+#: ../../intro.rst:31
 msgid ""
-"You can move from right to left era and from air to bone conduction "
+"You can move from right to left ear and from air to bone conduction "
 "stimulation by selecting the desired options in the drop-down menus for "
 "``Channel 1`` at the top of the left panel. ``Channel 2`` is used to "
 "deliver masking noise. To turn on ``Channel 2`` check the ``Chan. 2 ON`` "
 "check box on the right panel, a ``M`` marker on the audiogram window "
 "will indicate the masking noise level. You can use the ``Chan. 2 level`` "
 "box and the up/down arrows on its right to set the masker level. You can "
 "also ``lock`` the ``Channel 1`` and ``Channel 2`` levels using the "
-"``Lock Channels`` checkbox on the left panel; when the channels are "
+"``Lock Channels`` checkbox on the right panel; when the channels are "
 "locked increasing/decreasing the stimulus level by a given amount will "
 "automatically change the masker level by the the same amount."
 msgstr ""
 "Vous pouvez passer de l'oreille droite à la gauche et de la stimulation "
 "en conduction aérienne à celle en conduction osseuse en sélectionnant "
 "les options souhaitées dans les menus déroulant pour le ``Canal 1`` en "
 "haut du panneau de gauche. Le ``Canal 2`` est utilisé pour envoyer du "
 "bruit masquant. Pour allumer le ``Canal 2`` cochez la case ``Can. 2 ON`` "
 "sur le panneau de droite, un marqueur ``M`` dans la fenêtre de "
 "l'audiogramme affichera le niveau courant du bruit masquant. Vous pouvez "
 "utiliser la case ``Niveau du can. 2`` ainsi que les flèches haut/bas à "
 "sa droite pour saisir le niveau du bruit masquant. Vous pouvez aussi "
 "\"verrouiller\" le ``Canal 2`` au ``Canal 1`` en cochant la case "
-"``Verrouiller les canaux`` sur le panneau de gauche : lorsque les canaux "
+"``Verrouiller les canaux`` sur le panneau de droite : lorsque les canaux "
 "sont verrouillés, des augmentations/baisses du niveau du stimulus d'une "
 "taille donné déclencheront automatiquement des changements du niveau du "
 "masqueur de la même taille."
 
-#: ../../intro.rst:23
+#: ../../intro.rst:33
 msgid ""
 "A detailed description of all the features of ``audiometry_trainer`` "
 "will be given in the next sections. Section :ref:`sec-installation` "
 "tells how to obtain and install ``audiometry_trainer``. Sections :ref:"
 "`sec-threshold_search` and :ref:`sec-masking` explain how to perform a "
 "threshold search and how to use masking, respectively."
 msgstr ""
 "Une description détaillée de toutes les fonctionnalités de "
 "``audiometry_trainer`` sera donne dans les sections suivantes. La "
 "Section :ref:`sec-installation` explique comment obtenir et installer "
 "``audiometry_trainer``. Les sections :ref:`sec-threshold_search` and :"
 "ref:`sec-masking` expliquent comment faire une recherche de seuil et "
 "comment utiliser le masquage, respectivement."
 
-#: ../../intro.rst:25
+#: ../../intro.rst:35
 msgid ""
 "``audiometry_trainer`` uses psychometric functions to model virtual "
 "patient responses. Responses are not deterministic (always yes/no above/"
 "below a given stimulus level) but probabilistic, with the probability of "
 "a response increasing with the stimulus level. This adds realism to the "
 "software because in real life the responses of patients are not "
 "deterministic. Section :ref:`sec-virtual_listener` details the "
@@ -150,15 +163,15 @@
 "déterministes (toujours oui/non au dessus/dessous d'un certain niveau de "
 "stimulation) mais probabilistes, avec une probabilité de réponse "
 "croissante en fonction du niveau de stimulation. Cela rends le logiciel "
 "plus réaliste car dans la vie réelle les réponses des patients ne sont "
 "pas déterministes. La section :ref:`sec-virtual_listener` détaille le "
 "modèle de courbe psychométrique utilisé par ``audiometry_trainer``."
 
-#: ../../intro.rst:27
+#: ../../intro.rst:37
 msgid ""
 "``audiometry_trainer`` allows you to create and use your own case files. "
 "This functionality can be accessed via the ``Generate case`` button "
 "under the ``File menu`` and will be described in detail in Section :ref:"
 "`sec-generate_case`. Some knowledge of the psychometric function model "
 "used by ``audiometry_trainer`` will be needed to create your own case "
 "files."
@@ -167,18 +180,45 @@
 "fichiers de cas. Vous pouvez accéder à cette fonctionnalité à travers "
 "l'action ``Générer un cas`` sous le menu ``Fichier`` et ça sera illustré "
 "en détails dans la Section :ref:`sec-generate_case`. Quelques "
 "connaissances du modèle de fonction psychométrique utilisé par "
 "``audiometry_trainer`` seront nécessaires pour la création de vos "
 "propres fichiers de cas."
 
-#: ../../intro.rst:29
+#: ../../intro.rst:39
 msgid ""
 "Section :ref:`sec-user_interface` covers in details all the user "
 "interface. Section :ref:`sec-internals` describes some of the internals "
 "of the software and is mainly intended for developers rather than for "
 "end users."
 msgstr ""
 "La Section :ref:`sec-user_interface` couvre en détail toute l'interface "
 "utilisateur. La Section :ref:`sec-internals` décrits quelques aspects du "
 "fonctionnement interne du logiciel et est adressée aux développeurs "
 "plutôt qu'aux utilisateurs du logiciel."
+
+#~ msgid ""
+#~ "At startup ``audiometry_trainer`` selects a random virtual patient "
+#~ "case file (you can load other case files from the ``File menu``). The "
+#~ "``S`` marker in the audiogram window shows the current stimulus "
+#~ "level. The threshold search is more conveniently conducted using the "
+#~ "keyboard rather than via mouse button presses. Press the space bar to "
+#~ "play the stimulus (the ``Stimulus light`` at the bottom will light "
+#~ "up). If the virtual patient heard the stimulus the ``Response light`` "
+#~ "on the left side will light up. Use the up/down arrows to change the "
+#~ "stimulus level. Once you've found the threshold, press the ``T`` key "
+#~ "to mark it on the audiogram plot. Use the right/left arrow keys to "
+#~ "move to another frequency."
+#~ msgstr ""
+#~ "Au démarrage ``audiometry_trainer`` sélectionne de façon aléatoire un "
+#~ "fichier de cas d'un patient virtuel (vous pouvez charger d'autres cas "
+#~ "depuis le menu ``Fichier``). Le marqueur ``S`` affiché dans la "
+#~ "fenêtre de l'audiogramme indique le niveau courant du stimulus. C'est "
+#~ "plus pratique d'effectuer la recherche du seuil avec le clavier qu'un "
+#~ "utilisant la souris pour cliquer sur des boutons. Appuyez sur la "
+#~ "barre d'espace pour jouer le stimulus (le ``Témoin du stimulus`` en "
+#~ "bas s'allumera). Si le patient virtuel a entendu le stimulus le "
+#~ "``Témoin de réponse`` sur la gauche s'allumera. Utilisez les flèches "
+#~ "haut/bas pour changer le niveau du stimulus. Lorsque vous avez trouvé "
+#~ "le seuil marquez-le en appuyant sur la touche ``T`` (de l'anglais "
+#~ "\"Threshold\"). Utilisez les flèches droite/gauche pour vous déplacer "
+#~ "sur une autre fréquence."
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.mo`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/masking.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.mo`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.mo` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.mo`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.po` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.po`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/logistic_psy.fr.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/logistic_psy.fr.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/logistic_psy.png` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/logistic_psy.png`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/make.bat` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/make.bat`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/masking.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/masking.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/references.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/references.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/threshold_search.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/threshold_search.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/doc/virtual_listener.rst` & `audiometry_trainer-0.1.6/audiometry_trainer/doc/virtual_listener.rst`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/global_parameters.py` & `audiometry_trainer-0.1.6/audiometry_trainer/global_parameters.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/hughson_westlake.py` & `audiometry_trainer-0.1.6/audiometry_trainer/hughson_westlake.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/main_window.py` & `audiometry_trainer-0.1.6/audiometry_trainer/main_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,23 +19,23 @@
 
 import matplotlib, os, platform, random, time
 matplotlib.rcParams['path.simplify'] = False
 import matplotlib.ticker as ticker
 
 if pyqtversion == 5:
     from PyQt5 import QtGui, QtCore
-    from PyQt5.QtCore import Qt, QEvent
+    from PyQt5.QtCore import Qt, QEvent, QUrl
     from PyQt5.QtGui import QDesktopServices, QDoubleValidator, QIcon, QIntValidator, QPainter
     from PyQt5.QtWidgets import QAction, QApplication, QCheckBox, QColorDialog, QComboBox, QDesktopWidget, QFileDialog, QFrame, QGridLayout, QHBoxLayout, QInputDialog, QLabel, QLayout, QLineEdit, QMainWindow, QMessageBox, QPushButton, QSizePolicy, QSpacerItem, QSpinBox, QSplitter, QTextEdit, QToolTip, QVBoxLayout, QWhatsThis, QWidget
     from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
     from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
     matplotlib.rcParams['backend'] = "Qt5Agg"
 elif pyqtversion == 6:
     from PyQt6 import QtGui, QtCore
-    from PyQt6.QtCore import Qt, QEvent
+    from PyQt6.QtCore import Qt, QEvent, QUrl
     from PyQt6.QtGui import QAction, QDesktopServices, QDoubleValidator, QIcon, QIntValidator, QPainter
     from PyQt6.QtWidgets import QApplication, QCheckBox, QColorDialog, QComboBox, QFileDialog, QFrame, QGridLayout, QHBoxLayout, QInputDialog, QLabel, QLayout, QLineEdit, QMainWindow, QMessageBox, QPushButton, QSizePolicy, QSpacerItem, QSpinBox, QSplitter, QTextEdit, QToolTip, QVBoxLayout, QWhatsThis, QWidget
     from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg as FigureCanvas
     from matplotlib.backends.backend_qt5agg import NavigationToolbar2QT as NavigationToolbar
     matplotlib.rcParams['backend'] = "Qt5Agg"
     
 # Matplotlib Figure object
@@ -166,58 +166,62 @@
         self.fig = Figure(facecolor=self.canvasColor, dpi=self.dpi, figsize=(20, 15), constrained_layout=True)
         self.ylims = (-25, 125)
         self.xlims = (80, 10000)
         self.setupBaseFigure()
 
         ## MENU BAR
         self.menubar = self.menuBar()
-        exitAction = QAction(QIcon(':/exit'), self.tr('Exit'), self)
+        exitAction = QAction(QIcon(':/right-from-bracket-solid'), self.tr('Exit'), self)
         exitAction.setShortcut('Ctrl+Q')
         exitAction.setStatusTip(self.tr('Exit application'))
         exitAction.triggered.connect(self.close)
         self.statusBar()
         loadCaseAction = QAction(QIcon(':/folder-open-regular'), self.tr('Load case'), self)
         loadCaseAction.setShortcut('Ctrl+L')
         loadCaseAction.setStatusTip(self.tr('Load case file'))
         loadCaseAction.triggered.connect(self.loadCaseDialog)
         loadRandomCaseAction = QAction(QIcon(':/dice-solid'), self.tr('Load random case'), self) #QIcon(':/dice-solid'), self.tr('Exit'), self.tr('Load random case'), self)
         #loadCaseAction.setShortcut('Ctrl+L')
         loadRandomCaseAction.setStatusTip(self.tr('Load random case file'))
         loadRandomCaseAction.triggered.connect(self.loadRandomCase)
-        generateCaseAction = QAction(self.tr('Generate case'), self)
+        generateCaseAction = QAction(QIcon(':/gears-solid'), self.tr('Generate case'), self)
         generateCaseAction.triggered.connect(self.onClickGenerateCase)
         #FILE MENU
         self.fileMenu = self.menubar.addMenu(self.tr('&File'))
         self.fileMenu.addAction(loadCaseAction)
         self.fileMenu.addAction(loadRandomCaseAction)
         self.fileMenu.addAction(generateCaseAction)
         self.fileMenu.addAction(exitAction)
 
         #EDIT MENU
         self.editMenu = self.menubar.addMenu(self.tr('&Edit'))
-        self.editPrefAction = QAction(self.tr('Preferences'), self)
+        self.editPrefAction = QAction(QIcon(':/sliders-solid'), self.tr('Preferences'), self)
         self.editMenu.addAction(self.editPrefAction)
         self.editPrefAction.triggered.connect(self.onEditPref)
         #HELP MENU
         self.helpMenu = self.menubar.addMenu(self.tr('&Help'))
 
-        self.onShowManualHtmlAction = QAction(self.tr('Manual (html)'), self)
+        self.onShowManualHtmlAction = QAction(QIcon(":/book-bookmark-solid"), self.tr('Manual (html)'), self)
         self.helpMenu.addAction(self.onShowManualHtmlAction)
         self.onShowManualHtmlAction.triggered.connect(self.onShowManualHtml)
 
-        self.onShowManualPdfAction = QAction(self.tr('Manual (pdf)'), self)
+        self.onShowManualPdfAction = QAction(QIcon(":/book-solid"), self.tr('Manual (pdf)'), self)
         self.helpMenu.addAction(self.onShowManualPdfAction)
         self.onShowManualPdfAction.triggered.connect(self.onShowManualPdf)
 
-        self.onAboutAction = QAction(QIcon.fromTheme("help-about", QIcon(":/help-about")), self.tr('About audiometry_trainer'), self)
+        self.onShowVideoTutorialsAction = QAction(QIcon(":/film-solid"), self.tr('Online video tutorials'), self)
+        self.helpMenu.addAction(self.onShowVideoTutorialsAction)
+        self.onShowVideoTutorialsAction.triggered.connect(self.onShowVideoTutorials)
+
+        self.onAboutAction = QAction(QIcon(":/circle-info-solid"), self.tr('About audiometry_trainer'), self)
         self.helpMenu.addAction(self.onAboutAction)
         self.onAboutAction.triggered.connect(self.onAbout)
 
         #WHATSTHIS
-        self.onWhatsThisAction = QAction(QIcon.fromTheme("help-contextual", QIcon(":/help-contextual")), self.tr('?'), self)
+        self.onWhatsThisAction = QAction(self.tr("?"), self)
         self.menubar.addAction(self.onWhatsThisAction)
         self.onWhatsThisAction.triggered.connect(self.onWhatsThis)
 
         ## control grid left side
         n = 0
         self.ch1Label = QLabel(self.tr('Chan. 1:'), self)
         self.transducerChooserCh1 = QComboBox()
@@ -263,27 +267,14 @@
         self.TESFCouplingChooser.textActivated[str].connect(self.onTESFCouplingChooserChange)
         self.TESFCouplingChooser.setWhatsThis(self.tr("Select coupling option for the test ear."))
         self.TESFCouplingChooser.setToolTip(self.tr("Select coupling option for the test ear."))
         self.grid_L.addWidget(self.TESFCouplingLabel, n, 0)
         self.grid_L.addWidget(self.TESFCouplingChooser, n, 1)
         self.TESFCouplingLabel.hide()
         self.TESFCouplingChooser.hide()
-        n = n+1
-        self.lockChansCheckBox = QCheckBox(self.tr('Lock channels'))
-        self.lockChansCheckBox.stateChanged[int].connect(self.toggleLockChans)
-        self.lockChansCheckBox.setIcon(QtGui.QIcon(":/lock-open-solid"))
-        self.lockChansCheckBox.setWhatsThis(self.tr("Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount."))
-        self.lockChansCheckBox.setToolTip(self.tr("Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount."))
-        self.grid_L.addWidget(self.lockChansCheckBox, n, 0, 1, 1)
-
-        self.autoSearchButton = QPushButton(self.tr("Auto. thresh. search"), self)
-        self.autoSearchButton.clicked.connect(self.onClickAutoButton)
-        self.autoSearchButton.setWhatsThis(self.tr("Perform an automatic threshold search using the Hughson-Westlake procedure."))
-        self.autoSearchButton.setToolTip(self.tr("Perform an automatic threshold search using the Hughson-Westlake procedure."))
-        self.grid_L.addWidget(self.autoSearchButton, n, 1)
         
         n = n+1
         self.showRespEarCheckBox = QCheckBox(self.tr('Show response ear'))
         self.showRespEarCheckBox.stateChanged[int].connect(self.toggleShowRespEar)
         self.grid_L.addWidget(self.showRespEarCheckBox, n, 0, 1, 2)
         self.showRespEarCheckBox.setWhatsThis(self.tr("Response light will turn red/blue if the right/left ear is responding. White if both ears respond."))
         self.showRespEarCheckBox.setToolTip(self.tr("Response light will turn red/blue if the right/left ear is responding. White if both ears respond."))
@@ -291,14 +282,21 @@
         self.showRespCountsCheckBox = QCheckBox(self.tr('Show response counts'))
         self.showRespCountsCheckBox.setChecked(self.showRespCounts)
         self.showRespCountsCheckBox.stateChanged[int].connect(self.toggleShowRespCounts)
         self.showRespCountsCheckBox.setWhatsThis(self.tr("Show the counts of responses on ascending level trials."))
         self.showRespCountsCheckBox.setToolTip(self.tr("Show the counts of responses on ascending level trials."))
         self.grid_L.addWidget(self.showRespCountsCheckBox, n, 0, 1, 2)
         n = n+1
+
+        self.autoSearchButton = QPushButton(QIcon(':/robot-solid'), self.tr("Auto. thresh. search"), self)
+        self.autoSearchButton.clicked.connect(self.onClickAutoButton)
+        self.autoSearchButton.setWhatsThis(self.tr("Perform an automatic threshold search using the Hughson-Westlake procedure."))
+        self.autoSearchButton.setToolTip(self.tr("Perform an automatic threshold search using the Hughson-Westlake procedure."))
+        self.grid_L.addWidget(self.autoSearchButton, n, 0, 1, 2)
+        n = n+1
         self.respLightLabel = QLabel(self.tr("Response light"))
         self.respLightLabel.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         self.respLightLabel.setStyleSheet("font-weight: bold")
         self.grid_L.addWidget(self.respLightLabel, n, 0, 1, 2)
         n = n+1
         self.respLight = indicatorLight(self)
         self.respLight.setWhatsThis(self.tr("The light will turn on if the virtual listener responds to the stimulus."))
@@ -495,19 +493,26 @@
         self.ch2DownButton.setWhatsThis(self.tr("Decrease the level of the masking noise."))
         self.ch2DownButton.setToolTip(self.tr("Decrease the level of the masking noise."))
         self.grid_R.addWidget(self.ch2DownButton, n, 2)
         self.ch2DownButton.clicked.connect(self.onClickCh2DownButton)
         
         n = n+1
         self.ch2OnCheckBox = QCheckBox(self.tr('Chan. 2 ON'))
-        #self.gridOn.setChecked(self.prm['pref']['grid'])
+        self.ch2OnCheckBox.setIcon(QtGui.QIcon(":/mask-solid-off"))
         self.ch2OnCheckBox.setWhatsThis(self.tr("Turn ON the masking noise in channel 2."))
         self.ch2OnCheckBox.setToolTip(self.tr("Turn ON the masking noise in channel 2."))
         self.ch2OnCheckBox.stateChanged[int].connect(self.toggleCh2)
         self.grid_R.addWidget(self.ch2OnCheckBox, n, 0)
+        n = n+1
+        self.lockChansCheckBox = QCheckBox(self.tr('Lock channels'))
+        self.lockChansCheckBox.stateChanged[int].connect(self.toggleLockChans)
+        self.lockChansCheckBox.setIcon(QtGui.QIcon(":/lock-open-solid"))
+        self.lockChansCheckBox.setWhatsThis(self.tr("Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount."))
+        self.lockChansCheckBox.setToolTip(self.tr("Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount."))
+        self.grid_R.addWidget(self.lockChansCheckBox, n, 0)
 
         n = n+1
         self.showCaseFileNameCheckBox = QCheckBox(self.tr('Show case filename'))
         self.showCaseFileNameCheckBox.setChecked(False)
         self.showCaseFileNameCheckBox.stateChanged[int].connect(self.toggleShowCaseFileName)
         self.showCaseFileNameCheckBox.setWhatsThis(self.tr("Show the filename of the case currently loaded."))
         self.showCaseFileNameCheckBox.setToolTip(self.tr("Show the filename of the case currently loaded."))
@@ -944,17 +949,20 @@
         self.canvas.draw()
 
     def toggleCh2(self, state):
         if self.ch2OnCheckBox.isChecked():
             self.ch2On = True
             self.ch2Tracker, = self.axes.plot(self.testFreq, self.ch2Lev, marker=self.ch2Marker, color=self.currCh2Color, markersize=self.trackerMarkerSize)
             self.NTEStatusChooser.setCurrentIndex(self.NTEStatusChooser.findText(self.tr("Earphone on")))
+            self.ch2OnCheckBox.setIcon(QtGui.QIcon(":/mask-solid"))
         else:
             self.ch2On = False
             self.ch2Tracker.remove()
+            self.NTEStatusChooser.setCurrentIndex(self.NTEStatusChooser.findText(self.tr("Uncovered")))
+            self.ch2OnCheckBox.setIcon(QtGui.QIcon(":/mask-solid-off"))
         self.canvas.draw()
         self.mw.setFocus()
 
     def toggleLockChans(self, state):
         if self.lockChansCheckBox.isChecked():
             self.chansLocked = True
             self.lockChansCheckBox.setText(self.tr("Unlock channels"))
@@ -2093,14 +2101,23 @@
         localized_html_path = os.path.abspath(self.prm['rootDirectory']) + '/doc/_build/html_'+self.prm['locale_string'][0:2]+'/index.html'
         if os.path.isfile(localized_html_path):
             fileToOpen = localized_html_path
         else:
             fileToOpen = os.path.abspath(self.prm['rootDirectory']) + '/doc/_build/html/index.html'
         QDesktopServices.openUrl(QtCore.QUrl.fromLocalFile(fileToOpen))
 
+    def onShowVideoTutorials(self):
+        url_en = QUrl("https://www.youtube.com/playlist?list=PLyfCl_MBfnRBWhN_N3IOJ7wGvIZuRXLK4")
+        url_fr = QUrl("https://www.youtube.com/playlist?list=PLyfCl_MBfnRBh7CLE48BeawkZpKODle1X")
+        if self.prm['locale_string'][0:2] == 'fr':
+            url = url_fr
+        else:
+            url = url_en
+        QDesktopServices.openUrl(url)
+
     def onAbout(self):
         if pyqtversion in [5,6]:
             qt_compiled_ver = QtCore.QT_VERSION_STR
             qt_runtime_ver = QtCore.qVersion()
             qt_pybackend_ver = QtCore.PYQT_VERSION_STR
             qt_pybackend = "PyQt"
         QMessageBox.about(self, self.tr("About audiometry_trainer"),
@@ -2117,14 +2134,16 @@
                 This program is distributed in the hope that it will be useful,
                 but WITHOUT ANY WARRANTY; without even the implied warranty of
                 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
                 GNU General Public License for more details.
                 <p>
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see <a href="http://www.gnu.org/licenses/">http://www.gnu.org/licenses/</a>
+
+                <p> A number of icons are from Font Awesome, released under the <a href="https://creativecommons.org/licenses/by/4.0/">CC BY 4.0 license</a>. See <a href="https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads">CREDITS.txt</a> in the source distribution for details.
                 <p>Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}""").format(__version__, self.prm['builddate'], platform.python_version(), qt_pybackend, qt_pybackend_ver, qt_compiled_ver, qt_runtime_ver, platform.system()))
 
 
 class indicatorLight(QFrame):
     def __init__(self, parent):
         QFrame.__init__(self, parent)
         self.setSizePolicy(QSizePolicy(QSizePolicy.Policy.Expanding, QSizePolicy.Policy.Preferred))
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/pysdt.py` & `audiometry_trainer-0.1.6/audiometry_trainer/pysdt.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/utility_functions.py` & `audiometry_trainer-0.1.6/audiometry_trainer/utility_functions.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer/window_generate_case.py` & `audiometry_trainer-0.1.6/audiometry_trainer/window_generate_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 #    You should have received a copy of the GNU General Public License
 #    along with audiometry_trainer.  If not, see <http://www.gnu.org/licenses/>.
 
 from .pyqtver import*
 if pyqtversion == 5:
     from PyQt5 import QtGui, QtCore, QtWidgets
     from PyQt5.QtCore import pyqtSignal, QItemSelectionModel, QLocale, Qt, QThread
-    from PyQt5.QtGui import QColor, QDoubleValidator, QIntValidator
+    from PyQt5.QtGui import QColor, QDoubleValidator, QIcon, QIntValidator
     from PyQt5.QtWidgets import QAction, QApplication, QCheckBox, QColorDialog, QComboBox, QDesktopWidget, QDialog, QDialogButtonBox, QFileDialog, QFrame, QGridLayout, QHBoxLayout, QLabel, QLineEdit, QMainWindow, QMenu, QMessageBox, QProgressBar, QProgressDialog, QPushButton, QSizePolicy, QSplitter, QTableView, QTableWidget, QTableWidgetItem, QTextEdit, QVBoxLayout, QWidget
 elif pyqtversion == 6:
     from PyQt6 import QtGui, QtCore, QtWidgets
     from PyQt6.QtCore import pyqtSignal, QItemSelectionModel, QLocale, Qt, QThread
-    from PyQt6.QtGui import QAction, QColor, QDoubleValidator, QIntValidator
+    from PyQt6.QtGui import QAction, QColor, QDoubleValidator, QIcon, QIntValidator
     from PyQt6.QtWidgets import QApplication, QCheckBox, QColorDialog, QComboBox, QDialog, QDialogButtonBox, QFileDialog, QFrame, QGridLayout, QHBoxLayout, QLabel, QLineEdit, QMainWindow, QMenu, QMessageBox, QProgressBar, QProgressDialog, QPushButton, QSizePolicy, QSplitter, QTableView, QTableWidget, QTableWidgetItem, QTextEdit, QVBoxLayout, QWidget
 
 import fnmatch, os, scipy
 import numpy as np
 import pandas as pd
 #from .utility_audiogram import*
 from .hughson_westlake import*
@@ -52,19 +52,19 @@
         self.freqs = np.array([125, 250, 500, 750, 1000, 1500, 2000, 3000, 4000, 6000, 8000])
         self.nFreqs = len(self.freqs)
         self.seed = None
 
         self.menubar = self.menuBar()
 
         self.fileMenu = self.menubar.addMenu(self.tr('&File'))
-        loadPrmAction = QAction(self.tr('Load parameters'), self)
+        loadPrmAction = QAction(QIcon(':/folder-open-regular'), self.tr('Load parameters'), self)
         loadPrmAction.setStatusTip(self.tr('Load audiogram parameters'))
         loadPrmAction.triggered.connect(self.onLoadPrmFile)
         self.fileMenu.addAction(loadPrmAction)
-        savePrmAction = QAction(self.tr('Save parameters'), self)
+        savePrmAction = QAction(QIcon(':/floppy-disk-solid'), self.tr('Save parameters'), self)
         savePrmAction.setStatusTip(self.tr('Save audiogram parameters'))
         savePrmAction.triggered.connect(self.onSavePrmFile)
         self.fileMenu.addAction(savePrmAction)
         
         self.editMenu = self.menubar.addMenu(self.tr('&Edit'))
         editFreqsAction = QAction(self.tr('Frequencies'), self)
         editFreqsAction.setStatusTip(self.tr('Add/remove audiogram frequencies'))
@@ -85,15 +85,15 @@
 
         self.vBox_L = QVBoxLayout()
         self.grid_R = QGridLayout()
         self.grid_R.setAlignment(Qt.AlignmentFlag.AlignTop)
         self.vBox_L.addWidget(self.valsTableWidget)
 
         n = 0
-        self.runSimulationButton = QPushButton(self.tr("Run simulation"), self)
+        self.runSimulationButton = QPushButton(QIcon(':/person-running-solid'), self.tr("Run simulation"), self)
         self.grid_R.addWidget(self.runSimulationButton, n, 0, 1, 2)
         self.runSimulationButton.clicked.connect(self.onClickRunSimulationButton)
         n = n+1
         self.nSimLabel = QLabel(self.tr("No. simulations"))
         self.nSimTF = QLineEdit("1000")
         self.nSimTF.setValidator(QIntValidator(self))
         self.nSim = self.currLocale.toInt(self.nSimTF.text())[0]
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer.egg-info/PKG-INFO` & `audiometry_trainer-0.1.6/audiometry_trainer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiometry_trainer
-Version: 0.1.5
+Version: 0.1.6
 Summary: Clinical audiometry simulator
 Author-email: Samuele Carcagno <sam.carcagno@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `audiometry_trainer-0.1.5/audiometry_trainer.egg-info/SOURCES.txt` & `audiometry_trainer-0.1.6/audiometry_trainer.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 .gitignore
 .readthedocs.yaml
 COPYING.txt
+CREDITS.txt
 MANIFEST.in
 README.md
 pyproject.toml
 resources.qrc
 setup_cx.py
 audiometry_trainer/__init__.py
 audiometry_trainer/__main__.py
@@ -33,14 +34,20 @@
 audiometry_trainer/case_files/danesh_et_al_2018_info_fr.md
 audiometry_trainer/case_files/hamad_et_al_2002_case_3.csv
 audiometry_trainer/case_files/hamad_et_al_2002_case_3_info.md
 audiometry_trainer/case_files/hamad_et_al_2002_case_3_info_fr.md
 audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C.csv
 audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info.md
 audiometry_trainer/case_files/kramer_and_brown_2019_fig_9-3C_info_fr.md
+audiometry_trainer/case_files/lee_et_al_2021_case_1.csv
+audiometry_trainer/case_files/lee_et_al_2021_case_1_info.md
+audiometry_trainer/case_files/lee_et_al_2021_case_1_info_fr.md
+audiometry_trainer/case_files/manzari_2010.csv
+audiometry_trainer/case_files/manzari_2010_info.md
+audiometry_trainer/case_files/manzari_2010_info_fr.md
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A.csv
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info.md
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_A_info_fr.md
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B.csv
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info.md
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_B_info_fr.md
 audiometry_trainer/case_files/morse-fortier_et_al_2024_case_C.csv
@@ -97,14 +104,16 @@
 audiometry_trainer/case_files/yacullo_2015_fig_6-6.csv
 audiometry_trainer/case_files/yacullo_2015_fig_6-6_info.md
 audiometry_trainer/case_files/yacullo_2015_fig_6-6_info_fr.md
 audiometry_trainer/doc/Makefile
 audiometry_trainer/doc/audiometry_trainer.fr.png
 audiometry_trainer/doc/audiometry_trainer.png
 audiometry_trainer/doc/conf.py
+audiometry_trainer/doc/file_menu.fr.png
+audiometry_trainer/doc/file_menu.png
 audiometry_trainer/doc/generate_case.rst
 audiometry_trainer/doc/index.rst
 audiometry_trainer/doc/installation.rst
 audiometry_trainer/doc/internals.rst
 audiometry_trainer/doc/intro.rst
 audiometry_trainer/doc/logistic_psy.fr.png
 audiometry_trainer/doc/logistic_psy.png
@@ -128,14 +137,15 @@
 audiometry_trainer/doc/_build/html/references.html
 audiometry_trainer/doc/_build/html/search.html
 audiometry_trainer/doc/_build/html/searchindex.js
 audiometry_trainer/doc/_build/html/threshold_search.html
 audiometry_trainer/doc/_build/html/user_interface.html
 audiometry_trainer/doc/_build/html/virtual_listener.html
 audiometry_trainer/doc/_build/html/_images/audiometry_trainer.png
+audiometry_trainer/doc/_build/html/_images/file_menu.png
 audiometry_trainer/doc/_build/html/_images/logistic_psy.png
 audiometry_trainer/doc/_build/html/_sources/generate_case.rst.txt
 audiometry_trainer/doc/_build/html/_sources/index.rst.txt
 audiometry_trainer/doc/_build/html/_sources/installation.rst.txt
 audiometry_trainer/doc/_build/html/_sources/internals.rst.txt
 audiometry_trainer/doc/_build/html/_sources/intro.rst.txt
 audiometry_trainer/doc/_build/html/_sources/masking.rst.txt
@@ -187,14 +197,16 @@
 audiometry_trainer/doc/_build/html_fr/search.html
 audiometry_trainer/doc/_build/html_fr/searchindex.js
 audiometry_trainer/doc/_build/html_fr/threshold_search.html
 audiometry_trainer/doc/_build/html_fr/user_interface.html
 audiometry_trainer/doc/_build/html_fr/virtual_listener.html
 audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.fr.png
 audiometry_trainer/doc/_build/html_fr/_images/audiometry_trainer.png
+audiometry_trainer/doc/_build/html_fr/_images/file_menu.fr.png
+audiometry_trainer/doc/_build/html_fr/_images/file_menu.png
 audiometry_trainer/doc/_build/html_fr/_images/logistic_psy.fr.png
 audiometry_trainer/doc/_build/html_fr/_sources/generate_case.rst.txt
 audiometry_trainer/doc/_build/html_fr/_sources/index.rst.txt
 audiometry_trainer/doc/_build/html_fr/_sources/installation.rst.txt
 audiometry_trainer/doc/_build/html_fr/_sources/internals.rst.txt
 audiometry_trainer/doc/_build/html_fr/_sources/intro.rst.txt
 audiometry_trainer/doc/_build/html_fr/_sources/masking.rst.txt
@@ -254,31 +266,58 @@
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/references.po
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.mo
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/threshold_search.po
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.mo
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/user_interface.po
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.mo
 audiometry_trainer/doc/locale/fr/LC_MESSAGES/virtual_listener.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/generate_case.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/generate_case.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/index.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/index.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/installation.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/installation.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/internals.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/internals.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/intro.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/intro.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/masking.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/masking.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/references.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/references.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/threshold_search.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/threshold_search.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/user_interface.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/user_interface.po
+audiometry_trainer/doc/locale/it/LC_MESSAGES/virtual_listener.mo
+audiometry_trainer/doc/locale/it/LC_MESSAGES/virtual_listener.po
 icons/arrow-down-solid.svg
 icons/arrow-up-solid.svg
 icons/audiometry_trainer_icon.ico
 icons/audiometry_trainer_icon.svg
+icons/book-bookmark-solid.svg
+icons/book-solid.svg
+icons/circle-info-solid.svg
 icons/dice-solid.svg
-icons/exit.svg
+icons/film-solid.svg
+icons/floppy-disk-solid.svg
 icons/folder-open-regular.svg
+icons/gears-solid.svg
 icons/headphones-solid.svg
-icons/help-about.svgz
-icons/help-contents.svgz
-icons/help-contextual.svgz
 icons/insert.svg
 icons/lock-open-solid.svg
 icons/lock-solid.svg
+icons/mask-solid-off.svg
 icons/mask-solid.svg
-icons/preferences-other.svgz
+icons/person-running-solid.svg
+icons/question-solid.svg
+icons/right-from-bracket-solid.svg
+icons/robot-solid.svg
 icons/skull-solid.svg
+icons/sliders-solid.svg
 prep-release/audiometry_trainer.pro
 prep-release/audiometry_trainer_el.ts
 prep-release/audiometry_trainer_en_GB.ts
 prep-release/audiometry_trainer_en_US.ts
 prep-release/audiometry_trainer_es.ts
 prep-release/audiometry_trainer_fr.ts
 prep-release/audiometry_trainer_it.ts
```

### Comparing `audiometry_trainer-0.1.5/icons/dice-solid.svg` & `audiometry_trainer-0.1.6/icons/dice-solid.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/icons/folder-open-regular.svg` & `audiometry_trainer-0.1.6/icons/folder-open-regular.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/icons/headphones-solid.svg` & `audiometry_trainer-0.1.6/icons/headphones-solid.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/icons/insert.svg` & `audiometry_trainer-0.1.6/icons/insert.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/icons/mask-solid.svg` & `audiometry_trainer-0.1.6/icons/mask-solid.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/icons/skull-solid.svg` & `audiometry_trainer-0.1.6/icons/skull-solid.svg`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer.pro` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer.pro`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_el.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_el.ts`

 * *Files 2% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_el.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_el.ts`

```diff
@@ -171,80 +171,80 @@
       <source>Lapse rate L</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
       <source>Lock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
       <source>Show response ear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation type="unfinished"/>
@@ -261,580 +261,587 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="196"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
-      <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
-                                - version: {0}; &lt;br&gt;
-                                - build date: {1} &lt;br&gt;
-                                &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
-                                All rights reserved. &lt;p&gt;
-                This program is free software: you can redistribute it and/or modify
-                it under the terms of the GNU General Public License as published by
-                the Free Software Foundation, either version 3 of the License, or
-                (at your option) any later version.
-                &lt;p&gt;
-                This program is distributed in the hope that it will be useful,
-                but WITHOUT ANY WARRANTY; without even the implied warranty of
-                MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-                GNU General Public License for more details.
-                &lt;p&gt;
-                You should have received a copy of the GNU General Public License
-                along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
-                &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
       <location filename="../audiometry_trainer/main_window.py" line="201"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="178"/>
       <source>Load case</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="180"/>
       <source>Load case file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="197"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="101"/>
       <source>Frequency (kHz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="182"/>
       <source>Load random case</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="184"/>
       <source>Load random case file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="186"/>
       <source>Generate case</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
       <source>Auto. thresh. search</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
       <source>Show response counts</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="203"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
       <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
       <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
       <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
       <source>Show the counts of responses on ascending level trials.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
+      <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
+                                - version: {0}; &lt;br&gt;
+                                - build date: {1} &lt;br&gt;
+                                &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
+                                All rights reserved. &lt;p&gt;
+                This program is free software: you can redistribute it and/or modify
+                it under the terms of the GNU General Public License as published by
+                the Free Software Foundation, either version 3 of the License, or
+                (at your option) any later version.
+                &lt;p&gt;
+                This program is distributed in the hope that it will be useful,
+                but WITHOUT ANY WARRANTY; without even the implied warranty of
+                MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                GNU General Public License for more details.
+                &lt;p&gt;
+                You should have received a copy of the GNU General Public License
+                along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
+                &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
       <location filename="../audiometry_trainer/dialog_edit_preferences.py" line="478"/>
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_GB.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_GB.ts`

 * *Files 2% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_GB.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_GB.ts`

```diff
@@ -181,20 +181,20 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation type="unfinished"/>
@@ -256,565 +256,570 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
-      <source>Lock channels</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
-      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
-      <source>Auto. thresh. search</source>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
+      <source>Show response ear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
-      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
+      <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
-      <source>Show response ear</source>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
+      <source>Show response counts</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
-      <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
+      <source>Show the counts of responses on ascending level trials.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
-      <source>Show response counts</source>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
+      <source>Auto. thresh. search</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
-      <source>Show the counts of responses on ascending level trials.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
+      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
+      <source>Lock channels</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
+      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -824,14 +829,16 @@
                 This program is distributed in the hope that it will be useful,
                 but WITHOUT ANY WARRANTY; without even the implied warranty of
                 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
                 GNU General Public License for more details.
                 &lt;p&gt;
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
                 &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_US.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_US.ts`

 * *Files 2% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_en_US.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_en_US.ts`

```diff
@@ -171,80 +171,80 @@
       <source>Lapse rate L</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
       <source>Lock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
       <source>Show response ear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation type="unfinished"/>
@@ -261,580 +261,587 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="196"/>
       <source>&amp;Edit</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
-      <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
-                                - version: {0}; &lt;br&gt;
-                                - build date: {1} &lt;br&gt;
-                                &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
-                                All rights reserved. &lt;p&gt;
-                This program is free software: you can redistribute it and/or modify
-                it under the terms of the GNU General Public License as published by
-                the Free Software Foundation, either version 3 of the License, or
-                (at your option) any later version.
-                &lt;p&gt;
-                This program is distributed in the hope that it will be useful,
-                but WITHOUT ANY WARRANTY; without even the implied warranty of
-                MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-                GNU General Public License for more details.
-                &lt;p&gt;
-                You should have received a copy of the GNU General Public License
-                along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
-                &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
       <location filename="../audiometry_trainer/main_window.py" line="201"/>
       <source>&amp;Help</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="178"/>
       <source>Load case</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="180"/>
       <source>Load case file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="197"/>
       <source>Preferences</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="101"/>
       <source>Frequency (kHz)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="182"/>
       <source>Load random case</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="184"/>
       <source>Load random case file</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="186"/>
       <source>Generate case</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
       <source>Auto. thresh. search</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
       <source>Show response counts</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="203"/>
       <source>Manual (html)</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
       <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
       <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
       <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
       <source>Show the counts of responses on ascending level trials.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
       <translation type="unfinished"/>
     </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
+      <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
+                                - version: {0}; &lt;br&gt;
+                                - build date: {1} &lt;br&gt;
+                                &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
+                                All rights reserved. &lt;p&gt;
+                This program is free software: you can redistribute it and/or modify
+                it under the terms of the GNU General Public License as published by
+                the Free Software Foundation, either version 3 of the License, or
+                (at your option) any later version.
+                &lt;p&gt;
+                This program is distributed in the hope that it will be useful,
+                but WITHOUT ANY WARRANTY; without even the implied warranty of
+                MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+                GNU General Public License for more details.
+                &lt;p&gt;
+                You should have received a copy of the GNU General Public License
+                along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
+                &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation type="unfinished"/>
+    </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
       <location filename="../audiometry_trainer/dialog_edit_preferences.py" line="478"/>
       <source>There are unsaved changes. Apply Changes?</source>
       <translation type="unfinished"/>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_es.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_es.ts`

 * *Files 2% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_es.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_es.ts`

```diff
@@ -181,20 +181,20 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation type="unfinished"/>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation type="unfinished"/>
@@ -256,565 +256,570 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
-      <source>Lock channels</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
-      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
-      <source>Auto. thresh. search</source>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
+      <source>Show response ear</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
-      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
+      <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
-      <source>Show response ear</source>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
+      <source>Show response counts</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
-      <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
+      <source>Show the counts of responses on ascending level trials.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
-      <source>Show response counts</source>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
+      <source>Auto. thresh. search</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
-      <source>Show the counts of responses on ascending level trials.</source>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
+      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
+      <source>Lock channels</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
+      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -824,14 +829,16 @@
                 This program is distributed in the hope that it will be useful,
                 but WITHOUT ANY WARRANTY; without even the implied warranty of
                 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
                 GNU General Public License for more details.
                 &lt;p&gt;
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
                 &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_fr.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_fr.ts`

 * *Files 0% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_fr.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_fr.ts`

```diff
@@ -181,20 +181,20 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation>Niveau (dB HL)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
       <translation>Supra-aural</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation>Droite</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation>Quitter</translation>
@@ -233,15 +233,15 @@
       <location filename="../audiometry_trainer/main_window.py" line="189"/>
       <source>&amp;File</source>
       <translation>&amp;Fichier</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="196"/>
       <source>&amp;Edit</source>
-      <translation>&amp;Éditer</translation>
+      <translation>É&amp;dition</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="197"/>
       <source>Preferences</source>
       <translation>Préférences</translation>
     </message>
     <message>
@@ -256,565 +256,570 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation>Mode d'emploi (pdf)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation>Tutoriels vidéo en ligne</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation>À propos d' audiometry_trainer</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation>?</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation>Can. 1 :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
       <translation>Insert</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation>Conduction Osseuse</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
       <translation>Champ libre</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
       <translation>Sélectionnez le transducteur pour l'oreille testée.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation>Oreille test :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation>Gauche</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
       <translation>Sélectionnez l'oreille testée (droite ou gauche).</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation>État de l'oreille test :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation>Sans appareil</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation>Avec appareil</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
       <translation>Réglez le status de l'oreille testée (avec ou sans appareil).</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation>Couplage de l'oreille test :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation>Dôme (ouverte)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation>Dôme (tulipe)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation>Dôme (évent simple)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation>Dôme (évent double)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation>Double dôme (power)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation>Embout</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation>Sélectionnez l'option de couplage pour l'oreille testée.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
-      <source>Lock channels</source>
-      <translation>Verrouiller les canaux</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
-      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
-      <translation>Verrouillez les canaux afin que des changements de niveau du stimulus produisent des changements de niveau du bruit masquant de la même taille.</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
-      <source>Auto. thresh. search</source>
-      <translation>Rech. seuil auto</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
-      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
-      <translation>Exécutez une recherche du seuil automatique en utilisant la procédure Hughson-Westlake.</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
       <source>Show response ear</source>
       <translation>Afficher l'oreille qui répond</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
       <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation>Le témoin de réponse s'allumera en rouge/bleu si l'oreille droite/gauche répond. Blanc si les deux oreilles répondent.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
       <source>Show response counts</source>
       <translation>Afficher le compte des réponses</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
       <source>Show the counts of responses on ascending level trials.</source>
       <translation>Affichez le compte des réponses obtenues sur des essais de niveau ascendant.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
+      <source>Auto. thresh. search</source>
+      <translation>Rech. seuil auto</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
+      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
+      <translation>Exécutez une recherche du seuil automatique en utilisant la procédure Hughson-Westlake.</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
       <translation>Témoin de réponse</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
       <translation>Le témoin s'allumera si le sujet virtuel répond au stimulus.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation>Marquer le seuil</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
       <translation>Marquez le seuil au niveau courant.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation>Pas de réponse</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
       <translation>Marquez sur l'audiogramme qu'il n'y avait pas de réponse au niveau maximal du stimulus.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation>Dilemme de masquage</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
       <translation>Marquez sur l'audiogramme que le seuil courant n'a pas pu être établi à cause d'un dilemme de masquage.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation>Affichage des seuils estimés :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation>Seuil non masqué aér. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation>Affichez les seuils non masqués en conduction aérienne que vous avez mesuré pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation>Seuil non masqué aér. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation>Affichez les seuils non masqués en conduction aérienne que vous avez mesuré pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation>Seuil non masqué oss. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation>Affichez les seuils non masqués en conduction osseuse que vous avez mesuré pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation>Seuil non masqué oss. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation>Affichez les seuils non masqués en conduction osseuse que vous avez mesuré pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation>Seuil masqué aér. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation>Affichez les seuils masqués en conduction aérienne que vous avez mesuré pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation>Seuil masqué aér. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation>Affichez les seuils masqués en conduction aérienne que vous avez mesuré pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation>Seuil masqué oss. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation>Affichez les seuils masqués en conduction osseuse que vous avez mesuré pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation>Seuil masqué oss. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation>Affichez les seuils masqués en conduction osseuse que vous avez mesuré pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
       <translation>Affichage des vrais seuils :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
       <translation>Seuil aér. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
       <translation>Affichez les seuils attendus en conduction aérienne pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation>IC</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
       <translation>Affichez les intervalles de confiance de 95% des seuils attendus en conduction aérienne pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
       <translation>Seuil aér. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
       <translation>Affichez les seuils attendus en conduction aérienne pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
       <translation>Affichez les intervalles de confiance de 95% des seuils attendus en conduction aérienne pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
       <translation>Seuil oss. D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
       <translation>Affichez les seuils attendus en conduction osseuse pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
       <translation>Affichez les intervalles de confiance de 95% des seuils attendus en conduction osseuse pour l'oreille droite.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
       <translation>Seuil oss. G</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
       <translation>Affichez les seuils attendus en conduction osseuse pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
       <translation>Affichez les intervalles de confiance de 95% des seuils attendus en conduction osseuse pour l'oreille gauche.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
       <translation>État de l'oreille non testée :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
       <translation>Nue</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
       <translation>Écouter sur l'oreille</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
       <translation>Indiquez si le sujet virtuel a un écouter sur l'oreille non testée ou pas. Une comparaison de ces deux conditions (sans envoye de bruit masquant) peut être utilisée pour estimer l'effet d'occlusion.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation>Can. 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
       <translation>Bouchon</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
       <translation>Sélectionne le status de l'oreille non testée.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation>Can. 2 :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
       <translation>Sélectionnez le transducteur employé pour envoyer le bruit masquant à travers le canal 2.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation>Niveau du can. 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation>Saisissez le niveau, en dB de masquage efficace (EM), du bruit masquant.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
       <translation>Augmentez le niveau du bruit masquant.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation>-</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
       <translation>Baissez le niveau du bruit masquant.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation>Can. 2 ON</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
       <translation>Déclenchez l'envoi de bruit masquant dans le canal 2.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
+      <source>Lock channels</source>
+      <translation>Verrouiller les canaux</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
+      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
+      <translation>Verrouillez les canaux afin que des changements de niveau du stimulus produisent des changements de niveau du bruit masquant de la même taille.</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation>Afficher le nom du fichier</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
       <translation>Affichez le nom du fichier pour le cas actuellement chargé.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation>Afficher l'info du cas</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
       <translation>Affichez l'information disponible pour le cas actuellement chargée.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation>Fichier du cas :</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation>Grille</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
       <translation>Affichez une grille sur l'audiogramme.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
       <translation>Ce témoin s'allumera lorsque un stimulus est reproduit sur le canal 1.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
       <translation>Témoin de stimulation</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
       <translation>Reproduisez le stimulus sur le canal 1.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation>Pas d'info disponible sur le cas</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation>Choisir le fichier de cas à charger</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation>Fichiérs CSV (*.csv *CSV *Csv);;All Files (*)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation>Déverouiller les canaux</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation>Avertissement</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
       <translation>Le niveau du canal 2 demandé hors limites pour le transducter actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
       <translation>Le canal 2 a atteint son niveau maximal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
       <translation>Le canal 2 a atteint son niveau minimal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
       <translation>Le canal 1 a atteint son niveau minimal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
       <translation>Le canal 2 est verrouillé au canal 1 et a atteint son niveau minimal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
       <translation>Le canal 1 a atteint son niveau maximal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
       <translation>Le canal 2 est verrouillé au canal 1 et a atteint son niveau maximal pour le transducteur actuel</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
       <translation>La recherche automatique n'est pas disponible quand le canal 2 est actif</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
       <translation>Circum-aural</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -824,34 +829,36 @@
                 This program is distributed in the hope that it will be useful,
                 but WITHOUT ANY WARRANTY; without even the implied warranty of
                 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
                 GNU General Public License for more details.
                 &lt;p&gt;
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
                 &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2107"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2124"/>
       <source>Earphones on</source>
       <translation type="obsolete">Ècouter sur l'oreille</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2107"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2124"/>
       <source>Earphones On</source>
       <translation type="obsolete">Écouter sur l'oreille</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2107"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2124"/>
       <source>Chan. 2 Level</source>
       <translation type="obsolete">Niveau can. 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2107"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2124"/>
       <source>All Files (*)</source>
       <translation type="obsolete">Tous les fichiers (*)</translation>
     </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
@@ -899,15 +906,15 @@
       <location filename="../audiometry_trainer/window_generate_case.py" line="64"/>
       <source>Save audiogram parameters</source>
       <translation>Sauvegarder les paramètres de l'audiogramme</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="68"/>
       <source>&amp;Edit</source>
-      <translation>&amp;Éditer</translation>
+      <translation>&amp;Édition</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="69"/>
       <source>Frequencies</source>
       <translation>Fréquences</translation>
     </message>
     <message>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_it.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_it.ts`

 * *Files 8% similar despite different names*

#### Comparing `audiometry_trainer-0.1.5/prep-release/audiometry_trainer_it.ts` & `audiometry_trainer-0.1.6/prep-release/audiometry_trainer_it.ts`

```diff
@@ -90,90 +90,90 @@
     </message>
   </context>
   <context>
     <name>SpreadsheetWidget</name>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Bone R mdp</source>
-      <translation>Ossea D. pnt. med.</translation>
+      <translation>Ossea pnt. med. D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Bone R width</source>
-      <translation>Ossea D. largh.</translation>
+      <translation>Ossea largh. D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>ABG R</source>
-      <translation type="unfinished"/>
+      <translation>Gap Aer.-Oss. D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>F. A. rate R</source>
-      <translation type="unfinished"/>
+      <translation>Tasso F.A. D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Lapse rate R</source>
-      <translation type="unfinished"/>
+      <translation>Tasso inatt. D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Gain R</source>
-      <translation type="unfinished"/>
+      <translation>Guadagno D</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Bone L mdp</source>
-      <translation type="unfinished"/>
+      <translation>Ossea pnt. med. S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Bone L width</source>
-      <translation type="unfinished"/>
+      <translation>Ossea largh. S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>ABG L</source>
-      <translation type="unfinished"/>
+      <translation>Gap Aer.-Oss. S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>F. A. rate L</source>
-      <translation type="unfinished"/>
+      <translation>Tasso F.A. S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Lapse rate L</source>
-      <translation type="unfinished"/>
+      <translation>Tasso inatt. S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="594"/>
       <source>Gain L</source>
-      <translation type="unfinished"/>
+      <translation>Guadagno S</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="680"/>
       <source>Copy</source>
-      <translation type="unfinished"/>
+      <translation>Copia</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="681"/>
       <source>Cut</source>
-      <translation type="unfinished"/>
+      <translation>Taglia</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="682"/>
       <source>Paste</source>
-      <translation type="unfinished"/>
+      <translation>Incolla</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/window_generate_case.py" line="683"/>
       <source>Set value</source>
-      <translation type="unfinished"/>
+      <translation>Imposta valore</translation>
     </message>
   </context>
   <context>
     <name>applicationWindow</name>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="101"/>
       <source>Frequency (kHz)</source>
@@ -181,20 +181,20 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="102"/>
       <source>Level (dB HL)</source>
       <translation>Intensità (dB HL)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Supra-aural</source>
-      <translation>Supra-aurale</translation>
+      <translation>Sovra-aurale</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1965"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1973"/>
       <source>Right</source>
       <translation>Destro</translation>
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="173"/>
       <source>Exit</source>
       <translation>Uscita</translation>
@@ -256,565 +256,570 @@
     </message>
     <message>
       <location filename="../audiometry_trainer/main_window.py" line="207"/>
       <source>Manual (pdf)</source>
       <translation>Manuale (pdf)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="211"/>
+      <source>Online video tutorials</source>
+      <translation type="unfinished"/>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>About audiometry_trainer</source>
       <translation>A proposito di audiometry_trainer</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="216"/>
+      <location filename="../audiometry_trainer/main_window.py" line="220"/>
       <source>?</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="222"/>
+      <location filename="../audiometry_trainer/main_window.py" line="226"/>
       <source>Chan. 1:</source>
       <translation>Can. 1:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Insert</source>
-      <translation type="unfinished"/>
+      <translation>Inserto</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1970"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1978"/>
       <source>Bone</source>
       <translation>Ossea</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1677"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1685"/>
       <source>Sound field</source>
-      <translation type="unfinished"/>
+      <translation>Campo sonoro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="234"/>
+      <location filename="../audiometry_trainer/main_window.py" line="238"/>
       <source>Select the transducer for the test ear.</source>
-      <translation type="unfinished"/>
+      <translation>Seleziona il trasduttore per l'orecchio test</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="239"/>
+      <location filename="../audiometry_trainer/main_window.py" line="243"/>
       <source>Test ear:</source>
       <translation>Orecchio test:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1784"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1792"/>
       <source>Left</source>
       <translation>Sinistro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="245"/>
+      <location filename="../audiometry_trainer/main_window.py" line="249"/>
       <source>Select the test ear (right or left).</source>
-      <translation type="unfinished"/>
+      <translation>Selezione l'orecchio test (destro o sinistro)</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="249"/>
+      <location filename="../audiometry_trainer/main_window.py" line="253"/>
       <source>Test ear status:</source>
       <translation>Stato dell'orecchio test:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1746"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1754"/>
       <source>Unaided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1748"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1756"/>
       <source>Aided</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="254"/>
+      <location filename="../audiometry_trainer/main_window.py" line="258"/>
       <source>Set the status (aided or unaided) of the test ear.</source>
-      <translation type="unfinished"/>
+      <translation>Imposta lo stato (con o senza protesi) dell'orecchio test</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="260"/>
+      <location filename="../audiometry_trainer/main_window.py" line="264"/>
       <source>Test ear coupling:</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1722"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
       <source>Dome (open)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1724"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
       <source>Dome (tulip)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1726"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1734"/>
       <source>Dome (single vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1728"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1736"/>
       <source>Dome (double vent)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1730"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1738"/>
       <source>Double dome (power)</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1732"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1740"/>
       <source>Earmold</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="265"/>
+      <location filename="../audiometry_trainer/main_window.py" line="269"/>
       <source>Select coupling option for the test ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="964"/>
-      <source>Lock channels</source>
-      <translation>Aggancia i canali</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="275"/>
-      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="278"/>
-      <source>Auto. thresh. search</source>
-      <translation>Ric. soglia auto</translation>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="281"/>
-      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
-      <translation type="unfinished"/>
-    </message>
-    <message>
-      <location filename="../audiometry_trainer/main_window.py" line="285"/>
+      <location filename="../audiometry_trainer/main_window.py" line="276"/>
       <source>Show response ear</source>
       <translation>Mostra l'orecchio che risponde</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="289"/>
+      <location filename="../audiometry_trainer/main_window.py" line="280"/>
       <source>Response light will turn red/blue if the right/left ear is responding. White if both ears respond.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="291"/>
+      <location filename="../audiometry_trainer/main_window.py" line="282"/>
       <source>Show response counts</source>
       <translation>Mostra la conta delle risposte</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="295"/>
+      <location filename="../audiometry_trainer/main_window.py" line="286"/>
       <source>Show the counts of responses on ascending level trials.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra la conta delle risposte per i trial d'intensità ascendente</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="298"/>
+      <location filename="../audiometry_trainer/main_window.py" line="290"/>
+      <source>Auto. thresh. search</source>
+      <translation>Ric. soglia auto</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="293"/>
+      <source>Perform an automatic threshold search using the Hughson-Westlake procedure.</source>
+      <translation>Esegui una ricerca della soglia automatica utilizzando la procedure di Hughson-Westlake</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="296"/>
       <source>Response light</source>
-      <translation>Segnale di risposta</translation>
+      <translation>Spia di risposta</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="305"/>
+      <location filename="../audiometry_trainer/main_window.py" line="303"/>
       <source>The light will turn on if the virtual listener responds to the stimulus.</source>
-      <translation type="unfinished"/>
+      <translation>La spia si accenderà se l'ascoltatore virtuale risponde allo stimolo</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="308"/>
+      <location filename="../audiometry_trainer/main_window.py" line="306"/>
       <source>Mark threshold</source>
       <translation>Marca la soglia</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="310"/>
+      <location filename="../audiometry_trainer/main_window.py" line="308"/>
       <source>Mark the threshold at the current level.</source>
-      <translation type="unfinished"/>
+      <translation>Marca la soglia al livello corrente</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="314"/>
+      <location filename="../audiometry_trainer/main_window.py" line="312"/>
       <source>No response</source>
       <translation>No risposta</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="316"/>
+      <location filename="../audiometry_trainer/main_window.py" line="314"/>
       <source>Mark in the audiogram that no response was obtained at the highest stimulus level.</source>
-      <translation type="unfinished"/>
+      <translation>Marca sull'audiogramma che nessuna risposta è stata ottenuta alla più alta intensità dello stimolo.</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="319"/>
+      <location filename="../audiometry_trainer/main_window.py" line="317"/>
       <source>Masking dilemma</source>
       <translation>Dilemma di mascheramento</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="319"/>
       <source>Mark in the audiogram that the current threshold cannot be established because of a masking dilemma.</source>
-      <translation type="unfinished"/>
+      <translation>Marca sull'audiogramma che la soglia attuale non può essere stabilita a causa di un dilemma di mascheramento</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="325"/>
+      <location filename="../audiometry_trainer/main_window.py" line="323"/>
       <source>Show estimated thresholds:</source>
       <translation>Mostra le soglie stimate:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="330"/>
+      <location filename="../audiometry_trainer/main_window.py" line="328"/>
       <source>Thresh. unm. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="334"/>
+      <location filename="../audiometry_trainer/main_window.py" line="332"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="339"/>
+      <location filename="../audiometry_trainer/main_window.py" line="337"/>
       <source>Thresh. unm. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="343"/>
+      <location filename="../audiometry_trainer/main_window.py" line="341"/>
       <source>Show the unmasked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="346"/>
+      <location filename="../audiometry_trainer/main_window.py" line="344"/>
       <source>Thresh. unm. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="350"/>
+      <location filename="../audiometry_trainer/main_window.py" line="348"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="353"/>
+      <location filename="../audiometry_trainer/main_window.py" line="351"/>
       <source>Thresh. unm. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="357"/>
+      <location filename="../audiometry_trainer/main_window.py" line="355"/>
       <source>Show the unmasked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="360"/>
+      <location filename="../audiometry_trainer/main_window.py" line="358"/>
       <source>Thresh. msk. air R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="364"/>
+      <location filename="../audiometry_trainer/main_window.py" line="362"/>
       <source>Show the masked air conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="367"/>
+      <location filename="../audiometry_trainer/main_window.py" line="365"/>
       <source>Thresh. msk. air L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="371"/>
+      <location filename="../audiometry_trainer/main_window.py" line="369"/>
       <source>Show the masked air conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="374"/>
+      <location filename="../audiometry_trainer/main_window.py" line="372"/>
       <source>Thresh. msk. bone R</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="378"/>
+      <location filename="../audiometry_trainer/main_window.py" line="376"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the right ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="381"/>
+      <location filename="../audiometry_trainer/main_window.py" line="379"/>
       <source>Thresh. msk. bone L</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="385"/>
+      <location filename="../audiometry_trainer/main_window.py" line="383"/>
       <source>Show the masked bone conduction thresholds that you've estimated for the left ear.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="389"/>
+      <location filename="../audiometry_trainer/main_window.py" line="387"/>
       <source>Show actual thresholds:</source>
-      <translation type="unfinished"/>
+      <translation>Mostra le soglie reali:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="393"/>
+      <location filename="../audiometry_trainer/main_window.py" line="391"/>
       <source>Thresh. air R</source>
-      <translation type="unfinished"/>
+      <translation>Soglia aera D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="396"/>
+      <location filename="../audiometry_trainer/main_window.py" line="394"/>
       <source>Show the expected air conduction thresholds for the right ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra le soglie per conduzione aerea attese per l'orecchio destro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="433"/>
+      <location filename="../audiometry_trainer/main_window.py" line="431"/>
       <source>CI</source>
       <translation>IC</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="402"/>
+      <location filename="../audiometry_trainer/main_window.py" line="400"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the right ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra gli intervalli di confidenza al 95% per le soglie aeree attese per l'orecchio destro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="405"/>
+      <location filename="../audiometry_trainer/main_window.py" line="403"/>
       <source>Thresh. air L</source>
-      <translation type="unfinished"/>
+      <translation>Soglia aerea S</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="408"/>
+      <location filename="../audiometry_trainer/main_window.py" line="406"/>
       <source>Show the expected air conduction thresholds for the left ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra le soglie aeree attese per l'orecchio sinistro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="414"/>
+      <location filename="../audiometry_trainer/main_window.py" line="412"/>
       <source>Show 95% confidence intervals for the expected air conduction thresholds for the left ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra gli intervalli di confidenza al 95% per le soglie aeree attese per l'orecchio sinistro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="417"/>
+      <location filename="../audiometry_trainer/main_window.py" line="415"/>
       <source>Thresh. bone R</source>
-      <translation type="unfinished"/>
+      <translation>Soglia ossea D</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="420"/>
+      <location filename="../audiometry_trainer/main_window.py" line="418"/>
       <source>Show the expected bone conduction thresholds for the right ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra le soglie osee attese per l'orecchio destro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="425"/>
+      <location filename="../audiometry_trainer/main_window.py" line="423"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the right ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra gli intervalli di confidenza al 95% per le soglie osee attese per l'orecchio destro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="428"/>
+      <location filename="../audiometry_trainer/main_window.py" line="426"/>
       <source>Thresh. bone L</source>
-      <translation type="unfinished"/>
+      <translation>Soglia ossea S</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="431"/>
+      <location filename="../audiometry_trainer/main_window.py" line="429"/>
       <source>Show the expected bone conduction thresholds for the left ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra le soglie osee attese per l'orecchio sinistro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="436"/>
+      <location filename="../audiometry_trainer/main_window.py" line="434"/>
       <source>Show 95% confidence intervals for the expected bone conduction thresholds for the left ear.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra gli intervalli di confidenza al 95% per le soglie osee attese per l'orecchio sinistro</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="452"/>
+      <location filename="../audiometry_trainer/main_window.py" line="450"/>
       <source>Non-test ear status:</source>
-      <translation type="unfinished"/>
+      <translation type="unfinished">Stato dell'orecchio non testato:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1639"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1647"/>
       <source>Uncovered</source>
-      <translation type="unfinished"/>
+      <translation>Scoperto</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1684"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1692"/>
       <source>Earphone on</source>
-      <translation type="unfinished"/>
+      <translation>Auricolare sull'orecchio</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="446"/>
+      <location filename="../audiometry_trainer/main_window.py" line="444"/>
       <source>Indicate whether the virtual listener has an earphone on the non-test ear or not. Comparing these two conditions (while no masking noise is being played) can be used to estimate the occlusion effect.</source>
-      <translation type="unfinished"/>
+      <translation>Indicare se l'ascoltatore virtuale ha un auricolare sull'orecchio test o no. Una comparazione di queste due condizioni (senza riproduzione di rumore attraverso l'auricolare) può essere utile a stimare l'entità dell'effetto d'occlusione</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1715"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1723"/>
       <source>Chan. 2</source>
       <translation>Can. 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1689"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1697"/>
       <source>Earplug</source>
-      <translation type="unfinished"/>
+      <translation>Tappo</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="457"/>
+      <location filename="../audiometry_trainer/main_window.py" line="455"/>
       <source>Select the status of the non-test ear.</source>
-      <translation type="unfinished"/>
+      <translation>Seleziona lo stato dell'orecchio non testato</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="463"/>
+      <location filename="../audiometry_trainer/main_window.py" line="461"/>
       <source>Chan. 2:</source>
       <translation>Can. 2:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="472"/>
+      <location filename="../audiometry_trainer/main_window.py" line="470"/>
       <source>Select the transducer to deliver masking noise through channel 2.</source>
-      <translation type="unfinished"/>
+      <translation>Seleziona il trasduttore per inviare il rumore attraverso il canale 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="476"/>
+      <location filename="../audiometry_trainer/main_window.py" line="474"/>
       <source>Chan. 2 level</source>
       <translation>Intensità can. 2</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="482"/>
+      <location filename="../audiometry_trainer/main_window.py" line="480"/>
       <source>Input the level, in dB of effective masking (EM), of the masking noise.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="489"/>
+      <location filename="../audiometry_trainer/main_window.py" line="487"/>
       <source>Increase the level of the masking noise.</source>
-      <translation type="unfinished"/>
+      <translation>Aumenta l'intensità del rumore mascherante</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="493"/>
+      <location filename="../audiometry_trainer/main_window.py" line="491"/>
       <source>-</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="496"/>
+      <location filename="../audiometry_trainer/main_window.py" line="494"/>
       <source>Decrease the level of the masking noise.</source>
-      <translation type="unfinished"/>
+      <translation>Diminuisci l'intensità del rumore mascherante</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="501"/>
+      <location filename="../audiometry_trainer/main_window.py" line="499"/>
       <source>Chan. 2 ON</source>
       <translation>Can. 2 ON</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="504"/>
+      <location filename="../audiometry_trainer/main_window.py" line="502"/>
       <source>Turn ON the masking noise in channel 2.</source>
+      <translation>Avvia il rumore mascherante sul canale 2</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="972"/>
+      <source>Lock channels</source>
+      <translation>Aggancia i canali</translation>
+    </message>
+    <message>
+      <location filename="../audiometry_trainer/main_window.py" line="510"/>
+      <source>Lock the channels so that changing the stimulus level automatically changes the masking noise level by the same amount.</source>
       <translation type="unfinished"/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="509"/>
+      <location filename="../audiometry_trainer/main_window.py" line="514"/>
       <source>Show case filename</source>
       <translation>Nome del file di caso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="513"/>
+      <location filename="../audiometry_trainer/main_window.py" line="518"/>
       <source>Show the filename of the case currently loaded.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra il nome del file del caso attualmente caricato</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="516"/>
+      <location filename="../audiometry_trainer/main_window.py" line="521"/>
       <source>Show case info</source>
       <translation>Informazione del caso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="520"/>
+      <location filename="../audiometry_trainer/main_window.py" line="525"/>
       <source>Show the information available for the case currently loaded.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra l'informazione disponibile sul caso attualmente caricato</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="524"/>
+      <location filename="../audiometry_trainer/main_window.py" line="529"/>
       <source>Case file:</source>
       <translation>File del caso:</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="541"/>
+      <location filename="../audiometry_trainer/main_window.py" line="546"/>
       <source>Grid</source>
       <translation>Griglia</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="545"/>
+      <location filename="../audiometry_trainer/main_window.py" line="550"/>
       <source>Show a grid on the audiogram plot.</source>
-      <translation type="unfinished"/>
+      <translation>Mostra una griglia sull'audiogramma</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="554"/>
+      <location filename="../audiometry_trainer/main_window.py" line="559"/>
       <source>This light will turn on when a stimulus is being played on channel 1.</source>
-      <translation type="unfinished"/>
+      <translation>Questa spia si accende quando uno stimolo è in corso di riproduzione sul canale 1</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="555"/>
+      <location filename="../audiometry_trainer/main_window.py" line="560"/>
       <source>Stimulus light</source>
-      <translation>Segnale dello stimolo</translation>
+      <translation>Spia dello stimolo</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="558"/>
+      <location filename="../audiometry_trainer/main_window.py" line="563"/>
       <source>Play stimulus</source>
       <translation>Riproduci lo stimolo</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="562"/>
+      <location filename="../audiometry_trainer/main_window.py" line="567"/>
       <source>Play the stimulus on channel 1.</source>
-      <translation type="unfinished"/>
+      <translation>Riproduci lo stimolo sul canale 1</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="880"/>
+      <location filename="../audiometry_trainer/main_window.py" line="885"/>
       <source>No case info available</source>
       <translation>No informazione del caso disponibile</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>Choose case file to load</source>
       <translation>Scegli il file di caso da caricare</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="883"/>
+      <location filename="../audiometry_trainer/main_window.py" line="888"/>
       <source>CSV files (*.csv *CSV *Csv);;All Files (*)</source>
       <translation/>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="960"/>
+      <location filename="../audiometry_trainer/main_window.py" line="968"/>
       <source>Unlock channels</source>
       <translation>Sgancia i canali</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Warning</source>
       <translation>Avvertimento</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1293"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1301"/>
       <source>Requested channel 2 value out of limits for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il valore richiesto per il canale 2 va oltre i limiti del trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1307"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1315"/>
       <source>Channel 2 has reached its maximum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 2 ha raggiunto il livello di intensità massima per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1321"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1329"/>
       <source>Channel 2 has reached its minimum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 2 ha raggiunto il livello minimo per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1363"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1371"/>
       <source>Channel 1 has reached the minimum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 1 ha raggiunto il livello minimo per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1369"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1377"/>
       <source>Channel 2 is locked to channel 1 and has reached its minimum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 2 è agganciato al canale 1 ed ha raggiunto il livello minimo per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1380"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1388"/>
       <source>Channel 1 has reached the maximum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 1 ha raggiunto il livello massimo per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1386"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1394"/>
       <source>Channel 2 is locked to channel 1 and has reached its maximum level for the current transducers</source>
-      <translation type="unfinished"/>
+      <translation>Il canale 2 è agganciato al canale 1 ed ha raggiunto il livello massimo per il trasduttore in uso</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1435"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1443"/>
       <source>Automatic threshold search does not work when channel 2 is ON</source>
-      <translation type="unfinished"/>
+      <translation>La ricerca automatica della soglia non funziona quando il canale 2 è attivato</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="1652"/>
+      <location filename="../audiometry_trainer/main_window.py" line="1660"/>
       <source>Circum-aural</source>
-      <translation type="unfinished"/>
+      <translation>Circumaurale</translation>
     </message>
     <message>
-      <location filename="../audiometry_trainer/main_window.py" line="2106"/>
+      <location filename="../audiometry_trainer/main_window.py" line="2123"/>
       <source>&lt;b&gt;audiometry_trainer&lt;/b&gt; &lt;br&gt;
                                 - version: {0}; &lt;br&gt;
                                 - build date: {1} &lt;br&gt;
                                 &lt;p&gt; Copyright &amp;copy; 2023-2024 Samuele Carcagno. &lt;a href=&quot;mailto:sam.carcagno@gmail.com&quot;&gt;sam.carcagno@gmail.com&lt;/a&gt; 
                                 All rights reserved. &lt;p&gt;
                 This program is free software: you can redistribute it and/or modify
                 it under the terms of the GNU General Public License as published by
@@ -824,14 +829,16 @@
                 This program is distributed in the hope that it will be useful,
                 but WITHOUT ANY WARRANTY; without even the implied warranty of
                 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
                 GNU General Public License for more details.
                 &lt;p&gt;
                 You should have received a copy of the GNU General Public License
                 along with this program.  If not, see &lt;a href=&quot;http://www.gnu.org/licenses/&quot;&gt;http://www.gnu.org/licenses/&lt;/a&gt;
+
+                &lt;p&gt; A number of icons are from Font Awesome, released under the &lt;a href=&quot;https://creativecommons.org/licenses/by/4.0/&quot;&gt;CC BY 4.0 license&lt;/a&gt;. See &lt;a href=&quot;https://gitlab.com/sam81/audiometry_trainer/-/blob/main/CREDITS.txt?ref_type=heads&quot;&gt;CREDITS.txt&lt;/a&gt; in the source distribution for details.
                 &lt;p&gt;Python {2} - {3} {4} compiled against Qt {5}, and running with Qt {6} on {7}</source>
       <translation type="unfinished"/>
     </message>
   </context>
   <context>
     <name>applyChanges</name>
     <message>
```

### Comparing `audiometry_trainer-0.1.5/prep-release/mkupdate_pyqt6.sh` & `audiometry_trainer-0.1.6/prep-release/mkupdate_pyqt6.sh`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/release.py` & `audiometry_trainer-0.1.6/prep-release/release.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/switch_pyqt5.py` & `audiometry_trainer-0.1.6/prep-release/switch_pyqt5.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/switch_pyqt6.py` & `audiometry_trainer-0.1.6/prep-release/switch_pyqt6.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/prep-release/win_audiometry_trainer.iss` & `audiometry_trainer-0.1.6/prep-release/win_audiometry_trainer.iss`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ; Script generated by the Inno Setup Script Wizard.
 ; SEE THE DOCUMENTATION FOR DETAILS ON CREATING INNO SETUP SCRIPT FILES!
 
 #define MyAppName "audiometry_trainer"
-#define MyAppVersion "0.1.5"
+#define MyAppVersion "0.1.6"
 #define MyAppPublisher "Samuele Carcagno"
 #define MyAppURL "https://samcarcagno.altervista.org/audiometry_trainer/audiometry_trainer.html"
 #define MyAppExeName "audiometry_trainer.exe"
 
 [Setup]
 ; NOTE: The value of AppId uniquely identifies this application. Do not use the same AppId value in installers for other applications.
 ; (To generate a new GUID, click Tools | Generate GUID inside the IDE.)
```

### Comparing `audiometry_trainer-0.1.5/prep-release/winbuild.py` & `audiometry_trainer-0.1.6/prep-release/winbuild.py`

 * *Files identical despite different names*

### Comparing `audiometry_trainer-0.1.5/pyproject.toml` & `audiometry_trainer-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "audiometry_trainer"
-    version="0.1.5"
+    version="0.1.6"
 
 authors = [
   { name="Samuele Carcagno", email="sam.carcagno@gmail.com" },
 ]
 description = "Clinical audiometry simulator"
 license = {file = "COPYING.txt"}
 readme = "README.md"
```

### Comparing `audiometry_trainer-0.1.5/resources.qrc` & `audiometry_trainer-0.1.6/resources.qrc`

 * *Files 22% similar despite different names*

```diff
@@ -5,22 +5,29 @@
 <file>translations/audiometry_trainer_es.qm</file>
 <file>translations/audiometry_trainer_el.qm</file>
 <file>translations/audiometry_trainer_en_US.qm</file>
 <file>translations/audiometry_trainer_en_GB.qm</file>
 <file alias="audiometry_trainer_icon">icons/audiometry_trainer_icon.svg</file>
 <file alias="arrow-down-solid">icons/arrow-down-solid.svg</file>
 <file alias="arrow-up-solid">icons/arrow-up-solid.svg</file>
+<file alias="book-solid">icons/book-solid.svg</file>
+<file alias="book-bookmark-solid">icons/book-bookmark-solid.svg</file>
+<file alias="circle-info-solid">icons/circle-info-solid.svg</file>
 <file alias="dice-solid">icons/dice-solid.svg</file>
-<file alias="exit">icons/exit.svg</file>
+<file alias="film-solid">icons/film-solid.svg</file>
+<file alias="floppy-disk-solid">icons/floppy-disk-solid.svg</file>
 <file alias="folder-open-regular">icons/folder-open-regular.svg</file>
+<file alias="gears-solid">icons/gears-solid.svg</file>
 <file alias="headphones-solid">icons/headphones-solid.svg</file>
-<file alias="help-about">icons/help-about.svgz</file>
-<file alias="help-contents">icons/help-contents.svgz</file>
-<file alias="help-contextual">icons/help-contextual.svgz</file>
 <file alias="insert">icons/insert.svg</file>
-<file alias="preferences-other">icons/preferences-other.svgz</file>
 <file alias="lock-open-solid">icons/lock-open-solid.svg</file>
 <file alias="lock-solid">icons/lock-solid.svg</file>
 <file alias="mask-solid">icons/mask-solid.svg</file>
+<file alias="mask-solid-off">icons/mask-solid-off.svg</file>
+<file alias="person-running-solid">icons/person-running-solid.svg</file>
+<file alias="question-solid">icons/question-solid.svg</file>
+<file alias="right-from-bracket-solid">icons/right-from-bracket-solid.svg</file>
+<file alias="robot-solid">icons/robot-solid.svg</file>
 <file alias="skull-solid">icons/skull-solid.svg</file>
+<file alias="sliders-solid">icons/sliders-solid.svg</file>
 </qresource>
 </RCC>
```

### Comparing `audiometry_trainer-0.1.5/setup_cx.py` & `audiometry_trainer-0.1.6/setup_cx.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,11 +21,11 @@
                base=base,
                target_name = 'audiometry_trainer',
                icon='icons/audiometry_trainer_icon.ico'
                )
 ]
 
 setup(name='audiometry_trainer',
-    version="0.1.5",
+    version="0.1.6",
       description = '',
       options = {'build_exe': build_options},
       executables = executables)
```

