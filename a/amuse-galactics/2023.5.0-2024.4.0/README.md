# Comparing `tmp/amuse-galactics-2023.5.0.tar.gz` & `tmp/amuse-galactics-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-galactics-2023.5.0.tar", last modified: Wed May 17 10:18:46 2023, max compression
+gzip compressed data, was "amuse-galactics-2024.4.0.tar", last modified: Wed Apr 24 16:32:18 2024, max compression
```

## Comparing `amuse-galactics-2023.5.0.tar` & `amuse-galactics-2024.4.0.tar`

### file list

```diff
@@ -1,244 +1,244 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.901186 amuse-galactics-2023.5.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-galactics-2023.5.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1195 2023-05-17 10:18:46.901010 amuse-galactics-2023.5.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       62 2022-11-22 11:55:14.000000 amuse-galactics-2023.5.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.864316 amuse-galactics-2023.5.0/amuse_galactics.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1195 2023-05-17 10:18:45.000000 amuse-galactics-2023.5.0/amuse_galactics.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    11247 2023-05-17 10:18:46.000000 amuse-galactics-2023.5.0/amuse_galactics.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-05-17 10:18:45.000000 amuse-galactics-2023.5.0/amuse_galactics.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-05-17 10:18:45.000000 amuse-galactics-2023.5.0/amuse_galactics.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-05-17 10:18:45.000000 amuse-galactics-2023.5.0/amuse_galactics.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-galactics-2023.5.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-05-17 10:18:46.901239 amuse-galactics-2023.5.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1798 2022-11-22 11:55:14.000000 amuse-galactics-2023.5.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.862062 amuse-galactics-2023.5.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.862117 amuse-galactics-2023.5.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.862167 amuse-galactics-2023.5.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.865769 amuse-galactics-2023.5.0/src/amuse/community/galactics/
--rw-r--r--   0 rieder     (501) staff       (20)     2204 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       50 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)    40300 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.862301 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.879679 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/
--rw-r--r--   0 rieder     (501) staff       (20)     4643 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     1393 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/alldens.f
--rw-r--r--   0 rieder     (501) staff       (20)     1808 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskdens.f
--rw-r--r--   0 rieder     (501) staff       (20)     1224 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskforce.f
--rw-r--r--   0 rieder     (501) staff       (20)     1136 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskpot.f
--rw-r--r--   0 rieder     (501) staff       (20)     2201 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bessj01.f
--rw-r--r--   0 rieder     (501) staff       (20)      347 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bulgedens.f
--rw-r--r--   0 rieder     (501) staff       (20)      693 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bulgedenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     5160 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bulgepotential.f
--rw-r--r--   0 rieder     (501) staff       (20)      867 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/contourden.f
--rw-r--r--   0 rieder     (501) staff       (20)    19567 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/dbh.f
--rw-r--r--   0 rieder     (501) staff       (20)     1209 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/dbhplot.f
--rw-r--r--   0 rieder     (501) staff       (20)      388 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/dens.f
--rw-r--r--   0 rieder     (501) staff       (20)     1172 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/densrpsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     4935 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdens.f
--rw-r--r--   0 rieder     (501) staff       (20)      144 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdensf.f
--rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     7722 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf.f
--rw-r--r--   0 rieder     (501) staff       (20)      795 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf3ez.f
--rw-r--r--   0 rieder     (501) staff       (20)      541 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf3intez.f
--rw-r--r--   0 rieder     (501) staff       (20)      392 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf5ez.f
--rw-r--r--   0 rieder     (501) staff       (20)      390 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf5intez.f
--rw-r--r--   0 rieder     (501) staff       (20)      826 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskinfo.f
--rw-r--r--   0 rieder     (501) staff       (20)      391 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/erfcc.f
--rw-r--r--   0 rieder     (501) staff       (20)      259 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/erfcen.f
--rw-r--r--   0 rieder     (501) staff       (20)      121 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/fixedbulgepot.f
--rw-r--r--   0 rieder     (501) staff       (20)     4449 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/fixedhalopot.f
--rw-r--r--   0 rieder     (501) staff       (20)     3949 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/flatdiskpot.cc
--rw-r--r--   0 rieder     (501) staff       (20)      308 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/fnamidden.f
--rw-r--r--   0 rieder     (501) staff       (20)     4656 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/force.f
--rw-r--r--   0 rieder     (501) staff       (20)     2355 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gasdisk3.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6252 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/genbulge.c
--rw-r--r--   0 rieder     (501) staff       (20)    10959 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gendisk.c
--rw-r--r--   0 rieder     (501) staff       (20)     1599 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gengas.c
--rw-r--r--   0 rieder     (501) staff       (20)     6873 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/genhalo.c
--rw-r--r--   0 rieder     (501) staff       (20)     7110 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/getfreqs.f
--rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/golden.c
--rw-r--r--   0 rieder     (501) staff       (20)      361 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/halodens.f
--rw-r--r--   0 rieder     (501) staff       (20)      808 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/haloinfo.f
--rw-r--r--   0 rieder     (501) staff       (20)     5219 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/halopotential.f
--rw-r--r--   0 rieder     (501) staff       (20)      919 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/main.h
--rw-r--r--   0 rieder     (501) staff       (20)      400 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/modstamp.f
--rw-r--r--   0 rieder     (501) staff       (20)     3005 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/newfreqs.f
--rw-r--r--   0 rieder     (501) staff       (20)     2929 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/omekap.f
--rw-r--r--   0 rieder     (501) staff       (20)     4642 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/pgstub.f
--rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/plgndr1.f
--rw-r--r--   0 rieder     (501) staff       (20)     3849 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/plotforce.f
--rw-r--r--   0 rieder     (501) staff       (20)     1849 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/plothalo.f
--rw-r--r--   0 rieder     (501) staff       (20)      362 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/polarbulgedens.f
--rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/polardens.f
--rw-r--r--   0 rieder     (501) staff       (20)      338 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/polarhalodens.f
--rw-r--r--   0 rieder     (501) staff       (20)     2685 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/pot.f
--rw-r--r--   0 rieder     (501) staff       (20)    12595 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/prng_engine.hpp
--rw-r--r--   0 rieder     (501) staff       (20)     1394 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/prng_engine_wrapper.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2286 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/query.c
--rw-r--r--   0 rieder     (501) staff       (20)      856 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/ran1.c
--rw-r--r--   0 rieder     (501) staff       (20)     1347 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/rcirc.f
--rw-r--r--   0 rieder     (501) staff       (20)     2110 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/readdiskdf.f
--rw-r--r--   0 rieder     (501) staff       (20)     4102 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/readharmfile.f
--rw-r--r--   0 rieder     (501) staff       (20)      467 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/readmassrad.c
--rw-r--r--   0 rieder     (501) staff       (20)      189 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sigr2.f
--rw-r--r--   0 rieder     (501) staff       (20)      936 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sigz2.f
--rw-r--r--   0 rieder     (501) staff       (20)      410 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/simpson.c
--rw-r--r--   0 rieder     (501) staff       (20)     6992 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_burkert.f90
--rw-r--r--   0 rieder     (501) staff       (20)     9411 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_einasto.f90
--rw-r--r--   0 rieder     (501) staff       (20)     6973 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_hernquist.f90
--rw-r--r--   0 rieder     (501) staff       (20)     7702 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_nfw.f90
--rw-r--r--   0 rieder     (501) staff       (20)      924 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/splined.f
--rw-r--r--   0 rieder     (501) staff       (20)      808 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/splintd.f
--rw-r--r--   0 rieder     (501) staff       (20)      991 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/testgas.f90
--rw-r--r--   0 rieder     (501) staff       (20)    16013 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/thickdisk2.f90
--rw-r--r--   0 rieder     (501) staff       (20)      638 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/toascii.c
--rw-r--r--   0 rieder     (501) staff       (20)      744 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/totdens.f
--rw-r--r--   0 rieder     (501) staff       (20)     1446 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/vcirc.c
--rw-r--r--   0 rieder     (501) staff       (20)    41672 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/interface.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.879837 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/
--rw-r--r--   0 rieder     (501) staff       (20)      238 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/README.install
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.879988 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.881018 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.bulge
--rw-r--r--   0 rieder     (501) staff       (20)      143 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.dbh
--rw-r--r--   0 rieder     (501) staff       (20)      132 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.disk
--rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.diskdf
--rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.gendenspsi
--rw-r--r--   0 rieder     (501) staff       (20)       28 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/in.halo
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.882359 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.bulge
--rw-r--r--   0 rieder     (501) staff       (20)      142 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.dbh
--rw-r--r--   0 rieder     (501) staff       (20)      132 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.disk
--rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.diskdf
--rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.gendenspsi
--rw-r--r--   0 rieder     (501) staff       (20)       28 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/in.halo
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.883575 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      452 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/ics.job
--rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.bulge
--rw-r--r--   0 rieder     (501) staff       (20)      144 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.dbh
--rw-r--r--   0 rieder     (501) staff       (20)      131 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.disk
--rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.diskdf
--rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.gendenspsi
--rw-r--r--   0 rieder     (501) staff       (20)       27 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/in.halo
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.884551 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       17 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.bulge
--rw-r--r--   0 rieder     (501) staff       (20)       48 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.dbh
--rw-r--r--   0 rieder     (501) staff       (20)      133 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.disk
--rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.diskdf
--rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.gendenspsi
--rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/in.halo
--rw-r--r--   0 rieder     (501) staff       (20)     2689 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/README.parameters
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.885341 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/
--rw-r--r--   0 rieder     (501) staff       (20)        6 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/.smhist
--rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       17 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/in.bulge
--rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/in.dbh
--rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/in.gendenspsi
--rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/in.halo
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.888209 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/
--rw-r--r--   0 rieder     (501) staff       (20)     1107 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)      445 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/README.install
--rw-r--r--   0 rieder     (501) staff       (20)      900 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/appdiskforce.f
--rw-r--r--   0 rieder     (501) staff       (20)      825 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/appdiskpot.f
--rw-r--r--   0 rieder     (501) staff       (20)      811 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/checkvirial.c
--rw-r--r--   0 rieder     (501) staff       (20)      173 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/common.h
--rw-r--r--   0 rieder     (501) staff       (20)     1421 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/commonblocks.h
--rw-r--r--   0 rieder     (501) staff       (20)     1490 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/energysort.c
--rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/equivalence.h
--rw-r--r--   0 rieder     (501) staff       (20)      215 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/extern.h
--rw-r--r--   0 rieder     (501) staff       (20)     2523 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/force.f
--rw-r--r--   0 rieder     (501) staff       (20)       62 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/parameters.h
--rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/plgndr1.f
--rw-r--r--   0 rieder     (501) staff       (20)     2786 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/readharmfile.f
--rw-r--r--   0 rieder     (501) staff       (20)      427 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/rigidpot.c
--rw-r--r--   0 rieder     (501) staff       (20)      691 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/testforce.c
--rw-r--r--   0 rieder     (501) staff       (20)      914 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/testp.c
--rw-r--r--   0 rieder     (501) staff       (20)     1072 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/vcirc.c
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.899069 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/
--rw-r--r--   0 rieder     (501) staff       (20)     7015 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     1520 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskdens.f
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskforce.f
--rw-r--r--   0 rieder     (501) staff       (20)      823 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskpot.f
--rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/bulgedenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     4705 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/bulgepotential.f
--rw-r--r--   0 rieder     (501) staff       (20)     1501 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/commonblocks
--rw-r--r--   0 rieder     (501) staff       (20)    14897 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dbh.f
--rw-r--r--   0 rieder     (501) staff       (20)      261 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dens.f
--rw-r--r--   0 rieder     (501) staff       (20)      546 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfbulge.f
--rw-r--r--   0 rieder     (501) staff       (20)     1176 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfcorrection.f
--rw-r--r--   0 rieder     (501) staff       (20)      529 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfhalo.f
--rw-r--r--   0 rieder     (501) staff       (20)     1385 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdens.f
--rw-r--r--   0 rieder     (501) staff       (20)      128 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdensf.f
--rw-r--r--   0 rieder     (501) staff       (20)      747 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     5154 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf.f
--rw-r--r--   0 rieder     (501) staff       (20)      536 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf3ez.f
--rw-r--r--   0 rieder     (501) staff       (20)      559 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf3intez.f
--rw-r--r--   0 rieder     (501) staff       (20)      341 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf5ez.f
--rw-r--r--   0 rieder     (501) staff       (20)      411 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf5intez.f
--rw-r--r--   0 rieder     (501) staff       (20)     2697 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskpotentialestimate.f
--rw-r--r--   0 rieder     (501) staff       (20)     2206 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dpolardens.f
--rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/equivalence
--rw-r--r--   0 rieder     (501) staff       (20)      257 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/erfcen.f
--rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/errmsg.dat
--rw-r--r--   0 rieder     (501) staff       (20)      308 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/fnamidden.f
--rw-r--r--   0 rieder     (501) staff       (20)     2490 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/force.f
--rw-r--r--   0 rieder     (501) staff       (20)     4906 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/genbulge.c
--rw-r--r--   0 rieder     (501) staff       (20)     1481 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendenspsibulge.f
--rw-r--r--   0 rieder     (501) staff       (20)     1623 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendenspsihalo.f
--rw-r--r--   0 rieder     (501) staff       (20)     4444 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendf.f
--rw-r--r--   0 rieder     (501) staff       (20)     7966 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendisk.c
--rw-r--r--   0 rieder     (501) staff       (20)     4699 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/genhalo.c
--rw-r--r--   0 rieder     (501) staff       (20)     6557 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/getfreqs.f
--rw-r--r--   0 rieder     (501) staff       (20)     1363 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/getpsi.f
--rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/golden.c
--rw-r--r--   0 rieder     (501) staff       (20)      127 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halodens.f
--rw-r--r--   0 rieder     (501) staff       (20)      569 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halodenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     4810 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halopotential.f
--rw-r--r--   0 rieder     (501) staff       (20)     1804 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halopotentialestimate.f
--rw-r--r--   0 rieder     (501) staff       (20)     1145 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/main.h
--rw-r--r--   0 rieder     (501) staff       (20)     6127 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/make.log
--rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/modstamp.f
--rw-r--r--   0 rieder     (501) staff       (20)      668 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/nfwprofiles.f
--rw-r--r--   0 rieder     (501) staff       (20)     2819 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/omekap.f
--rw-r--r--   0 rieder     (501) staff       (20)       66 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/parameters
--rw-r--r--   0 rieder     (501) staff       (20)     6452 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgenbulge.c
--rw-r--r--   0 rieder     (501) staff       (20)     9270 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgendisk.c
--rw-r--r--   0 rieder     (501) staff       (20)     6253 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgenhalo.c
--rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/plgndr1.f
--rw-r--r--   0 rieder     (501) staff       (20)      370 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/polarbulgedens.f
--rw-r--r--   0 rieder     (501) staff       (20)      373 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/polardens.f
--rw-r--r--   0 rieder     (501) staff       (20)      337 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/polarhalodens.f
--rw-r--r--   0 rieder     (501) staff       (20)     1576 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pot.f
--rw-r--r--   0 rieder     (501) staff       (20)    12595 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/prng_engine.hpp
--rw-r--r--   0 rieder     (501) staff       (20)     1394 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/prng_engine_wrapper.cpp
--rw-r--r--   0 rieder     (501) staff       (20)     2024 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/query.c
--rw-r--r--   0 rieder     (501) staff       (20)      856 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/ran1.c
--rw-r--r--   0 rieder     (501) staff       (20)     1084 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/rcirc.f
--rw-r--r--   0 rieder     (501) staff       (20)      756 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readdenspsi.f
--rw-r--r--   0 rieder     (501) staff       (20)     1819 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readdiskdf.f
--rw-r--r--   0 rieder     (501) staff       (20)     2615 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readharmfile.f
--rw-r--r--   0 rieder     (501) staff       (20)      467 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readmassrad.c
--rw-r--r--   0 rieder     (501) staff       (20)     9658 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/sersicprofiles.f
--rw-r--r--   0 rieder     (501) staff       (20)      135 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/sigr2.f
--rw-r--r--   0 rieder     (501) staff       (20)      302 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/sigz2.f
--rw-r--r--   0 rieder     (501) staff       (20)      410 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/simpson.c
--rw-r--r--   0 rieder     (501) staff       (20)      960 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/splined.f
--rw-r--r--   0 rieder     (501) staff       (20)      806 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/splintd.f
--rw-r--r--   0 rieder     (501) staff       (20)      638 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/toascii.c
--rw-r--r--   0 rieder     (501) staff       (20)      426 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/totdens.f
--rw-r--r--   0 rieder     (501) staff       (20)      436 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/velocityfactors.f
--rw-r--r--   0 rieder     (501) staff       (20)      148 2023-05-17 10:18:45.000000 amuse-galactics-2023.5.0/src/amuse/community/galactics/version.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-05-17 10:18:46.900714 amuse-galactics-2023.5.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-galactics-2023.5.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49373 2023-05-17 08:15:41.000000 amuse-galactics-2023.5.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-galactics-2023.5.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.943353 amuse-galactics-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2022-11-22 11:55:14.000000 amuse-galactics-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1226 2024-04-24 16:32:18.943090 amuse-galactics-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       62 2022-11-22 11:55:14.000000 amuse-galactics-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.942686 amuse-galactics-2024.4.0/amuse_galactics.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1226 2024-04-24 16:32:17.000000 amuse-galactics-2024.4.0/amuse_galactics.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    11248 2024-04-24 16:32:18.000000 amuse-galactics-2024.4.0/amuse_galactics.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:17.000000 amuse-galactics-2024.4.0/amuse_galactics.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:17.000000 amuse-galactics-2024.4.0/amuse_galactics.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:17.000000 amuse-galactics-2024.4.0/amuse_galactics.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2023-05-17 10:16:28.000000 amuse-galactics-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:18.943420 amuse-galactics-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1599 2024-04-24 15:35:29.000000 amuse-galactics-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.905141 amuse-galactics-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.905196 amuse-galactics-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.905248 amuse-galactics-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.908670 amuse-galactics-2024.4.0/src/amuse/community/galactics/
+-rw-r--r--   0 rieder     (501) staff       (20)     2204 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       50 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:17.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)    40300 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.905376 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.921186 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     4643 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     1393 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/alldens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1808 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1224 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskforce.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1136 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskpot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2201 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bessj01.f
+-rw-r--r--   0 rieder     (501) staff       (20)      347 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bulgedens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      693 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bulgedenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5160 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bulgepotential.f
+-rw-r--r--   0 rieder     (501) staff       (20)      867 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/contourden.f
+-rw-r--r--   0 rieder     (501) staff       (20)    19567 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/dbh.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1209 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/dbhplot.f
+-rw-r--r--   0 rieder     (501) staff       (20)      388 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/dens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1172 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/densrpsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4935 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      144 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdensf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1007 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7722 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf.f
+-rw-r--r--   0 rieder     (501) staff       (20)      795 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf3ez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      541 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf3intez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      392 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf5ez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      390 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf5intez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      826 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskinfo.f
+-rw-r--r--   0 rieder     (501) staff       (20)      391 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/erfcc.f
+-rw-r--r--   0 rieder     (501) staff       (20)      259 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/erfcen.f
+-rw-r--r--   0 rieder     (501) staff       (20)      121 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/fixedbulgepot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4449 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/fixedhalopot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3949 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/flatdiskpot.cc
+-rw-r--r--   0 rieder     (501) staff       (20)      308 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/fnamidden.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4656 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/force.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2355 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gasdisk3.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6252 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/genbulge.c
+-rw-r--r--   0 rieder     (501) staff       (20)    10959 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gendisk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1599 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gengas.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6873 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/genhalo.c
+-rw-r--r--   0 rieder     (501) staff       (20)     7110 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/getfreqs.f
+-rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/golden.c
+-rw-r--r--   0 rieder     (501) staff       (20)      361 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/halodens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      808 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/haloinfo.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5219 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/halopotential.f
+-rw-r--r--   0 rieder     (501) staff       (20)      919 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/main.h
+-rw-r--r--   0 rieder     (501) staff       (20)      400 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/modstamp.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3005 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/newfreqs.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2929 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/omekap.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4642 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/pgstub.f
+-rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/plgndr1.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3849 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/plotforce.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1849 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/plothalo.f
+-rw-r--r--   0 rieder     (501) staff       (20)      362 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/polarbulgedens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/polardens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      338 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/polarhalodens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2685 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/pot.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12595 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/prng_engine.hpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1394 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/prng_engine_wrapper.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2286 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/query.c
+-rw-r--r--   0 rieder     (501) staff       (20)      856 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/ran1.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1347 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/rcirc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2110 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/readdiskdf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4102 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/readharmfile.f
+-rw-r--r--   0 rieder     (501) staff       (20)      467 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/readmassrad.c
+-rw-r--r--   0 rieder     (501) staff       (20)      189 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sigr2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      936 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sigz2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      410 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/simpson.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6992 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_burkert.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     9411 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_einasto.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     6973 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_hernquist.f90
+-rw-r--r--   0 rieder     (501) staff       (20)     7702 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_nfw.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      924 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/splined.f
+-rw-r--r--   0 rieder     (501) staff       (20)      808 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/splintd.f
+-rw-r--r--   0 rieder     (501) staff       (20)      991 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/testgas.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    16013 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/thickdisk2.f90
+-rw-r--r--   0 rieder     (501) staff       (20)      638 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/toascii.c
+-rw-r--r--   0 rieder     (501) staff       (20)      744 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/totdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1446 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/vcirc.c
+-rw-r--r--   0 rieder     (501) staff       (20)    41672 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/interface.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.921336 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/
+-rw-r--r--   0 rieder     (501) staff       (20)      238 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/README.install
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.921492 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.922624 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.bulge
+-rw-r--r--   0 rieder     (501) staff       (20)      143 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.dbh
+-rw-r--r--   0 rieder     (501) staff       (20)      132 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.disk
+-rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.diskdf
+-rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.gendenspsi
+-rw-r--r--   0 rieder     (501) staff       (20)       28 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/in.halo
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.923790 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.bulge
+-rw-r--r--   0 rieder     (501) staff       (20)      142 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.dbh
+-rw-r--r--   0 rieder     (501) staff       (20)      132 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.disk
+-rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.diskdf
+-rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.gendenspsi
+-rw-r--r--   0 rieder     (501) staff       (20)       28 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/in.halo
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.924998 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      452 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/ics.job
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.bulge
+-rw-r--r--   0 rieder     (501) staff       (20)      144 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.dbh
+-rw-r--r--   0 rieder     (501) staff       (20)      131 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.disk
+-rw-r--r--   0 rieder     (501) staff       (20)       31 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.diskdf
+-rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.gendenspsi
+-rw-r--r--   0 rieder     (501) staff       (20)       27 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/in.halo
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.926052 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       17 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.bulge
+-rw-r--r--   0 rieder     (501) staff       (20)       48 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.dbh
+-rw-r--r--   0 rieder     (501) staff       (20)      133 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.disk
+-rw-r--r--   0 rieder     (501) staff       (20)       32 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.diskdf
+-rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.gendenspsi
+-rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/in.halo
+-rw-r--r--   0 rieder     (501) staff       (20)     2689 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/README.parameters
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.926955 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/.smhist
+-rw-r--r--   0 rieder     (501) staff       (20)     1015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       17 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/in.bulge
+-rw-r--r--   0 rieder     (501) staff       (20)       56 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/in.dbh
+-rw-r--r--   0 rieder     (501) staff       (20)        8 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/in.gendenspsi
+-rw-r--r--   0 rieder     (501) staff       (20)       29 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/in.halo
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.929515 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/
+-rw-r--r--   0 rieder     (501) staff       (20)     1107 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)      445 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/README.install
+-rw-r--r--   0 rieder     (501) staff       (20)      900 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/appdiskforce.f
+-rw-r--r--   0 rieder     (501) staff       (20)      825 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/appdiskpot.f
+-rw-r--r--   0 rieder     (501) staff       (20)      811 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/checkvirial.c
+-rw-r--r--   0 rieder     (501) staff       (20)      173 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/common.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1421 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/commonblocks.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1490 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/energysort.c
+-rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/equivalence.h
+-rw-r--r--   0 rieder     (501) staff       (20)      215 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/extern.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2523 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/force.f
+-rw-r--r--   0 rieder     (501) staff       (20)       62 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/parameters.h
+-rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/plgndr1.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2786 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/readharmfile.f
+-rw-r--r--   0 rieder     (501) staff       (20)      427 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/rigidpot.c
+-rw-r--r--   0 rieder     (501) staff       (20)      691 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/testforce.c
+-rw-r--r--   0 rieder     (501) staff       (20)      914 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/testp.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1072 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/vcirc.c
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.940956 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/
+-rw-r--r--   0 rieder     (501) staff       (20)     7015 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     1520 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskforce.f
+-rw-r--r--   0 rieder     (501) staff       (20)      823 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskpot.f
+-rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/bulgedenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4705 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/bulgepotential.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1501 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/commonblocks
+-rw-r--r--   0 rieder     (501) staff       (20)    14897 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dbh.f
+-rw-r--r--   0 rieder     (501) staff       (20)      261 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      546 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfbulge.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1176 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfcorrection.f
+-rw-r--r--   0 rieder     (501) staff       (20)      529 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfhalo.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1385 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      128 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdensf.f
+-rw-r--r--   0 rieder     (501) staff       (20)      747 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5154 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf.f
+-rw-r--r--   0 rieder     (501) staff       (20)      536 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf3ez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      559 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf3intez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      341 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf5ez.f
+-rw-r--r--   0 rieder     (501) staff       (20)      411 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf5intez.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2697 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskpotentialestimate.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2206 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dpolardens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      263 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/equivalence
+-rw-r--r--   0 rieder     (501) staff       (20)      257 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/erfcen.f
+-rw-r--r--   0 rieder     (501) staff       (20)        0 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/errmsg.dat
+-rw-r--r--   0 rieder     (501) staff       (20)      308 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/fnamidden.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2490 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/force.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4906 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/genbulge.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1481 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendenspsibulge.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1623 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendenspsihalo.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4444 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7966 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendisk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     4699 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/genhalo.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6557 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/getfreqs.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1363 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/getpsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)      687 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/golden.c
+-rw-r--r--   0 rieder     (501) staff       (20)      127 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halodens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      569 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halodenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4810 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halopotential.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1804 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halopotentialestimate.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1145 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/main.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6127 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/make.log
+-rw-r--r--   0 rieder     (501) staff       (20)      421 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/modstamp.f
+-rw-r--r--   0 rieder     (501) staff       (20)      668 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/nfwprofiles.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2819 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/omekap.f
+-rw-r--r--   0 rieder     (501) staff       (20)       66 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/parameters
+-rw-r--r--   0 rieder     (501) staff       (20)     6452 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgenbulge.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9270 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgendisk.c
+-rw-r--r--   0 rieder     (501) staff       (20)     6253 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgenhalo.c
+-rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/plgndr1.f
+-rw-r--r--   0 rieder     (501) staff       (20)      370 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/polarbulgedens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      373 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/polardens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      337 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/polarhalodens.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1576 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pot.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12595 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/prng_engine.hpp
+-rw-r--r--   0 rieder     (501) staff       (20)     1394 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/prng_engine_wrapper.cpp
+-rw-r--r--   0 rieder     (501) staff       (20)     2024 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/query.c
+-rw-r--r--   0 rieder     (501) staff       (20)      856 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/ran1.c
+-rw-r--r--   0 rieder     (501) staff       (20)     1084 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/rcirc.f
+-rw-r--r--   0 rieder     (501) staff       (20)      756 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readdenspsi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1819 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readdiskdf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2615 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readharmfile.f
+-rw-r--r--   0 rieder     (501) staff       (20)      467 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readmassrad.c
+-rw-r--r--   0 rieder     (501) staff       (20)     9658 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/sersicprofiles.f
+-rw-r--r--   0 rieder     (501) staff       (20)      135 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/sigr2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      302 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/sigz2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      410 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/simpson.c
+-rw-r--r--   0 rieder     (501) staff       (20)      960 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/splined.f
+-rw-r--r--   0 rieder     (501) staff       (20)      806 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/splintd.f
+-rw-r--r--   0 rieder     (501) staff       (20)      638 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/toascii.c
+-rw-r--r--   0 rieder     (501) staff       (20)      426 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/totdens.f
+-rw-r--r--   0 rieder     (501) staff       (20)      436 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/velocityfactors.f
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:18.942456 amuse-galactics-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-galactics-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-galactics-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-galactics-2024.4.0/support/version.py
```

### Comparing `amuse-galactics-2023.5.0/PKG-INFO` & `amuse-galactics-2024.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-galactics
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Galactics
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
 
 This package installs the Galactics community code for AMUSE.
