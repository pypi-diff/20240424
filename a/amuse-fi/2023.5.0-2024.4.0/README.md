# Comparing `tmp/amuse-fi-2023.5.0.tar.gz` & `tmp/amuse-fi-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-fi-2023.5.0.tar", last modified: Wed May 17 10:18:31 2023, max compression
+gzip compressed data, was "amuse-fi-2024.4.0.tar", last modified: Wed Apr 24 16:32:07 2024, max compression
```

## Comparing `amuse-fi-2023.5.0.tar` & `amuse-fi-2024.4.0.tar`

### file list

```diff
@@ -1,230 +1,230 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.840019 amuse-fi-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-fi-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1174 2023-05-17 10:18:31.839844 amuse-fi-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       55 2022-11-22 11:55:14.000000 amuse-fi-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.787991 amuse-fi-2023.5.0/amuse_fi.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1174 2023-05-17 10:18:30.000000 amuse-fi-2023.5.0/amuse_fi.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)     9579 2023-05-17 10:18:31.000000 amuse-fi-2023.5.0/amuse_fi.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:30.000000 amuse-fi-2023.5.0/amuse_fi.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:18:30.000000 amuse-fi-2023.5.0/amuse_fi.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:30.000000 amuse-fi-2023.5.0/amuse_fi.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-fi-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:31.840064 amuse-fi-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1749 2022-11-22 11:55:14.000000 amuse-fi-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.786455 amuse-fi-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.786507 amuse-fi-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.786563 amuse-fi-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.789202 amuse-fi-2023.5.0/src/amuse/community/fi/
--rw-r--r--   0 rieder     (501) staff       (20)     8604 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      570 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/README
--rw-r--r--   0 rieder     (501) staff       (20)       33 2023-03-16 12:23:56.000000 amuse-fi-2023.5.0/src/amuse/community/fi/__init__.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.789339 amuse-fi-2023.5.0/src/amuse/community/fi/data/
--rw-r--r--   0 rieder     (501) staff       (20)      417 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/README.txt
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.827174 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/
--rw-r--r--   0 rieder     (501) staff       (20)     3248 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/C.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6504 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/C.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3245 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Fe.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     3603 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Fe.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H.cool
--rw-r--r--   0 rieder     (501) staff       (20)    23682 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.H2cool
--rw-r--r--   0 rieder     (501) staff       (20)    23677 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.HH2cool
--rw-r--r--   0 rieder     (501) staff       (20)    23681 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/He.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/He.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/N.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/N.cool
--rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Ne.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Ne.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3253 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/O.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/O.cool
--rw-r--r--   0 rieder     (501) staff       (20)     3252 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Si.Hcool
--rw-r--r--   0 rieder     (501) staff       (20)     2703 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Si.cool
--rw-r--r--   0 rieder     (501) staff       (20)   388874 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_02_10.halo
--rw-r--r--   0 rieder     (501) staff       (20)   387117 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_12_10_023.halo
--rw-r--r--   0 rieder     (501) staff       (20)   389434 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_18_06_10.halo
--rw-r--r--   0 rieder     (501) staff       (20)   390037 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_2_10_0045.halo
--rw-r--r--   0 rieder     (501) staff       (20)   390535 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_1.25.halo
--rw-r--r--   0 rieder     (501) staff       (20)   386828 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_1.8.halo
--rw-r--r--   0 rieder     (501) staff       (20)   386365 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_2.2.halo
--rw-r--r--   0 rieder     (501) staff       (20)   232230 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burkct_4_20_02.halo
--rw-r--r--   0 rieder     (501) staff       (20)   231759 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burkct_4_20_04.halo
--rw-r--r--   0 rieder     (501) staff       (20)       63 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/extinctionlaw
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_102_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)  1413118 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_124_12.halo
--rw-r--r--   0 rieder     (501) staff       (20)  1412343 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_144_12.halo
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_181_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_195_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_50_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)   613922 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_50_3.halo
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_55_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_96_2.halo
--rw-r--r--   0 rieder     (501) staff       (20)   232872 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_04_20_32.halo
--rw-r--r--   0 rieder     (501) staff       (20)   228699 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_10_40_02
--rw-r--r--   0 rieder     (501) staff       (20)   228699 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_10_40_02.halo
--rw-r--r--   0 rieder     (501) staff       (20)   387068 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2.6_40_0044.halo
--rw-r--r--   0 rieder     (501) staff       (20)    75791 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_005.halo
--rw-r--r--   0 rieder     (501) staff       (20)    75537 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_01.halo
--rw-r--r--   0 rieder     (501) staff       (20)    75299 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_02.halo
--rw-r--r--   0 rieder     (501) staff       (20)    74261 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_04.halo
--rw-r--r--   0 rieder     (501) staff       (20)    74017 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_08.halo
--rw-r--r--   0 rieder     (501) staff       (20)   229348 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_40_1.halo
--rw-r--r--   0 rieder     (501) staff       (20)    92475 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_3_30_1.halo
--rw-r--r--   0 rieder     (501) staff       (20)   230551 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_4_40_06.halo
--rw-r--r--   0 rieder     (501) staff       (20)   229049 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_6_40_025.halo
--rw-r--r--   0 rieder     (501) staff       (20)   230343 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_6_40_04.halo
--rw-r--r--   0 rieder     (501) staff       (20)   387603 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_7_40_00088
--rw-r--r--   0 rieder     (501) staff       (20)   387603 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_7_40_00088.halo
--rw-r--r--   0 rieder     (501) staff       (20)  1130171 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_004_6.halo
--rw-r--r--   0 rieder     (501) staff       (20)   389780 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_12_10_015.halo
--rw-r--r--   0 rieder     (501) staff       (20)   390976 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_2_10_0036.halo
--rw-r--r--   0 rieder     (501) staff       (20)   460781 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfwct_2_20_149.halo
--rw-r--r--   0 rieder     (501) staff       (20)      186 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/readme
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_emp.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_emp.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z008.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z008.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z02.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z02.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z05.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z05.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z10.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z10.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_emp.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_emp.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z008.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z008.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z02.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z02.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z05.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z05.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z10.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z10.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_emp.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_emp.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z004.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z004.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z008.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z008.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z02.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z02.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z05.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z05.starprop
--rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z10.starmodel
--rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z10.starprop
--rw-r--r--   0 rieder     (501) staff       (20)     2752 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/data/input/uvpol10_10
--rw-r--r--   0 rieder     (501) staff       (20)    29402 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)   145248 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/src/amuse/community/fi/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/map_interface.f90
--rwxr-xr-x   0 rieder     (501) staff       (20)     2385 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/patch_globals_dot_h.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.838390 amuse-fi-2023.5.0/src/amuse/community/fi/src/
--rw-r--r--   0 rieder     (501) staff       (20)     3577 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/H2cool.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5269 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     8093 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/blackhole.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3839 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/buildnearlist.f90
--rw-r--r--   0 rieder     (501) staff       (20)    14854 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/buildtree.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6744 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/clean.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1293 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/combine_simple.f90
--rw-r--r--   0 rieder     (501) staff       (20)      699 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/coolcurve.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7179 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/cooling.f90
--rw-r--r--   0 rieder     (501) staff       (20)    13104 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/density.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3888 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/diagnostics.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3908 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/elements.f90
--rw-r--r--   0 rieder     (501) staff       (20)    23610 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/entdot.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7018 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/ethstep.f90
--rw-r--r--   0 rieder     (501) staff       (20)       72 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/extern_dummy.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5242 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/extract.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5249 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fcco.f90
--rw-r--r--   0 rieder     (501) staff       (20)    17962 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/feedback.f90
--rw-r--r--   0 rieder     (501) staff       (20)     2373 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fftw3.f
--rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fi.f90
--rw-r--r--   0 rieder     (501) staff       (20)    27314 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fi_viewer.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7231 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fixedhalo.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fthread.f
--rw-r--r--   0 rieder     (501) staff       (20)     2491 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/fuvflux.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1685 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/glfi.f90
--rw-r--r--   0 rieder     (501) staff       (20)    12584 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/globals_template.h
--rw-r--r--   0 rieder     (501) staff       (20)     5425 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/gravity.f90
--rw-r--r--   0 rieder     (501) staff       (20)     9085 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/gravsum.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1256 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/hash.f90
--rw-r--r--   0 rieder     (501) staff       (20)      786 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/heating.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3911 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/heco.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7279 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/hicube.f90
--rw-r--r--   0 rieder     (501) staff       (20)      373 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/image
--rw-r--r--   0 rieder     (501) staff       (20)     6815 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/init.f90
--rw-r--r--   0 rieder     (501) staff       (20)    12082 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/io-old.f
--rw-r--r--   0 rieder     (501) staff       (20)     4424 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/io.f90
--rw-r--r--   0 rieder     (501) staff       (20)    18639 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/io2.f90
--rw-r--r--   0 rieder     (501) staff       (20)    11653 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/ionize.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1388 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/makemap.f90
--rw-r--r--   0 rieder     (501) staff       (20)    13085 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/makemapmod.f90
--rw-r--r--   0 rieder     (501) staff       (20)     8644 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/map_helpers.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3472 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/mem.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7805 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/molecules.f90
--rw-r--r--   0 rieder     (501) staff       (20)    44011 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_helpers.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7849 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)       55 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_interface_gl.f90
--rw-r--r--   0 rieder     (501) staff       (20)      793 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_io2_stub.f90
--rw-r--r--   0 rieder     (501) staff       (20)      163 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_io_stub.f90
--rw-r--r--   0 rieder     (501) staff       (20)    10666 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/pmgrav.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5793 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/ppread.f90
--rw-r--r--   0 rieder     (501) staff       (20)    14101 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/project.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6077 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/pt.c
--rw-r--r--   0 rieder     (501) staff       (20)     6858 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/pt.h
--rw-r--r--   0 rieder     (501) staff       (20)      998 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/ptf77.c
--rw-r--r--   0 rieder     (501) staff       (20)      729 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/random.f90
--rw-r--r--   0 rieder     (501) staff       (20)    19968 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/readparam.f90
--rw-r--r--   0 rieder     (501) staff       (20)     8330 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/rgabe.f90
--rw-r--r--   0 rieder     (501) staff       (20)     2671 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/rgabe2.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3700 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/rgadget.f90
--rw-r--r--   0 rieder     (501) staff       (20)     2419 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/rsimple.f90
--rw-r--r--   0 rieder     (501) staff       (20)    21176 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/search.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3321 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh2.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3150 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh3.f90
--rw-r--r--   0 rieder     (501) staff       (20)      684 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sfinfo.f90
--rw-r--r--   0 rieder     (501) staff       (20)     1077 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/snapreader.f90
--rw-r--r--   0 rieder     (501) staff       (20)    21935 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/snapviewer.f90
--rw-r--r--   0 rieder     (501) staff       (20)     4106 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sort.f90
--rw-r--r--   0 rieder     (501) staff       (20)    11705 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/sphray_io.f90
--rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/starprop.f90
--rw-r--r--   0 rieder     (501) staff       (20)    27611 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/stars3d.f90
--rw-r--r--   0 rieder     (501) staff       (20)     8260 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/stellar.f90
--rw-r--r--   0 rieder     (501) staff       (20)     8264 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/stepsystem.f90
--rw-r--r--   0 rieder     (501) staff       (20)     2116 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/tidalsum.f90
--rw-r--r--   0 rieder     (501) staff       (20)     5209 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/timestep.f90
--rw-r--r--   0 rieder     (501) staff       (20)     9000 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/togabe.f90
--rw-r--r--   0 rieder     (501) staff       (20)     3810 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/togabe2.f90
--rw-r--r--   0 rieder     (501) staff       (20)      838 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/tosimple.f90
--rw-r--r--   0 rieder     (501) staff       (20)     2481 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/tosimplex.f90
--rw-r--r--   0 rieder     (501) staff       (20)    15902 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/treewalk.f90
--rw-r--r--   0 rieder     (501) staff       (20)      970 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/update_tree.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6931 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/util.f90
--rw-r--r--   0 rieder     (501) staff       (20)    16465 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/src/amuse/community/fi/src/varia.f90
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:30.000000 amuse-fi-2023.5.0/src/amuse/community/fi/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:31.839613 amuse-fi-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-fi-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-fi-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-fi-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.703833 amuse-fi-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-fi-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1205 2024-04-24 16:32:07.703618 amuse-fi-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       55 2022-11-22 11:55:14.000000 amuse-fi-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.703308 amuse-fi-2024.4.0/amuse_fi.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1205 2024-04-24 16:32:06.000000 amuse-fi-2024.4.0/amuse_fi.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)     9580 2024-04-24 16:32:07.000000 amuse-fi-2024.4.0/amuse_fi.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:06.000000 amuse-fi-2024.4.0/amuse_fi.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:06.000000 amuse-fi-2024.4.0/amuse_fi.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:06.000000 amuse-fi-2024.4.0/amuse_fi.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-fi-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:07.703904 amuse-fi-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1557 2024-04-24 15:35:29.000000 amuse-fi-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.650143 amuse-fi-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.650193 amuse-fi-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.650242 amuse-fi-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.653592 amuse-fi-2024.4.0/src/amuse/community/fi/
+-rw-r--r--   0 rieder     (501) staff       (20)     8604 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      570 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/README
+-rw-r--r--   0 rieder     (501) staff       (20)       33 2023-03-16 12:23:56.000000 amuse-fi-2024.4.0/src/amuse/community/fi/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:06.000000 amuse-fi-2024.4.0/src/amuse/community/fi/_version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.653775 amuse-fi-2024.4.0/src/amuse/community/fi/data/
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/README.txt
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.687586 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/
+-rw-r--r--   0 rieder     (501) staff       (20)     3248 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/C.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6504 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/C.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3245 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Fe.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     3603 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Fe.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H.cool
+-rw-r--r--   0 rieder     (501) staff       (20)    23682 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.H2cool
+-rw-r--r--   0 rieder     (501) staff       (20)    23677 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.HH2cool
+-rw-r--r--   0 rieder     (501) staff       (20)    23681 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/He.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/He.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/N.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/N.cool
+-rw-r--r--   0 rieder     (501) staff       (20)        2 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Ne.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Ne.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3253 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/O.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     6084 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/O.cool
+-rw-r--r--   0 rieder     (501) staff       (20)     3252 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Si.Hcool
+-rw-r--r--   0 rieder     (501) staff       (20)     2703 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Si.cool
+-rw-r--r--   0 rieder     (501) staff       (20)   388874 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_02_10.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   387117 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_12_10_023.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   389434 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_18_06_10.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   390037 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_2_10_0045.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   390535 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_1.25.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   386828 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_1.8.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   386365 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_2.2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   232230 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burkct_4_20_02.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   231759 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burkct_4_20_04.halo
+-rw-r--r--   0 rieder     (501) staff       (20)       63 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/extinctionlaw
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_102_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  1413118 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_124_12.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  1412343 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_144_12.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_181_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_195_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_50_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   613922 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_50_3.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_55_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  2910187 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_96_2.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   232872 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_04_20_32.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   228699 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_10_40_02
+-rw-r--r--   0 rieder     (501) staff       (20)   228699 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_10_40_02.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   387068 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2.6_40_0044.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    75791 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_005.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    75537 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_01.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    75299 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_02.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    74261 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_04.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    74017 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_08.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   229348 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_40_1.halo
+-rw-r--r--   0 rieder     (501) staff       (20)    92475 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_3_30_1.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   230551 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_4_40_06.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   229049 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_6_40_025.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   230343 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_6_40_04.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   387603 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_7_40_00088
+-rw-r--r--   0 rieder     (501) staff       (20)   387603 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_7_40_00088.halo
+-rw-r--r--   0 rieder     (501) staff       (20)  1130171 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_004_6.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   389780 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_12_10_015.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   390976 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_2_10_0036.halo
+-rw-r--r--   0 rieder     (501) staff       (20)   460781 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfwct_2_20_149.halo
+-rw-r--r--   0 rieder     (501) staff       (20)      186 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/readme
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_emp.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_emp.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z008.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z008.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z02.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z02.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z05.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z05.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z10.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z10.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_emp.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_emp.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z008.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z008.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z02.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z02.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z05.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z05.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z10.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z10.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_emp.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_emp.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z004.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z004.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z008.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z008.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z02.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z02.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z05.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z05.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)    28750 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z10.starmodel
+-rw-r--r--   0 rieder     (501) staff       (20)    26977 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z10.starprop
+-rw-r--r--   0 rieder     (501) staff       (20)     2752 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/src/amuse/community/fi/data/input/uvpol10_10
+-rw-r--r--   0 rieder     (501) staff       (20)    29402 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)   145222 2024-04-24 15:35:29.000000 amuse-fi-2024.4.0/src/amuse/community/fi/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/map_interface.f90
+-rwxr-xr-x   0 rieder     (501) staff       (20)     2385 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/patch_globals_dot_h.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.701794 amuse-fi-2024.4.0/src/amuse/community/fi/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     3577 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/H2cool.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5269 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     8093 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/blackhole.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3839 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/buildnearlist.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    14854 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/buildtree.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6744 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/clean.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1293 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/combine_simple.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      699 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/coolcurve.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7179 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/cooling.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    13104 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/density.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3888 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/diagnostics.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3908 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/elements.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    23610 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/entdot.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7018 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/ethstep.f90
+-rw-r--r--   0 rieder     (501) staff       (20)       72 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/extern_dummy.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5242 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/extract.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5249 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fcco.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    17962 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/feedback.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     2373 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fftw3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1635 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fi.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    27314 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fi_viewer.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7231 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fixedhalo.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fthread.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2491 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/fuvflux.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1685 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/glfi.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    12584 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/globals_template.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5425 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/gravity.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     9085 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/gravsum.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1256 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/hash.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      786 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/heating.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3911 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/heco.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7279 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/hicube.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      373 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/image
+-rw-r--r--   0 rieder     (501) staff       (20)     6815 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/init.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    12082 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/io-old.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4424 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/io.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    18639 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/io2.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    11653 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/ionize.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1388 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/makemap.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    13085 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/makemapmod.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     8644 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/map_helpers.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3472 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/mem.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7805 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/molecules.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    44011 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_helpers.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7849 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)       55 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_interface_gl.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      793 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_io2_stub.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      163 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_io_stub.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    10666 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/pmgrav.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5793 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/ppread.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    14101 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/project.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6077 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/pt.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6858 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/pt.h
+-rw-r--r--   0 rieder     (501) staff       (20)      998 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/ptf77.c
+-rw-r--r--   0 rieder     (501) staff       (20)      729 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/random.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    19968 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/readparam.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     8330 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/rgabe.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     2671 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/rgabe2.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3700 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/rgadget.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     2419 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/rsimple.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    21176 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/search.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3321 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3591 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh2.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3150 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh3.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      684 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sfinfo.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     1077 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/snapreader.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    21935 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/snapviewer.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     4106 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sort.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    11705 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/sphray_io.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     4532 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/starprop.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    27611 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/stars3d.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     8260 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/stellar.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     8264 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/stepsystem.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     2116 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/tidalsum.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     5209 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/timestep.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     9000 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/togabe.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     3810 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/togabe2.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      838 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/tosimple.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     2481 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/tosimplex.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    15902 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/treewalk.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      970 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/update_tree.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6931 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/util.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    16465 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/src/amuse/community/fi/src/varia.f90
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:07.703114 amuse-fi-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-fi-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-fi-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-fi-2024.4.0/support/version.py
```

### Comparing `amuse-fi-2023.5.0/PKG-INFO` & `amuse-fi-2024.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-fi
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - FI
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the FI community code for AMUSE.
```

### Comparing `amuse-fi-2023.5.0/amuse_fi.egg-info/PKG-INFO` & `amuse-fi-2024.4.0/amuse_fi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-fi
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - FI
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,11 +19,12 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: amuse-framework
 
 This package installs the FI community code for AMUSE.