```

### Comparing `amuse-galactics-2023.5.0/amuse_galactics.egg-info/PKG-INFO` & `amuse-galactics-2024.4.0/amuse_galactics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-galactics
-Version: 2023.5.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Galactics
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
 
 This package installs the Galactics community code for AMUSE.
```

### Comparing `amuse-galactics-2023.5.0/amuse_galactics.egg-info/SOURCES.txt` & `amuse-galactics-2024.4.0/amuse_galactics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 amuse_galactics.egg-info/PKG-INFO
 amuse_galactics.egg-info/SOURCES.txt
 amuse_galactics.egg-info/dependency_links.txt
 amuse_galactics.egg-info/requires.txt
 amuse_galactics.egg-info/top_level.txt
 src/amuse/community/galactics/Makefile
 src/amuse/community/galactics/__init__.py
+src/amuse/community/galactics/_version.py
 src/amuse/community/galactics/gas_interface.py
 src/amuse/community/galactics/interface.py
-src/amuse/community/galactics/version.py
 src/amuse/community/galactics/gas_src/src/Makefile
 src/amuse/community/galactics/gas_src/src/alldens.f
 src/amuse/community/galactics/gas_src/src/appdiskdens.f
 src/amuse/community/galactics/gas_src/src/appdiskforce.f
 src/amuse/community/galactics/gas_src/src/appdiskpot.f
 src/amuse/community/galactics/gas_src/src/bessj01.f
 src/amuse/community/galactics/gas_src/src/bulgedens.f