```

### Comparing `amuse-fi-2023.5.0/amuse_fi.egg-info/SOURCES.txt` & `amuse-fi-2024.4.0/amuse_fi.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 amuse_fi.egg-info/SOURCES.txt
 amuse_fi.egg-info/dependency_links.txt
 amuse_fi.egg-info/requires.txt
 amuse_fi.egg-info/top_level.txt
 src/amuse/community/fi/Makefile
 src/amuse/community/fi/README
 src/amuse/community/fi/__init__.py
+src/amuse/community/fi/_version.py
 src/amuse/community/fi/interface.f90
 src/amuse/community/fi/interface.py
 src/amuse/community/fi/map_interface.f90
 src/amuse/community/fi/patch_globals_dot_h.py
-src/amuse/community/fi/version.py
 src/amuse/community/fi/data/README.txt
 src/amuse/community/fi/data/input/C.Hcool
 src/amuse/community/fi/data/input/C.cool
 src/amuse/community/fi/data/input/Fe.Hcool
 src/amuse/community/fi/data/input/Fe.cool
 src/amuse/community/fi/data/input/H.Hcool
 src/amuse/community/fi/data/input/H.cool
```

### Comparing `amuse-fi-2023.5.0/setup.py` & `amuse-fi-2024.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.fi.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/fi/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/fi/_version.py",
+}
 
 setup(
     name=name,
     use_scm_version=use_scm_version,
     setup_requires=setup_requires,
-    version=version,
     classifiers=classifiers,
     url=url,
     author_email=author_email,
     author=author,
     license=license_,
     description=description,
     long_description=long_description,
     long_description_content_type=long_description_content_type,
     install_requires=install_requires,
-    python_requires=">=3.5",
+    python_requires=">=3.7",
     cmdclass=mapping_from_command_name_to_command_class,
     ext_modules=extensions,
     package_dir={
         'amuse.community.fi': 'src/amuse/community/fi',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/Makefile` & `amuse-fi-2024.4.0/src/amuse/community/fi/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/README` & `amuse-fi-2024.4.0/src/amuse/community/fi/README`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/C.Hcool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/C.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/C.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/C.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Fe.Hcool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Fe.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Fe.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Fe.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.H2cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.H2cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.HH2cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.HH2cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/H2.Hcool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/H2.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/He.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/He.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/N.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/N.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Ne.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Ne.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/O.Hcool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/O.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/O.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/O.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Si.Hcool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Si.Hcool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/Si.cool` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/Si.cool`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_02_10.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_02_10.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_12_10_023.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_12_10_023.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_18_06_10.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_18_06_10.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/bct_2_10_0045.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/bct_2_10_0045.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_1.25.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_1.25.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_1.8.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_1.8.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burk_2.2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burk_2.2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burkct_4_20_02.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burkct_4_20_02.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/burkct_4_20_04.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/burkct_4_20_04.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_102_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_102_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_124_12.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_124_12.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_144_12.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_144_12.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_181_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_181_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_195_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_195_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_50_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_50_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_50_3.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_50_3.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_55_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_55_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/hk_96_2.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/hk_96_2.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_04_20_32.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_04_20_32.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_10_40_02` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_10_40_02`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_10_40_02.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_10_40_02.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2.6_40_0044.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2.6_40_0044.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_005.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_005.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_01.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_01.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_02.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_02.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_04.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_04.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_20_08.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_20_08.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_2_40_1.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_2_40_1.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_3_30_1.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_3_30_1.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_4_40_06.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_4_40_06.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_6_40_025.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_6_40_025.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_6_40_04.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_6_40_04.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_7_40_00088` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_7_40_00088`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/isoct_7_40_00088.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/isoct_7_40_00088.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_004_6.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_004_6.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_12_10_015.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_12_10_015.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfw_2_10_0036.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfw_2_10_0036.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/nfwct_2_20_149.halo` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/nfwct_2_20_149.halo`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_emp.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_emp.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_emp.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_emp.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0001.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z0004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z008.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z008.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z008.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z008.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z02.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z02.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z02.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z02.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z05.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z05.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z05.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z05.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z10.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z10.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_msca_z10.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_msca_z10.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_emp.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_emp.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_emp.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_emp.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0001.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z0004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z008.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z008.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z008.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z008.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z02.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z02.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z02.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z02.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z05.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z05.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z05.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z05.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z10.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z10.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_salp_z10.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_salp_z10.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_emp.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_emp.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_emp.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_emp.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0001.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z0004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z004.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z004.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z004.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z004.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z008.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z008.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z008.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z008.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z02.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z02.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z02.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z02.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z05.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z05.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z05.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z05.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z10.starmodel` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z10.starmodel`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/ssp_sca_z10.starprop` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/ssp_sca_z10.starprop`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/data/input/uvpol10_10` & `amuse-fi-2024.4.0/src/amuse/community/fi/data/input/uvpol10_10`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/interface.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/interface.py` & `amuse-fi-2024.4.0/src/amuse/community/fi/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         .. [#] ADS:2005PhDT........17P (Pelupessy, PhD thesis 2005, Leiden Observatory)
         .. [#] ADS:1997A&A...325..972G (Gerritsen & Icke, 1997, A&A 325, 972)
     """
     get_total_radius=None
     get_total_mass=None
     get_center_of_mass_position=None
     get_center_of_mass_velocity=None
-    set_acceleration=None
     get_acceleration=None
     
     use_modules=['StoppingConditions','AmuseInterface']
     
     MODE_NORMAL = 'normal'
     MODE_NORMAL_OPENMP = 'openmp'
     MODE_PERIODIC_BOUNDARIES = 'periodic'
```

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/map_interface.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/map_interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/patch_globals_dot_h.py` & `amuse-fi-2024.4.0/src/amuse/community/fi/patch_globals_dot_h.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/H2cool.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/H2cool.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/Makefile` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/blackhole.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/blackhole.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/buildnearlist.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/buildnearlist.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/buildtree.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/buildtree.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/clean.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/clean.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/combine_simple.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/combine_simple.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/coolcurve.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/coolcurve.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/cooling.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/cooling.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/density.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/density.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/diagnostics.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/diagnostics.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/elements.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/elements.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/entdot.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/entdot.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/ethstep.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/ethstep.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/extract.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/extract.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fcco.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fcco.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/feedback.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/feedback.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fftw3.f` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fftw3.f`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fi.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fi.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fi_viewer.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fi_viewer.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fixedhalo.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fixedhalo.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fthread.f` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fthread.f`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/fuvflux.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/fuvflux.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/glfi.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/glfi.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/globals_template.h` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/globals_template.h`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/gravity.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/gravity.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/gravsum.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/gravsum.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/hash.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/hash.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/heating.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/heating.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/heco.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/heco.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/hicube.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/hicube.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/init.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/init.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/io-old.f` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/io-old.f`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/io.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/io.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/io2.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/io2.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/ionize.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/ionize.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/makemap.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/makemap.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/makemapmod.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/makemapmod.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/map_helpers.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/map_helpers.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/mem.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/mem.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/molecules.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/molecules.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_helpers.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_helpers.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_interface.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_interface.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/muse_io2_stub.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/muse_io2_stub.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/pmgrav.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/pmgrav.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/ppread.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/ppread.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/project.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/project.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/pt.c` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/pt.c`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/pt.h` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/pt.h`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/ptf77.c` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/ptf77.c`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/random.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/random.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/readparam.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/readparam.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/rgabe.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/rgabe.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/rgabe2.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/rgabe2.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/rgadget.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/rgadget.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/rsimple.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/rsimple.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/search.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/search.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh2.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh2.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sfh3.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sfh3.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sfinfo.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sfinfo.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/snapreader.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/snapreader.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/snapviewer.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/snapviewer.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sort.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sort.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/sphray_io.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/sphray_io.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/starprop.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/starprop.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/stars3d.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/stars3d.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/stellar.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/stellar.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/stepsystem.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/stepsystem.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/tidalsum.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/tidalsum.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/timestep.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/timestep.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/togabe.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/togabe.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/togabe2.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/togabe2.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/tosimple.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/tosimple.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/tosimplex.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/tosimplex.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/treewalk.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/treewalk.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/update_tree.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/update_tree.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/util.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/util.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/src/amuse/community/fi/src/varia.f90` & `amuse-fi-2024.4.0/src/amuse/community/fi/src/varia.f90`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/__init__.py` & `amuse-fi-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/classifiers.py` & `amuse-fi-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/config.py` & `amuse-fi-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/generate_main.py` & `amuse-fi-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/getsp.class` & `amuse-fi-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/getsp.java` & `amuse-fi-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/misc.py` & `amuse-fi-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-fi-2023.5.0/support/setup_codes.py` & `amuse-fi-2024.4.0/support/setup_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,15 @@
 import configparser
 
 from subprocess import Popen, PIPE, STDOUT
 
 from glob import glob
 
 from distutils.dir_util import create_tree
-# from distutils import log
-import logging
+from distutils import log
 from distutils import spawn
 from distutils import file_util
 from distutils.errors import DistutilsError
 from distutils.command.clean import clean
 from setuptools.command.install import install
 from setuptools import Command
 from setuptools.command.build import build
@@ -556,37 +555,37 @@
         if not os.path.exists(lib_binbuilddir):
             self.mkpath(lib_binbuilddir)
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                         continue
 
-                # self.announce("will copy worker: {0}".format(name), level = logging.INFO)
+                # self.announce("will copy worker: {0}".format(name), level = log.INFO)
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_binbuilddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -599,19 +598,19 @@
             worker_code_re = re.compile(r'(([a-zA-Z0-9]+_)*)?worker(_[a-zA-Z0-9]+)?')
         worker_so_re = re.compile(r'(([a-zA-Z0-9]+_)*)?cython(_[a-zA-Z0-9]+)?.so')
 
         for srcdir in self.makefile_paths(self.codes_src_dir):
             reldir = os.path.relpath(srcdir, self.codes_src_dir)
             temp_builddir = os.path.join(self.codes_dir, reldir)
 
-            self.announce("will copy worker: {0}".format(srcdir), level=logging.INFO)
+            self.announce("will copy worker: {0}".format(srcdir), level=log.INFO)
             lib_builddir = os.path.join(self.build_lib, os.path.relpath(srcdir, os.path.join(self.amuse_src_dir, '..')))
 
             shortname = reldir.lower()
-            self.announce(shortname, level=logging.INFO)
+            self.announce(shortname, level=log.INFO)
 
             for name in os.listdir(temp_builddir):
                 path = os.path.join(temp_builddir, name)
                 stat = os.stat(path)
 
                 if os.path.isfile(path):
                     if worker_so_re.match(name):
@@ -620,15 +619,15 @@
                         continue
 
                 if os.path.isfile(path) and os.access(path, os.X_OK):
                     if worker_code_re.match(name):
                         topath = os.path.join(lib_builddir, name)
                         self.copy_file(path, topath)
                     elif not name.endswith('.py'):
-                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=logging.WARN)
+                        self.announce("will not copy executable: {0}, it does not match the worker pattern".format(name), level=log.WARN)
             
             # also copy file or dir named data
             path = os.path.join(temp_builddir, 'data')
             topath = os.path.join(lib_builddir, 'data')
             if os.path.isfile(path):
                 self.copy_file(path, topath)
             if os.path.isdir(path):
@@ -712,15 +711,15 @@
         result = list(set(result))
 
         return result
 
     def call(self, arguments, buildlogfile=None, **keyword_arguments):
         stringio = []
 
-        self.announce(' '.join(arguments), logging.DEBUG)
+        self.announce(' '.join(arguments), log.DEBUG)
 
         process = Popen(
             arguments,
             stdout=PIPE,
             stderr=STDOUT,
             **keyword_arguments
         )
@@ -728,24 +727,24 @@
         while True:
             line = process.stdout.readline()
             if len(line) == 0:
                 break
 
             if buildlogfile is not None:
                 buildlogfile.write(line)
-            self.announce(line[:-1].decode("utf-8"), logging.DEBUG)
+            self.announce(line[:-1].decode("utf-8"), log.DEBUG)
             stringio.append(str(line, 'utf-8'))
 
         result = process.wait()
         content = ''.join(stringio)
 
         if result != 0:
-            self.announce("error in call, tail output:\n", logging.INFO)
-            self.announce(''.join(stringio[-100:]), logging.INFO)
-            self.announce("-"*80, logging.INFO)
+            self.announce("error in call, tail output:\n", log.INFO)
+            self.announce(''.join(stringio[-100:]), log.INFO)
+            self.announce("-"*80, log.INFO)
 
         return result, content
 
     def build_environment(self):
         environment = self.environment.copy()
         environment.update(os.environ)
         path = os.path.join(environment["MUSE_PACKAGE_DIR"], "src")
@@ -880,16 +879,16 @@
         build = list()
         lib_build = list()
         lib_not_build = list()
         environment = self.build_environment()
 
         buildlog = 'build.log'
 
-        self.announce("building libraries and community codes", level=logging.INFO)
-        self.announce("build, for logging, see '{0}'".format(buildlog), level=logging.INFO)
+        self.announce("building libraries and community codes", level=log.INFO)
+        self.announce("build, for logging, see '{0}'".format(buildlog), level=log.INFO)
 
         with open(buildlog, "w") as output:
             output.write('*'*100)
             output.write('\n')
             output.write('Building libraries and codes\n')
             output.write('*'*100)
             output.write('\n')
@@ -898,28 +897,28 @@
             self.copy_build_prereq_to_build_dir()
             self.copy_lib_to_build_dir()
 
         for x in self.makefile_paths(self.lib_dir):
 
             shortname = x[len(self.lib_dir) + 1:] + '-library'
             starttime = datetime.datetime.now()
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
 
             endtime = datetime.datetime.now()
             if returncode == 2:
-                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=logging.DEBUG)
+                self.announce("[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime), level=log.DEBUG)
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(x[len(self.lib_dir) + 1:])
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(x[len(self.lib_dir) + 1:])
                 else:
                     lib_not_build.append(shortname)
             else:
-                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=logging.DEBUG)
+                self.announce("[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime), level=log.DEBUG)
                 lib_build.append(shortname)
 
         if not self.codes_dir == self.codes_src_dir:
             self.copy_codes_to_build_dir()
 
         # environment.update(self.environment)
         makefile_paths = list(self.makefile_paths(self.codes_dir))
@@ -933,24 +932,24 @@
             # to distribute mesa, it will make the
             # download size from about 100mb size
             # to > 1Gb size.
             #
             # Could we remove some of the data files from mesa?
             #
             if not self.inplace and shortname == 'mesa':
-                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=logging.INFO)
+                self.announce("[{1:%H:%M:%S}] skipping {0}".format(shortname, starttime), level=log.INFO)
                 continue
 
-            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=logging.INFO)
+            self.announce("[{1:%H:%M:%S}] building {0}".format(shortname, starttime), level=log.INFO)
             returncode, outputlog = self.run_make_on_directory(shortname, x, 'all', environment)
             endtime = datetime.datetime.now()
             if returncode > 0:
                 self.announce(
                     "[{2:%H:%M:%S}] building {0}, failed, see {1!r} for error log".format(shortname, buildlog, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 if self.is_download_needed(outputlog):
                     is_download_needed.append(shortname)
                 elif self.is_cuda_needed(outputlog):
                     is_cuda_needed.append(shortname)
                 elif self.are_python_imports_needed(outputlog):
                     are_python_imports_needed.append(shortname)
@@ -960,40 +959,40 @@
                 if self.is_mpi_enabled():
                     continue
             else:
                 build.append(shortname)
                 is_built = True
                 self.announce(
                     "[{1:%H:%M:%S}] building {0}, succeeded".format(shortname, endtime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
 
             if not self.variant:
                 continue
 
             special_targets = self.get_special_targets(shortname, x, environment)
             for target, target_name in special_targets:
                 starttime = datetime.datetime.now()
                 self.announce(
                     "[{2:%H:%M:%S}] building {0} - {1}".format(shortname, target_name, starttime),
-                    level=logging.DEBUG
+                    level=log.DEBUG
                 )
                 returncode, outputlog = self.run_make_on_directory(shortname, x, target, environment)
                 endtime = datetime.datetime.now()
                 if returncode > 0:
                     specials_list = not_build_special.setdefault(shortname,[])
                     specials_list.append(target_name)
                     self.announce(
                         "[{3:%H:%M:%S}] building {0} - {1}, failed, see {2!r} for error log".format(shortname, target_name, buildlog, endtime),
-                        level=logging.DEBUG
+                        level=log.DEBUG
                     )
                 else:
                     build_to_special_targets.setdefault(shortname, list()).append(target_name)
                     self.announce(
-                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=logging.DEBUG
+                        "[{2:%H:%M:%S}] building {0} - {1}, succeeded".format(shortname, target_name, endtime), level=log.DEBUG
                     )
 
         # if supportrc["framework_install"]:
         #     self.copy_config_to_build_dir()
 
         if not self.codes_dir == self.codes_src_dir:
             # self.copy_worker_codes_to_build_dir()
@@ -1028,17 +1027,17 @@
             not_build
             or not_build_special
             or is_download_needed
             or is_cuda_needed
             or are_python_imports_needed
         ):
             if not_build:
-                level = logging.WARN
+                level = log.WARN
             else:
-                level = logging.INFO
+                level = log.INFO
             if not_build:
                 self.announce(
                     "Community codes not built (because of errors/ missing libraries):",
                     level=level
                 )
                 self.announce("="*80,  level=level)
                 for x in not_build:
@@ -1061,26 +1060,26 @@
                     self.announce(
                         f' * {x} , make {x}.code DOWNLOAD_CODES=1', level=level
                     )
 
             self.announce("="*80,  level=level)
 
         if build:
-            level = logging.INFO
+            level = log.INFO
             self.announce("Community codes built",  level=level)
             self.announce("="*80,  level=level)
             for x in build:
                 if x in build_to_special_targets:
                     y = build_to_special_targets[x]
                     self.announce('* {0} ({1})'.format(x, ','.join(y)), level=level)
                 else:
                     self.announce('* {0}'.format(x),  level=level)
             self.announce("="*80,  level=level)
 
-        level = logging.INFO
+        level = log.INFO
         self.announce(
             "{0} out of {1} codes built, {2} out of {3} libraries built".format(
                 len(build), 
                 len(build) + len(not_build), 
                 len(lib_build), 
                 len(lib_build) + len(lib_not_build)
             ),
```