```

### Comparing `amuse-galactics-2023.5.0/setup.py` & `amuse-galactics-2024.4.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,42 +29,35 @@
 ]
 
 package_data = {
 }
 
 mapping_from_command_name_to_command_class = setup_commands()
 
-try:
-    from src.amuse.community.galactics.version import version
-    use_scm_version = False
-    setup_requires = []
-except ImportError:
-    version = False
-    setup_requires = ['setuptools_scm']
-    use_scm_version = {
-        "root": "../..",
-        "relative_to": __file__,
-        "write_to": "src/amuse/community/galactics/version.py",
-    }
+setup_requires = ['setuptools_scm']
+use_scm_version = {
+    "root": "../..",
+    "relative_to": __file__,
+    "version_file": "src/amuse/community/galactics/_version.py",
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
         'amuse.community.galactics': 'src/amuse/community/galactics',
     },
     packages=packages,
     package_data=package_data,
```

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_interface.py` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_interface.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/alldens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/alldens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskdens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskdens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskforce.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskforce.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/appdiskpot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/appdiskpot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bessj01.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bessj01.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bulgedenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bulgedenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/bulgepotential.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/bulgepotential.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/contourden.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/contourden.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/dbh.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/dbh.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/dbhplot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/dbhplot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/densrpsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/densrpsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf3ez.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf3ez.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskdf3intez.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskdf3intez.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/diskinfo.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/diskinfo.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/fixedhalopot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/fixedhalopot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/flatdiskpot.cc` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/flatdiskpot.cc`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/force.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/force.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gasdisk3.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gasdisk3.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/genbulge.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/genbulge.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gendisk.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gendisk.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/gengas.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/gengas.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/genhalo.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/genhalo.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/getfreqs.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/getfreqs.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/golden.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/golden.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/haloinfo.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/haloinfo.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/halopotential.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/halopotential.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/main.h` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/main.h`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/newfreqs.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/newfreqs.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/omekap.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/omekap.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/pgstub.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/pgstub.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/plotforce.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/plotforce.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/plothalo.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/plothalo.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/pot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/pot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/prng_engine.hpp` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/prng_engine.hpp`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/prng_engine_wrapper.cpp` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/prng_engine_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/query.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/query.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/ran1.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/ran1.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/rcirc.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/rcirc.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/readdiskdf.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/readdiskdf.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/readharmfile.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/readharmfile.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sigz2.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sigz2.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_burkert.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_burkert.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_einasto.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_einasto.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_hernquist.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_hernquist.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/sphericaldf_nfw.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/sphericaldf_nfw.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/splined.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/splined.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/splintd.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/splintd.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/testgas.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/testgas.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/thickdisk2.f90` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/thickdisk2.f90`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/toascii.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/toascii.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/totdens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/totdens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/gas_src/src/vcirc.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/gas_src/src/vcirc.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/interface.py` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31a/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31a/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31b/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31b/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/M31c/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/M31c/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/NFW/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/NFW/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/README.parameters` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/README.parameters`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/models/Sersic/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/models/Sersic/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/appdiskforce.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/appdiskforce.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/appdiskpot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/appdiskpot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/checkvirial.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/checkvirial.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/commonblocks.h` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/commonblocks.h`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/energysort.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/energysort.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/force.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/force.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/readharmfile.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/readharmfile.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/testforce.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/testforce.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/testp.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/testp.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/potsrc/vcirc.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/potsrc/vcirc.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/Makefile` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskdens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskdens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskforce.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskforce.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/appdiskpot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/appdiskpot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/bulgedenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/bulgedenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/bulgepotential.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/bulgepotential.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/commonblocks` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/commonblocks`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dbh.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dbh.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfbulge.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfbulge.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfcorrection.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfcorrection.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dfhalo.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dfhalo.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf3ez.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf3ez.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskdf3intez.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskdf3intez.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/diskpotentialestimate.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/diskpotentialestimate.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/dpolardens.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/dpolardens.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/force.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/force.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/genbulge.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/genbulge.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendenspsibulge.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendenspsibulge.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendenspsihalo.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendenspsihalo.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendf.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendf.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/gendisk.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/gendisk.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/genhalo.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/genhalo.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/getfreqs.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/getfreqs.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/getpsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/getpsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/golden.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/golden.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halodenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halodenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halopotential.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halopotential.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/halopotentialestimate.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/halopotentialestimate.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/main.h` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/main.h`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/make.log` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/make.log`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/nfwprofiles.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/nfwprofiles.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/omekap.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/omekap.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgenbulge.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgenbulge.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgendisk.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgendisk.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pgenhalo.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pgenhalo.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/pot.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/pot.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/prng_engine.hpp` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/prng_engine.hpp`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/prng_engine_wrapper.cpp` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/prng_engine_wrapper.cpp`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/query.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/query.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/ran1.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/ran1.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/rcirc.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/rcirc.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readdenspsi.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readdenspsi.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readdiskdf.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readdiskdf.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/readharmfile.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/readharmfile.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/sersicprofiles.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/sersicprofiles.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/splined.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/splined.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/splintd.f` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/splintd.f`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/src/amuse/community/galactics/src/src/toascii.c` & `amuse-galactics-2024.4.0/src/amuse/community/galactics/src/src/toascii.c`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/__init__.py` & `amuse-galactics-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/classifiers.py` & `amuse-galactics-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/config.py` & `amuse-galactics-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/generate_main.py` & `amuse-galactics-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/getsp.class` & `amuse-galactics-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/getsp.java` & `amuse-galactics-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/misc.py` & `amuse-galactics-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-galactics-2023.5.0/support/setup_codes.py` & `amuse-galactics-2024.4.0/support/setup_codes.py`

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

