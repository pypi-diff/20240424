# Comparing `tmp/amuse-nbody6xx-2023.11.0.tar.gz` & `tmp/amuse-nbody6xx-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amuse-nbody6xx-2023.11.0.tar", last modified: Mon Nov 20 12:42:32 2023, max compression
+gzip compressed data, was "amuse-nbody6xx-2024.4.0.tar", last modified: Wed Apr 24 16:32:40 2024, max compression
```

## Comparing `amuse-nbody6xx-2023.11.0.tar` & `amuse-nbody6xx-2024.4.0.tar`

### file list

```diff
@@ -1,370 +1,370 @@
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.518673 amuse-nbody6xx-2023.11.0/
--rw-r--r--   0 rieder     (501) staff       (20)      216 2023-10-02 12:45:11.000000 amuse-nbody6xx-2023.11.0/MANIFEST.in
--rw-r--r--   0 rieder     (501) staff       (20)     1224 2023-11-20 12:42:32.518461 amuse-nbody6xx-2023.11.0/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)       61 2023-10-02 12:46:25.000000 amuse-nbody6xx-2023.11.0/README.md
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.437456 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/
--rw-r--r--   0 rieder     (501) staff       (20)     1224 2023-11-20 12:42:31.000000 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/PKG-INFO
--rw-r--r--   0 rieder     (501) staff       (20)    14722 2023-11-20 12:42:32.000000 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/SOURCES.txt
--rw-r--r--   0 rieder     (501) staff       (20)        1 2023-11-20 12:42:31.000000 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/dependency_links.txt
--rw-r--r--   0 rieder     (501) staff       (20)       16 2023-11-20 12:42:31.000000 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/requires.txt
--rw-r--r--   0 rieder     (501) staff       (20)        6 2023-11-20 12:42:31.000000 amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/top_level.txt
--rw-r--r--   0 rieder     (501) staff       (20)       93 2023-10-02 12:45:11.000000 amuse-nbody6xx-2023.11.0/pyproject.toml
--rw-r--r--   0 rieder     (501) staff       (20)       38 2023-11-20 12:42:32.518724 amuse-nbody6xx-2023.11.0/setup.cfg
--rw-r--r--   0 rieder     (501) staff       (20)     1593 2023-10-05 08:15:06.000000 amuse-nbody6xx-2023.11.0/setup.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.435624 amuse-nbody6xx-2023.11.0/src/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.435669 amuse-nbody6xx-2023.11.0/src/amuse/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.435713 amuse-nbody6xx-2023.11.0/src/amuse/community/
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.440157 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/
--rw-r--r--   0 rieder     (501) staff       (20)     1165 2022-11-30 13:58:15.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)       49 2022-10-03 08:52:42.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      419 2023-11-20 12:42:31.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/_version.py
--rw-r--r--   0 rieder     (501) staff       (20)     4417 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/common6.h
--rw-r--r--   0 rieder     (501) staff       (20)      622 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/debug.py
--rw-r--r--   0 rieder     (501) staff       (20)    21277 2023-10-05 08:27:15.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface.f90
--rw-r--r--   0 rieder     (501) staff       (20)    10090 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface.py
--rw-r--r--   0 rieder     (501) staff       (20)     1140 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface_new.py
--rw-r--r--   0 rieder     (501) staff       (20)      153 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/params.h
--rw-r--r--   0 rieder     (501) staff       (20)     4248 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/phigrape.py
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.516904 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/
--rw-r--r--   0 rieder     (501) staff       (20)    16277 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/Makefile
--rw-r--r--   0 rieder     (501) staff       (20)     5177 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/absorb.f
--rw-r--r--   0 rieder     (501) staff       (20)    12833 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/adjust.F
--rw-r--r--   0 rieder     (501) staff       (20)     2904 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/assess.f
--rw-r--r--   0 rieder     (501) staff       (20)     6847 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bindat.f
--rw-r--r--   0 rieder     (501) staff       (20)     2493 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binev.f
--rw-r--r--   0 rieder     (501) staff       (20)     6053 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binout.f
--rw-r--r--   0 rieder     (501) staff       (20)    23634 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binpop.F
--rw-r--r--   0 rieder     (501) staff       (20)      697 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/block.f
--rw-r--r--   0 rieder     (501) staff       (20)     4426 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bodies.f
--rw-r--r--   0 rieder     (501) staff       (20)     4225 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake.f
--rw-r--r--   0 rieder     (501) staff       (20)     7800 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake2.f
--rw-r--r--   0 rieder     (501) staff       (20)     4986 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake3.f
--rw-r--r--   0 rieder     (501) staff       (20)     1969 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bsetid.f
--rw-r--r--   0 rieder     (501) staff       (20)     1544 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cfuncs.f
--rw-r--r--   0 rieder     (501) staff       (20)    25315 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chain.f
--rw-r--r--   0 rieder     (501) staff       (20)    16794 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos.f
--rw-r--r--   0 rieder     (501) staff       (20)     2642 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos0.f
--rw-r--r--   0 rieder     (501) staff       (20)    12243 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1368 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chdata.f
--rw-r--r--   0 rieder     (501) staff       (20)     4087 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/check.f
--rw-r--r--   0 rieder     (501) staff       (20)     1614 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/check3.f
--rw-r--r--   0 rieder     (501) staff       (20)    10112 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/checkl.f
--rw-r--r--   0 rieder     (501) staff       (20)      680 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chfind.f
--rw-r--r--   0 rieder     (501) staff       (20)     5688 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chfirr.f
--rw-r--r--   0 rieder     (501) staff       (20)     5240 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chinit.f
--rw-r--r--   0 rieder     (501) staff       (20)     2466 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chlist.f
--rw-r--r--   0 rieder     (501) staff       (20)    22126 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chmod.f
--rw-r--r--   0 rieder     (501) staff       (20)     3032 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     1476 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chpot.f
--rw-r--r--   0 rieder     (501) staff       (20)    10290 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chrect.f
--rw-r--r--   0 rieder     (501) staff       (20)     6587 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chstab.f
--rw-r--r--   0 rieder     (501) staff       (20)    17465 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chterm.f
--rw-r--r--   0 rieder     (501) staff       (20)     1675 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/clint.f
--rw-r--r--   0 rieder     (501) staff       (20)     2343 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cloud.f
--rw-r--r--   0 rieder     (501) staff       (20)     2657 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cloud0.f
--rw-r--r--   0 rieder     (501) staff       (20)    22839 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmbody.f
--rw-r--r--   0 rieder     (501) staff       (20)     3354 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmcorr.f
--rw-r--r--   0 rieder     (501) staff       (20)     4603 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmfirr.f
--rw-r--r--   0 rieder     (501) staff       (20)     9380 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmfreg.f
--rw-r--r--   0 rieder     (501) staff       (20)    13893 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/coal.f
--rw-r--r--   0 rieder     (501) staff       (20)    14584 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/comenv.f
--rw-r--r--   0 rieder     (501) staff       (20)      108 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/common2.h
--rw-r--r--   0 rieder     (501) staff       (20)     4815 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/common6.h
--rw-r--r--   0 rieder     (501) staff       (20)      414 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/commonc.h
--rw-r--r--   0 rieder     (501) staff       (20)      982 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/const.f
--rw-r--r--   0 rieder     (501) staff       (20)     4837 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/core.f
--rw-r--r--   0 rieder     (501) staff       (20)     1259 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/corerd.f
--rw-r--r--   0 rieder     (501) staff       (20)      677 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cputim.F
--rw-r--r--   0 rieder     (501) staff       (20)     4622 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab2.f
--rw-r--r--   0 rieder     (501) staff       (20)     4738 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab3.f
--rw-r--r--   0 rieder     (501) staff       (20)     4203 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab4.f
--rw-r--r--   0 rieder     (501) staff       (20)     7371 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab5.f
--rw-r--r--   0 rieder     (501) staff       (20)     1139 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cuda_pointer.h
--rw-r--r--   0 rieder     (501) staff       (20)    46935 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cutil.h
--rw-r--r--   0 rieder     (501) staff       (20)     5544 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/data.F
--rw-r--r--   0 rieder     (501) staff       (20)     5900 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/decide.f
--rw-r--r--   0 rieder     (501) staff       (20)    17373 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/define.f
--rw-r--r--   0 rieder     (501) staff       (20)     2016 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/deform.f
--rw-r--r--   0 rieder     (501) staff       (20)     8278 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/degen.f
--rw-r--r--   0 rieder     (501) staff       (20)     2054 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/delay.f
--rw-r--r--   0 rieder     (501) staff       (20)    12172 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp.f
--rw-r--r--   0 rieder     (501) staff       (20)     7314 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp3.f
--rw-r--r--   0 rieder     (501) staff       (20)     9994 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp4.f
--rw-r--r--   0 rieder     (501) staff       (20)     4258 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/dgcore.f
--rw-r--r--   0 rieder     (501) staff       (20)     3287 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy1.f
--rw-r--r--   0 rieder     (501) staff       (20)     3222 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy3.f
--rw-r--r--   0 rieder     (501) staff       (20)     3207 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy4.f
--rw-r--r--   0 rieder     (501) staff       (20)      384 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/dtchck.f
--rw-r--r--   0 rieder     (501) staff       (20)     4471 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/eccmod.f
--rw-r--r--   0 rieder     (501) staff       (20)     3240 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ecirc.f
--rw-r--r--   0 rieder     (501) staff       (20)     1481 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/edot.f
--rw-r--r--   0 rieder     (501) staff       (20)     1503 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/efac2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1510 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/efac3.f
--rw-r--r--   0 rieder     (501) staff       (20)     4233 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/eigenvalue.f
--rw-r--r--   0 rieder     (501) staff       (20)     7867 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ellan.f
--rw-r--r--   0 rieder     (501) staff       (20)     2484 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/endreg.f
--rw-r--r--   0 rieder     (501) staff       (20)     2867 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy.f
--rw-r--r--   0 rieder     (501) staff       (20)     6378 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy_mpi.F
--rw-r--r--   0 rieder     (501) staff       (20)     3942 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy_scale.f
--rw-r--r--   0 rieder     (501) staff       (20)     1523 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel.f
--rw-r--r--   0 rieder     (501) staff       (20)     1715 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel3.f
--rw-r--r--   0 rieder     (501) staff       (20)     1451 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel4.f
--rw-r--r--   0 rieder     (501) staff       (20)    19840 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/escape.f
--rw-r--r--   0 rieder     (501) staff       (20)     2646 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/events.f
--rw-r--r--   0 rieder     (501) staff       (20)     8879 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/evolve.f
--rw-r--r--   0 rieder     (501) staff       (20)     1858 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expand.f
--rw-r--r--   0 rieder     (501) staff       (20)    14487 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expel.f
--rw-r--r--   0 rieder     (501) staff       (20)    13001 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expel2.f
--rw-r--r--   0 rieder     (501) staff       (20)     2426 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/extend.f
--rw-r--r--   0 rieder     (501) staff       (20)     2345 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fchain.f
--rw-r--r--   0 rieder     (501) staff       (20)     1132 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fclose.f
--rw-r--r--   0 rieder     (501) staff       (20)     1939 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fcloud.f
--rw-r--r--   0 rieder     (501) staff       (20)     4293 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fcorr.f
--rw-r--r--   0 rieder     (501) staff       (20)     1253 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fdisk.f
--rw-r--r--   0 rieder     (501) staff       (20)      704 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fhalo.f
--rw-r--r--   0 rieder     (501) staff       (20)     2177 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ficorr.f
--rw-r--r--   0 rieder     (501) staff       (20)     5740 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/file_init.F
--rw-r--r--   0 rieder     (501) staff       (20)     1659 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/findj.f
--rw-r--r--   0 rieder     (501) staff       (20)     3730 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/findm.f
--rw-r--r--   0 rieder     (501) staff       (20)       79 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/flush.f
--rw-r--r--   0 rieder     (501) staff       (20)       79 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/flush.t3e.f
--rw-r--r--   0 rieder     (501) staff       (20)     3970 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/flyby.f
--rw-r--r--   0 rieder     (501) staff       (20)      631 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fnuc.f
--rw-r--r--   0 rieder     (501) staff       (20)     4694 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpcorr.f
--rw-r--r--   0 rieder     (501) staff       (20)     1023 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     4267 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly1.f
--rw-r--r--   0 rieder     (501) staff       (20)     6710 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly1_mpi.f
--rw-r--r--   0 rieder     (501) staff       (20)     4347 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly2.f
--rw-r--r--   0 rieder     (501) staff       (20)     7077 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly2_mpi.f
--rw-r--r--   0 rieder     (501) staff       (20)     3469 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/freeze.f
--rw-r--r--   0 rieder     (501) staff       (20)      699 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gcinit.f
--rw-r--r--   0 rieder     (501) staff       (20)     2347 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gcint.f
--rw-r--r--   0 rieder     (501) staff       (20)     1182 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ghost.f
--rw-r--r--   0 rieder     (501) staff       (20)     3958 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant.f
--rw-r--r--   0 rieder     (501) staff       (20)     3587 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant2.f
--rw-r--r--   0 rieder     (501) staff       (20)     2350 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant3.f
--rw-r--r--   0 rieder     (501) staff       (20)     6787 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gntage.f
--rw-r--r--   0 rieder     (501) staff       (20)    17588 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gpunb.gpu.cu
--rw-r--r--   0 rieder     (501) staff       (20)     3841 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gpupot.gpu.cu
--rw-r--r--   0 rieder     (501) staff       (20)      669 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/grrad.f
--rw-r--r--   0 rieder     (501) staff       (20)     2593 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hcorr.f
--rw-r--r--   0 rieder     (501) staff       (20)    28150 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/helper_cuda.h
--rw-r--r--   0 rieder     (501) staff       (20)    16777 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/helper_string.h
--rw-r--r--   0 rieder     (501) staff       (20)     9988 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hiarch.f
--rw-r--r--   0 rieder     (501) staff       (20)     3234 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hicirc.f
--rw-r--r--   0 rieder     (501) staff       (20)     8995 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hidat.f
--rw-r--r--   0 rieder     (501) staff       (20)    17339 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/higrow.f
--rw-r--r--   0 rieder     (501) staff       (20)     4435 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himax.f
--rw-r--r--   0 rieder     (501) staff       (20)     3955 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himax2.f
--rw-r--r--   0 rieder     (501) staff       (20)     5887 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himod.f
--rw-r--r--   0 rieder     (501) staff       (20)     5858 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hipop.F
--rw-r--r--   0 rieder     (501) staff       (20)     2926 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hirect.f
--rw-r--r--   0 rieder     (501) staff       (20)     3527 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/histab.f
--rw-r--r--   0 rieder     (501) staff       (20)     6216 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hivel.f
--rw-r--r--   0 rieder     (501) staff       (20)     7108 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hmdot.f
--rw-r--r--   0 rieder     (501) staff       (20)     6086 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hmdot2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1593 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hotsys.f
--rw-r--r--   0 rieder     (501) staff       (20)      972 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hpsort.f
--rw-r--r--   0 rieder     (501) staff       (20)    23689 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag.f
--rw-r--r--   0 rieder     (501) staff       (20)    23123 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag.sverre.f
--rw-r--r--   0 rieder     (501) staff       (20)    21222 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag_fromJarrodnew.f
--rw-r--r--   0 rieder     (501) staff       (20)     5896 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrplot.f
--rw-r--r--   0 rieder     (501) staff       (20)     3655 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hut.f
--rw-r--r--   0 rieder     (501) staff       (20)     2967 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hut2.f
--rw-r--r--   0 rieder     (501) staff       (20)      390 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/iblock.f
--rw-r--r--   0 rieder     (501) staff       (20)     1903 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ichain.f
--rw-r--r--   0 rieder     (501) staff       (20)     1793 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imf.f
--rw-r--r--   0 rieder     (501) staff       (20)     4015 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imf2.f
--rw-r--r--   0 rieder     (501) staff       (20)    20460 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imfbd.f
--rw-r--r--   0 rieder     (501) staff       (20)    38011 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/impact.f
--rw-r--r--   0 rieder     (501) staff       (20)     1068 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/inclin.f
--rw-r--r--   0 rieder     (501) staff       (20)     1183 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/indexx.f
--rw-r--r--   0 rieder     (501) staff       (20)     6096 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/induce.f
--rw-r--r--   0 rieder     (501) staff       (20)      447 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/inext.f
--rw-r--r--   0 rieder     (501) staff       (20)     5589 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/input.F
--rw-r--r--   0 rieder     (501) staff       (20)     2635 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/insert.f
--rw-r--r--   0 rieder     (501) staff       (20)     6740 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/instar.f
--rw-r--r--   0 rieder     (501) staff       (20)     2027 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/int.amuse.F
--rw-r--r--   0 rieder     (501) staff       (20)    33532 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/intgrt.F
--rw-r--r--   0 rieder     (501) staff       (20)     8170 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/invert.f
--rw-r--r--   0 rieder     (501) staff       (20)     1354 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/jacobi.f
--rw-r--r--   0 rieder     (501) staff       (20)     1726 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kcpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     1347 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kepler.f
--rw-r--r--   0 rieder     (501) staff       (20)     6038 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick.f
--rw-r--r--   0 rieder     (501) staff       (20)     5873 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick.sverre.f
--rw-r--r--   0 rieder     (501) staff       (20)     1229 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1988 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksapo.f
--rw-r--r--   0 rieder     (501) staff       (20)     6846 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kscorr.f
--rw-r--r--   0 rieder     (501) staff       (20)     6941 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksin2.f
--rw-r--r--   0 rieder     (501) staff       (20)    10186 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksinit.f
--rw-r--r--   0 rieder     (501) staff       (20)    25322 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksint.f
--rw-r--r--   0 rieder     (501) staff       (20)     3957 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kslist.f
--rw-r--r--   0 rieder     (501) staff       (20)     3606 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksmod.f
--rw-r--r--   0 rieder     (501) staff       (20)     5876 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksperi.f
--rw-r--r--   0 rieder     (501) staff       (20)     6025 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspert.f
--rw-r--r--   0 rieder     (501) staff       (20)      648 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksphys.f
--rw-r--r--   0 rieder     (501) staff       (20)     9308 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspoly.f
--rw-r--r--   0 rieder     (501) staff       (20)     2841 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspred.f
--rw-r--r--   0 rieder     (501) staff       (20)     4068 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksrect.f
--rw-r--r--   0 rieder     (501) staff       (20)     4667 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksreg.f
--rw-r--r--   0 rieder     (501) staff       (20)     2134 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksres.f
--rw-r--r--   0 rieder     (501) staff       (20)     3105 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksres2.f
--rw-r--r--   0 rieder     (501) staff       (20)    13006 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksterm.f
--rw-r--r--   0 rieder     (501) staff       (20)    13169 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kstide.f
--rw-r--r--   0 rieder     (501) staff       (20)     7041 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/lagr.f
--rw-r--r--   0 rieder     (501) staff       (20)     6066 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/lagr2.f
--rw-r--r--   0 rieder     (501) staff       (20)     4304 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/levels.f
--rw-r--r--   0 rieder     (501) staff       (20)      327 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/magbrk.f
--rw-r--r--   0 rieder     (501) staff       (20)      443 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/matrix.f
--rw-r--r--   0 rieder     (501) staff       (20)    49941 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mdot.f
--rw-r--r--   0 rieder     (501) staff       (20)     9152 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/merge.f
--rw-r--r--   0 rieder     (501) staff       (20)    10565 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/merge2.f
--rw-r--r--   0 rieder     (501) staff       (20)    10139 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mix.f
--rw-r--r--   0 rieder     (501) staff       (20)     6160 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mloss.f
--rw-r--r--   0 rieder     (501) staff       (20)     2089 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mlwind.f
--rw-r--r--   0 rieder     (501) staff       (20)     3264 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/modify.F
--rw-r--r--   0 rieder     (501) staff       (20)     7833 2023-11-17 14:47:16.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mpif.h
--rw-r--r--   0 rieder     (501) staff       (20)     7833 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mpif.null.h
--rw-r--r--   0 rieder     (501) staff       (20)     6229 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mrenv.f
--rw-r--r--   0 rieder     (501) staff       (20)     2015 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mtrace.f
--rw-r--r--   0 rieder     (501) staff       (20)    13989 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mydump.F
--rw-r--r--   0 rieder     (501) staff       (20)     9160 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbint.f
--rw-r--r--   0 rieder     (501) staff       (20)     3366 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nblist.f
--rw-r--r--   0 rieder     (501) staff       (20)     6046 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbody6.F
--rw-r--r--   0 rieder     (501) staff       (20)     4390 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbody6.amuse.F
--rw-r--r--   0 rieder     (501) staff       (20)     1565 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbpot.f
--rw-r--r--   0 rieder     (501) staff       (20)     1773 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbrem.f
--rw-r--r--   0 rieder     (501) staff       (20)     1734 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbrest.f
--rw-r--r--   0 rieder     (501) staff       (20)     3554 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbsort.f
--rw-r--r--   0 rieder     (501) staff       (20)     3084 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbtide.f
--rw-r--r--   0 rieder     (501) staff       (20)     2957 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newreg.f
--rw-r--r--   0 rieder     (501) staff       (20)      891 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newsys.f
--rw-r--r--   0 rieder     (501) staff       (20)     3364 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newtev.f
--rw-r--r--   0 rieder     (501) staff       (20)     8045 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nstab.f
--rw-r--r--   0 rieder     (501) staff       (20)     1161 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/offset.f
--rw-r--r--   0 rieder     (501) staff       (20)     2373 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/orbit.f
--rw-r--r--   0 rieder     (501) staff       (20)    14786 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/output.F
--rw-r--r--   0 rieder     (501) staff       (20)     1303 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/params.h
--rw-r--r--   0 rieder     (501) staff       (20)     1893 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/peri.f
--rw-r--r--   0 rieder     (501) staff       (20)     1526 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/permit.f
--rw-r--r--   0 rieder     (501) staff       (20)     1313 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/pfac.f
--rw-r--r--   0 rieder     (501) staff       (20)     2923 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/phicor.f
--rw-r--r--   0 rieder     (501) staff       (20)      875 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/physks.f
--rw-r--r--   0 rieder     (501) staff       (20)      860 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/poti.f
--rw-r--r--   0 rieder     (501) staff       (20)     3744 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/proto_star.f
--rw-r--r--   0 rieder     (501) staff       (20)      400 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qforce.f
--rw-r--r--   0 rieder     (501) staff       (20)     9086 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod.f
--rw-r--r--   0 rieder     (501) staff       (20)     5332 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod3.f
--rw-r--r--   0 rieder     (501) staff       (20)     4361 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod4.f
--rw-r--r--   0 rieder     (501) staff       (20)     4915 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qtides.f
--rw-r--r--   0 rieder     (501) staff       (20)    12005 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/quad.f
--rw-r--r--   0 rieder     (501) staff       (20)      812 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/r2sort.f
--rw-r--r--   0 rieder     (501) staff       (20)     1370 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ran2.f
--rw-r--r--   0 rieder     (501) staff       (20)     4206 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rchain.f
--rw-r--r--   0 rieder     (501) staff       (20)     8112 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/recoil.f
--rw-r--r--   0 rieder     (501) staff       (20)      742 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/redraw.f
--rw-r--r--   0 rieder     (501) staff       (20)     8734 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reduce.f
--rw-r--r--   0 rieder     (501) staff       (20)     1006 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reflct.f
--rw-r--r--   0 rieder     (501) staff       (20)    29037 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/regint.F
--rw-r--r--   0 rieder     (501) staff       (20)     2050 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reinit.f
--rw-r--r--   0 rieder     (501) staff       (20)     3707 2020-03-24 14:36:25.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/remove.f
--rw-r--r--   0 rieder     (501) staff       (20)     7383 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rename.f
--rw-r--r--   0 rieder     (501) staff       (20)     1935 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/renew.f
--rw-r--r--   0 rieder     (501) staff       (20)    11084 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reset.f
--rw-r--r--   0 rieder     (501) staff       (20)    15083 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reset2.f
--rw-r--r--   0 rieder     (501) staff       (20)     4368 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/resolv.f
--rw-r--r--   0 rieder     (501) staff       (20)      707 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/resort.f
--rw-r--r--   0 rieder     (501) staff       (20)     4925 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rkint.f
--rw-r--r--   0 rieder     (501) staff       (20)      197 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rl.f
--rw-r--r--   0 rieder     (501) staff       (20)    57054 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/roche.f
--rw-r--r--   0 rieder     (501) staff       (20)      686 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmax.f
--rw-r--r--   0 rieder     (501) staff       (20)     1574 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmax2.f
--rw-r--r--   0 rieder     (501) staff       (20)      945 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmin.f
--rw-r--r--   0 rieder     (501) staff       (20)      607 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rsort.f
--rw-r--r--   0 rieder     (501) staff       (20)      497 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rssort.f
--rw-r--r--   0 rieder     (501) staff       (20)     5509 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/scale.F
--rw-r--r--   0 rieder     (501) staff       (20)     5179 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/search.f
--rw-r--r--   0 rieder     (501) staff       (20)     1115 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/select.f
--rw-r--r--   0 rieder     (501) staff       (20)     7148 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setsys.f
--rw-r--r--   0 rieder     (501) staff       (20)     2803 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setup.f
--rw-r--r--   0 rieder     (501) staff       (20)     1131 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setup2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1414 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/short.f
--rw-r--r--   0 rieder     (501) staff       (20)     2495 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/shrink.f
--rw-r--r--   0 rieder     (501) staff       (20)    12030 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/slow.f
--rw-r--r--   0 rieder     (501) staff       (20)      983 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sort1.f
--rw-r--r--   0 rieder     (501) staff       (20)     1921 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sort3.f
--rw-r--r--   0 rieder     (501) staff       (20)    25633 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/spiral.f
--rw-r--r--   0 rieder     (501) staff       (20)      547 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stability.f
--rw-r--r--   0 rieder     (501) staff       (20)     3634 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stabl3.f
--rw-r--r--   0 rieder     (501) staff       (20)     5495 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stabl4.f
--rw-r--r--   0 rieder     (501) staff       (20)     5136 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stablc.f
--rw-r--r--   0 rieder     (501) staff       (20)     2196 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stablz.f
--rw-r--r--   0 rieder     (501) staff       (20)    12734 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/star.f
--rw-r--r--   0 rieder     (501) staff       (20)     5767 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start.F
--rw-r--r--   0 rieder     (501) staff       (20)    10486 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start3.f
--rw-r--r--   0 rieder     (501) staff       (20)    10909 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start4.f
--rw-r--r--   0 rieder     (501) staff       (20)     1768 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/status.f
--rw-r--r--   0 rieder     (501) staff       (20)      773 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stepi.f
--rw-r--r--   0 rieder     (501) staff       (20)      780 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stepk.f
--rw-r--r--   0 rieder     (501) staff       (20)     3068 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/steps.f
--rw-r--r--   0 rieder     (501) staff       (20)     1088 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stumpf.f
--rw-r--r--   0 rieder     (501) staff       (20)     6446 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/subint.f
--rw-r--r--   0 rieder     (501) staff       (20)     2870 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/subsys.f
--rw-r--r--   0 rieder     (501) staff       (20)       45 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/swap.f
--rw-r--r--   0 rieder     (501) staff       (20)     1308 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/swcond.f
--rw-r--r--   0 rieder     (501) staff       (20)     2599 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sweep.f
--rw-r--r--   0 rieder     (501) staff       (20)     4247 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/switch.f
--rw-r--r--   0 rieder     (501) staff       (20)    19307 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/synch.f
--rw-r--r--   0 rieder     (501) staff       (20)     1206 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tchain.f
--rw-r--r--   0 rieder     (501) staff       (20)     4917 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tcirc.f
--rw-r--r--   0 rieder     (501) staff       (20)     1469 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides.f
--rw-r--r--   0 rieder     (501) staff       (20)     2070 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides2.f
--rw-r--r--   0 rieder     (501) staff       (20)     1182 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides3.f
--rw-r--r--   0 rieder     (501) staff       (20)      580 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/touch.f
--rw-r--r--   0 rieder     (501) staff       (20)     2436 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tperi.f
--rw-r--r--   0 rieder     (501) staff       (20)     2314 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     6353 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trans3.f
--rw-r--r--   0 rieder     (501) staff       (20)     2221 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trans4.f
--rw-r--r--   0 rieder     (501) staff       (20)     1864 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transk.f
--rw-r--r--   0 rieder     (501) staff       (20)     1799 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transq.f
--rw-r--r--   0 rieder     (501) staff       (20)     1167 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transx.f
--rw-r--r--   0 rieder     (501) staff       (20)     4054 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trdot.f
--rw-r--r--   0 rieder     (501) staff       (20)     1672 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trdot2.f
--rw-r--r--   0 rieder     (501) staff       (20)    11258 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trflow.f
--rw-r--r--   0 rieder     (501) staff       (20)    16894 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/triple.f
--rw-r--r--   0 rieder     (501) staff       (20)     1667 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tstab.f
--rw-r--r--   0 rieder     (501) staff       (20)      678 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tstep.f
--rw-r--r--   0 rieder     (501) staff       (20)     2104 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/units.f
--rw-r--r--   0 rieder     (501) staff       (20)    11010 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/unpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     6693 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/update.f
--rw-r--r--   0 rieder     (501) staff       (20)     4346 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/util_gpu.F
--rw-r--r--   0 rieder     (501) staff       (20)      462 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/vector.f
--rw-r--r--   0 rieder     (501) staff       (20)     1866 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/verify.f
--rw-r--r--   0 rieder     (501) staff       (20)     1817 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xcpred.f
--rw-r--r--   0 rieder     (501) staff       (20)     1225 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtf.f
--rw-r--r--   0 rieder     (501) staff       (20)     2597 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtpert.f
--rw-r--r--   0 rieder     (501) staff       (20)     9749 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnl0.F
--rw-r--r--   0 rieder     (501) staff       (20)     2233 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnld.f
--rw-r--r--   0 rieder     (501) staff       (20)     3207 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlf.f
--rw-r--r--   0 rieder     (501) staff       (20)      501 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlp.f
--rw-r--r--   0 rieder     (501) staff       (20)     1343 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlt.f
--rw-r--r--   0 rieder     (501) staff       (20)      314 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlu.f
--rw-r--r--   0 rieder     (501) staff       (20)     3066 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlv.f
--rw-r--r--   0 rieder     (501) staff       (20)     3364 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xvpred.f
--rw-r--r--   0 rieder     (501) staff       (20)      519 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ycopy.f
--rw-r--r--   0 rieder     (501) staff       (20)      515 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ysave.f
--rw-r--r--   0 rieder     (501) staff       (20)     3451 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zare.f
--rw-r--r--   0 rieder     (501) staff       (20)    16419 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zcnsts.f
--rw-r--r--   0 rieder     (501) staff       (20)    10438 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zdata.h
--rw-r--r--   0 rieder     (501) staff       (20)     2375 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zero.f
--rw-r--r--   0 rieder     (501) staff       (20)    24674 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zfuncs.f
-drwxr-xr-x   0 rieder     (501) staff       (20)        0 2023-11-20 12:42:32.518140 amuse-nbody6xx-2023.11.0/support/
--rw-r--r--   0 rieder     (501) staff       (20)      586 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/support/__init__.py
--rw-r--r--   0 rieder     (501) staff       (20)      841 2021-07-05 11:19:28.000000 amuse-nbody6xx-2023.11.0/support/classifiers.py
--rw-r--r--   0 rieder     (501) staff       (20)     2831 2022-11-30 13:58:15.000000 amuse-nbody6xx-2023.11.0/support/config.py
--rw-r--r--   0 rieder     (501) staff       (20)     2167 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/support/generate_main.py
--rw-r--r--   0 rieder     (501) staff       (20)     1356 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/support/getsp.class
--rw-r--r--   0 rieder     (501) staff       (20)      898 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/support/getsp.java
--rw-r--r--   0 rieder     (501) staff       (20)     1420 2020-03-24 14:36:26.000000 amuse-nbody6xx-2023.11.0/support/misc.py
--rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-09-24 08:36:42.000000 amuse-nbody6xx-2023.11.0/support/setup_codes.py
--rw-r--r--   0 rieder     (501) staff       (20)      145 2021-04-14 10:14:49.000000 amuse-nbody6xx-2023.11.0/support/version.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.293823 amuse-nbody6xx-2024.4.0/
+-rw-r--r--   0 rieder     (501) staff       (20)      216 2024-04-24 15:35:29.000000 amuse-nbody6xx-2024.4.0/MANIFEST.in
+-rw-r--r--   0 rieder     (501) staff       (20)     1223 2024-04-24 16:32:40.293600 amuse-nbody6xx-2024.4.0/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)       61 2024-04-24 15:35:29.000000 amuse-nbody6xx-2024.4.0/README.md
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.293022 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/
+-rw-r--r--   0 rieder     (501) staff       (20)     1223 2024-04-24 16:32:39.000000 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/PKG-INFO
+-rw-r--r--   0 rieder     (501) staff       (20)    14722 2024-04-24 16:32:40.000000 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/SOURCES.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        1 2024-04-24 16:32:39.000000 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/dependency_links.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       16 2024-04-24 16:32:39.000000 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/requires.txt
+-rw-r--r--   0 rieder     (501) staff       (20)        6 2024-04-24 16:32:39.000000 amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/top_level.txt
+-rw-r--r--   0 rieder     (501) staff       (20)       93 2024-04-24 15:35:29.000000 amuse-nbody6xx-2024.4.0/pyproject.toml
+-rw-r--r--   0 rieder     (501) staff       (20)       38 2024-04-24 16:32:40.293877 amuse-nbody6xx-2024.4.0/setup.cfg
+-rw-r--r--   0 rieder     (501) staff       (20)     1593 2024-04-24 15:35:29.000000 amuse-nbody6xx-2024.4.0/setup.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.234040 amuse-nbody6xx-2024.4.0/src/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.234092 amuse-nbody6xx-2024.4.0/src/amuse/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.234143 amuse-nbody6xx-2024.4.0/src/amuse/community/
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.237193 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/
+-rw-r--r--   0 rieder     (501) staff       (20)     1165 2023-03-14 13:48:49.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)       49 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      417 2024-04-24 16:32:39.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/_version.py
+-rw-r--r--   0 rieder     (501) staff       (20)     4417 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/common6.h
+-rw-r--r--   0 rieder     (501) staff       (20)      622 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/debug.py
+-rw-r--r--   0 rieder     (501) staff       (20)    21038 2024-04-24 15:35:29.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface.f90
+-rw-r--r--   0 rieder     (501) staff       (20)    10090 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1140 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface_new.py
+-rw-r--r--   0 rieder     (501) staff       (20)      153 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/params.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4248 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/phigrape.py
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.291572 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/
+-rw-r--r--   0 rieder     (501) staff       (20)    16277 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/Makefile
+-rw-r--r--   0 rieder     (501) staff       (20)     5177 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/absorb.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12833 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/adjust.F
+-rw-r--r--   0 rieder     (501) staff       (20)     2904 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/assess.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6847 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bindat.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2493 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binev.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6053 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binout.f
+-rw-r--r--   0 rieder     (501) staff       (20)    23634 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binpop.F
+-rw-r--r--   0 rieder     (501) staff       (20)      697 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/block.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4426 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bodies.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4225 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7800 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4986 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1969 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bsetid.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1544 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cfuncs.f
+-rw-r--r--   0 rieder     (501) staff       (20)    25315 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chain.f
+-rw-r--r--   0 rieder     (501) staff       (20)    16794 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2642 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos0.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12243 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1368 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chdata.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4087 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/check.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1614 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/check3.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10112 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/checkl.f
+-rw-r--r--   0 rieder     (501) staff       (20)      680 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chfind.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5688 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chfirr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5240 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chinit.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2466 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chlist.f
+-rw-r--r--   0 rieder     (501) staff       (20)    22126 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chmod.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3032 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1476 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chpot.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10290 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chrect.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6587 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chstab.f
+-rw-r--r--   0 rieder     (501) staff       (20)    17465 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chterm.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1675 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/clint.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2343 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cloud.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2657 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cloud0.f
+-rw-r--r--   0 rieder     (501) staff       (20)    22839 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmbody.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3354 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmcorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4603 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmfirr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9380 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmfreg.f
+-rw-r--r--   0 rieder     (501) staff       (20)    13893 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/coal.f
+-rw-r--r--   0 rieder     (501) staff       (20)    14584 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/comenv.f
+-rw-r--r--   0 rieder     (501) staff       (20)      108 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/common2.h
+-rw-r--r--   0 rieder     (501) staff       (20)     4815 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/common6.h
+-rw-r--r--   0 rieder     (501) staff       (20)      414 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/commonc.h
+-rw-r--r--   0 rieder     (501) staff       (20)      982 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/const.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4837 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/core.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1259 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/corerd.f
+-rw-r--r--   0 rieder     (501) staff       (20)      677 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cputim.F
+-rw-r--r--   0 rieder     (501) staff       (20)     4622 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4738 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4203 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7371 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab5.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1139 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cuda_pointer.h
+-rw-r--r--   0 rieder     (501) staff       (20)    46935 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cutil.h
+-rw-r--r--   0 rieder     (501) staff       (20)     5544 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/data.F
+-rw-r--r--   0 rieder     (501) staff       (20)     5900 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/decide.f
+-rw-r--r--   0 rieder     (501) staff       (20)    17373 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/define.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2016 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/deform.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8278 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/degen.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2054 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/delay.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12172 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7314 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9994 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4258 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/dgcore.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3287 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy1.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3222 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3207 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy4.f
+-rw-r--r--   0 rieder     (501) staff       (20)      384 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/dtchck.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4471 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/eccmod.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3240 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ecirc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1481 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/edot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1503 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/efac2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1510 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/efac3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4233 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/eigenvalue.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7867 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ellan.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2484 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/endreg.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2867 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6378 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy_mpi.F
+-rw-r--r--   0 rieder     (501) staff       (20)     3942 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy_scale.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1523 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1715 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1451 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel4.f
+-rw-r--r--   0 rieder     (501) staff       (20)    19840 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/escape.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2646 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/events.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8879 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/evolve.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1858 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expand.f
+-rw-r--r--   0 rieder     (501) staff       (20)    14487 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expel.f
+-rw-r--r--   0 rieder     (501) staff       (20)    13001 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expel2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2426 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/extend.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2345 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fchain.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1132 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fclose.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1939 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fcloud.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4293 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fcorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1253 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fdisk.f
+-rw-r--r--   0 rieder     (501) staff       (20)      704 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fhalo.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2177 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ficorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5740 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/file_init.F
+-rw-r--r--   0 rieder     (501) staff       (20)     1659 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/findj.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3730 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/findm.f
+-rw-r--r--   0 rieder     (501) staff       (20)       79 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/flush.f
+-rw-r--r--   0 rieder     (501) staff       (20)       79 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/flush.t3e.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3970 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/flyby.f
+-rw-r--r--   0 rieder     (501) staff       (20)      631 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fnuc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4694 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpcorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1023 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4267 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly1.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6710 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly1_mpi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4347 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7077 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly2_mpi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3469 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/freeze.f
+-rw-r--r--   0 rieder     (501) staff       (20)      699 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gcinit.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2347 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gcint.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1182 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ghost.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3958 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3587 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2350 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6787 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gntage.f
+-rw-r--r--   0 rieder     (501) staff       (20)    17588 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gpunb.gpu.cu
+-rw-r--r--   0 rieder     (501) staff       (20)     3841 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gpupot.gpu.cu
+-rw-r--r--   0 rieder     (501) staff       (20)      669 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/grrad.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2593 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hcorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)    28150 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/helper_cuda.h
+-rw-r--r--   0 rieder     (501) staff       (20)    16777 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/helper_string.h
+-rw-r--r--   0 rieder     (501) staff       (20)     9988 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hiarch.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3234 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hicirc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8995 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hidat.f
+-rw-r--r--   0 rieder     (501) staff       (20)    17339 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/higrow.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4435 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himax.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3955 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himax2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5887 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himod.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5858 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hipop.F
+-rw-r--r--   0 rieder     (501) staff       (20)     2926 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hirect.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3527 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/histab.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6216 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hivel.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7108 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hmdot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6086 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hmdot2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1593 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hotsys.f
+-rw-r--r--   0 rieder     (501) staff       (20)      972 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hpsort.f
+-rw-r--r--   0 rieder     (501) staff       (20)    23689 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag.f
+-rw-r--r--   0 rieder     (501) staff       (20)    23123 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag.sverre.f
+-rw-r--r--   0 rieder     (501) staff       (20)    21222 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag_fromJarrodnew.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5896 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrplot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3655 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hut.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2967 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hut2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      390 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/iblock.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1903 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ichain.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1793 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4015 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imf2.f
+-rw-r--r--   0 rieder     (501) staff       (20)    20460 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imfbd.f
+-rw-r--r--   0 rieder     (501) staff       (20)    38011 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/impact.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1068 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/inclin.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1183 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/indexx.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6096 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/induce.f
+-rw-r--r--   0 rieder     (501) staff       (20)      447 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/inext.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5589 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/input.F
+-rw-r--r--   0 rieder     (501) staff       (20)     2635 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/insert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6740 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/instar.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2027 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/int.amuse.F
+-rw-r--r--   0 rieder     (501) staff       (20)    33532 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/intgrt.F
+-rw-r--r--   0 rieder     (501) staff       (20)     8170 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/invert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1354 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/jacobi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1726 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kcpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1347 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kepler.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6038 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5873 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick.sverre.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1229 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1988 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksapo.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6846 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kscorr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6941 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksin2.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10186 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksinit.f
+-rw-r--r--   0 rieder     (501) staff       (20)    25322 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksint.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3957 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kslist.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3606 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksmod.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5876 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksperi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6025 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspert.f
+-rw-r--r--   0 rieder     (501) staff       (20)      648 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksphys.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9308 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspoly.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2841 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspred.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4068 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksrect.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4667 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksreg.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2134 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksres.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3105 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksres2.f
+-rw-r--r--   0 rieder     (501) staff       (20)    13006 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksterm.f
+-rw-r--r--   0 rieder     (501) staff       (20)    13169 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kstide.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7041 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/lagr.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6066 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/lagr2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4304 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/levels.f
+-rw-r--r--   0 rieder     (501) staff       (20)      327 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/magbrk.f
+-rw-r--r--   0 rieder     (501) staff       (20)      443 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/matrix.f
+-rw-r--r--   0 rieder     (501) staff       (20)    49941 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mdot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9152 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/merge.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10565 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/merge2.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10139 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mix.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6160 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mloss.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2089 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mlwind.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3264 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/modify.F
+-rw-r--r--   0 rieder     (501) staff       (20)     7833 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mpif.h
+-rw-r--r--   0 rieder     (501) staff       (20)     7833 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mpif.null.h
+-rw-r--r--   0 rieder     (501) staff       (20)     6229 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mrenv.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2015 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mtrace.f
+-rw-r--r--   0 rieder     (501) staff       (20)    13989 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mydump.F
+-rw-r--r--   0 rieder     (501) staff       (20)     9160 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbint.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3366 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nblist.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6046 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbody6.F
+-rw-r--r--   0 rieder     (501) staff       (20)     4390 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbody6.amuse.F
+-rw-r--r--   0 rieder     (501) staff       (20)     1565 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbpot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1773 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbrem.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1734 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbrest.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3554 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbsort.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3084 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbtide.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2957 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newreg.f
+-rw-r--r--   0 rieder     (501) staff       (20)      891 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newsys.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3364 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newtev.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8045 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nstab.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1161 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/offset.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2373 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/orbit.f
+-rw-r--r--   0 rieder     (501) staff       (20)    14786 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/output.F
+-rw-r--r--   0 rieder     (501) staff       (20)     1303 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/params.h
+-rw-r--r--   0 rieder     (501) staff       (20)     1893 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/peri.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1526 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/permit.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1313 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/pfac.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2923 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/phicor.f
+-rw-r--r--   0 rieder     (501) staff       (20)      875 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/physks.f
+-rw-r--r--   0 rieder     (501) staff       (20)      860 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/poti.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3744 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/proto_star.f
+-rw-r--r--   0 rieder     (501) staff       (20)      400 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qforce.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9086 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5332 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4361 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4915 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qtides.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12005 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/quad.f
+-rw-r--r--   0 rieder     (501) staff       (20)      812 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/r2sort.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1370 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ran2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4206 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rchain.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8112 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/recoil.f
+-rw-r--r--   0 rieder     (501) staff       (20)      742 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/redraw.f
+-rw-r--r--   0 rieder     (501) staff       (20)     8734 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reduce.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1006 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reflct.f
+-rw-r--r--   0 rieder     (501) staff       (20)    29037 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/regint.F
+-rw-r--r--   0 rieder     (501) staff       (20)     2050 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reinit.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3707 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/remove.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7383 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rename.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1935 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/renew.f
+-rw-r--r--   0 rieder     (501) staff       (20)    11084 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reset.f
+-rw-r--r--   0 rieder     (501) staff       (20)    15083 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reset2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4368 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/resolv.f
+-rw-r--r--   0 rieder     (501) staff       (20)      707 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/resort.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4925 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rkint.f
+-rw-r--r--   0 rieder     (501) staff       (20)      197 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rl.f
+-rw-r--r--   0 rieder     (501) staff       (20)    57054 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/roche.f
+-rw-r--r--   0 rieder     (501) staff       (20)      686 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmax.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1574 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmax2.f
+-rw-r--r--   0 rieder     (501) staff       (20)      945 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmin.f
+-rw-r--r--   0 rieder     (501) staff       (20)      607 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rsort.f
+-rw-r--r--   0 rieder     (501) staff       (20)      497 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rssort.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5509 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/scale.F
+-rw-r--r--   0 rieder     (501) staff       (20)     5179 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/search.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1115 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/select.f
+-rw-r--r--   0 rieder     (501) staff       (20)     7148 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setsys.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2803 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setup.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1131 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setup2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1414 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/short.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2495 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/shrink.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12030 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/slow.f
+-rw-r--r--   0 rieder     (501) staff       (20)      983 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sort1.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1921 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sort3.f
+-rw-r--r--   0 rieder     (501) staff       (20)    25633 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/spiral.f
+-rw-r--r--   0 rieder     (501) staff       (20)      547 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stability.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3634 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stabl3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5495 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stabl4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5136 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stablc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2196 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stablz.f
+-rw-r--r--   0 rieder     (501) staff       (20)    12734 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/star.f
+-rw-r--r--   0 rieder     (501) staff       (20)     5767 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start.F
+-rw-r--r--   0 rieder     (501) staff       (20)    10486 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start3.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10909 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1768 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/status.f
+-rw-r--r--   0 rieder     (501) staff       (20)      773 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stepi.f
+-rw-r--r--   0 rieder     (501) staff       (20)      780 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stepk.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3068 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/steps.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1088 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stumpf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6446 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/subint.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2870 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/subsys.f
+-rw-r--r--   0 rieder     (501) staff       (20)       45 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/swap.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1308 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/swcond.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2599 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sweep.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4247 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/switch.f
+-rw-r--r--   0 rieder     (501) staff       (20)    19307 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/synch.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1206 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tchain.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4917 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tcirc.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1469 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2070 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides2.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1182 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides3.f
+-rw-r--r--   0 rieder     (501) staff       (20)      580 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/touch.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2436 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tperi.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2314 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6353 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trans3.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2221 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trans4.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1864 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transk.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1799 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transq.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1167 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transx.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4054 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trdot.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1672 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trdot2.f
+-rw-r--r--   0 rieder     (501) staff       (20)    11258 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trflow.f
+-rw-r--r--   0 rieder     (501) staff       (20)    16894 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/triple.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1667 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tstab.f
+-rw-r--r--   0 rieder     (501) staff       (20)      678 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tstep.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2104 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/units.f
+-rw-r--r--   0 rieder     (501) staff       (20)    11010 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/unpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     6693 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/update.f
+-rw-r--r--   0 rieder     (501) staff       (20)     4346 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/util_gpu.F
+-rw-r--r--   0 rieder     (501) staff       (20)      462 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/vector.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1866 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/verify.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1817 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xcpred.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1225 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtf.f
+-rw-r--r--   0 rieder     (501) staff       (20)     2597 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtpert.f
+-rw-r--r--   0 rieder     (501) staff       (20)     9749 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnl0.F
+-rw-r--r--   0 rieder     (501) staff       (20)     2233 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnld.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3207 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlf.f
+-rw-r--r--   0 rieder     (501) staff       (20)      501 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlp.f
+-rw-r--r--   0 rieder     (501) staff       (20)     1343 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlt.f
+-rw-r--r--   0 rieder     (501) staff       (20)      314 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlu.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3066 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlv.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3364 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xvpred.f
+-rw-r--r--   0 rieder     (501) staff       (20)      519 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ycopy.f
+-rw-r--r--   0 rieder     (501) staff       (20)      515 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ysave.f
+-rw-r--r--   0 rieder     (501) staff       (20)     3451 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zare.f
+-rw-r--r--   0 rieder     (501) staff       (20)    16419 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zcnsts.f
+-rw-r--r--   0 rieder     (501) staff       (20)    10438 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zdata.h
+-rw-r--r--   0 rieder     (501) staff       (20)     2375 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zero.f
+-rw-r--r--   0 rieder     (501) staff       (20)    24674 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zfuncs.f
+drwxr-xr-x   0 rieder     (501) staff       (20)        0 2024-04-24 16:32:40.292840 amuse-nbody6xx-2024.4.0/support/
+-rw-r--r--   0 rieder     (501) staff       (20)      586 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/__init__.py
+-rw-r--r--   0 rieder     (501) staff       (20)      841 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/classifiers.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2831 2023-03-14 13:48:49.000000 amuse-nbody6xx-2024.4.0/support/config.py
+-rw-r--r--   0 rieder     (501) staff       (20)     2167 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/generate_main.py
+-rw-r--r--   0 rieder     (501) staff       (20)     1356 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/getsp.class
+-rw-r--r--   0 rieder     (501) staff       (20)      898 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/getsp.java
+-rw-r--r--   0 rieder     (501) staff       (20)     1420 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/misc.py
+-rw-r--r--   0 rieder     (501) staff       (20)    49244 2023-05-26 13:47:38.000000 amuse-nbody6xx-2024.4.0/support/setup_codes.py
+-rw-r--r--   0 rieder     (501) staff       (20)      145 2022-11-22 11:55:15.000000 amuse-nbody6xx-2024.4.0/support/version.py
```

### Comparing `amuse-nbody6xx-2023.11.0/PKG-INFO` & `amuse-nbody6xx-2024.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-nbody6xx
-Version: 2023.11.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Nbody6++
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/PKG-INFO` & `amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amuse-nbody6xx
-Version: 2023.11.0
+Version: 2024.4.0
 Summary: The Astrophysical Multipurpose Software Environment - Nbody6++
 Home-page: http://www.amusecode.org/
 Author: The AMUSE team
 Author-email: info@amusecode.org
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `amuse-nbody6xx-2023.11.0/amuse_nbody6xx.egg-info/SOURCES.txt` & `amuse-nbody6xx-2024.4.0/amuse_nbody6xx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/setup.py` & `amuse-nbody6xx-2024.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/Makefile` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/common6.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/common6.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/debug.py` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/debug.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface.f90` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface.f90`

 * *Files 6% similar despite different names*

```diff
@@ -297,21 +297,14 @@
         ay_amuse = FI(2, index_of_the_particle) + FR(2,
      &   index_of_the_particle)
         az_amuse = FI(3, index_of_the_particle) + FR(3,
      &   index_of_the_particle)
         get_acceleration = 0
       END FUNCTION
       
-      FUNCTION set_acceleration(index_of_the_particle, ax, ay, az)
-        INTEGER :: index_of_the_particle
-        DOUBLE PRECISION :: ax, ay, az
-        INTEGER :: set_acceleration
-        set_acceleration = -2
-      END FUNCTION
-      
       FUNCTION get_potential(index_of_the_particle, potential)
         INCLUDE 'src/common6.h'
         INTEGER :: index_of_the_particle
         DOUBLE PRECISION :: potential
         INTEGER :: get_potential
         potential = PHIDBL(index_of_the_particle)
         get_potential = 0
```

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface.py` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/interface_new.py` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/interface_new.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/phigrape.py` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/phigrape.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/Makefile` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/Makefile`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/absorb.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/absorb.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/adjust.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/adjust.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/assess.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/assess.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bindat.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bindat.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binev.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binev.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binout.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binout.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/binpop.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/binpop.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/block.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/block.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bodies.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bodies.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/brake3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/brake3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/bsetid.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/bsetid.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cfuncs.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cfuncs.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chain.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chain.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos0.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos0.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chaos2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chaos2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chdata.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chdata.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/check.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/check.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/check3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/check3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/checkl.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/checkl.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chfind.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chfind.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chfirr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chfirr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chinit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chinit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chlist.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chlist.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chmod.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chmod.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chpot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chpot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chrect.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chrect.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chstab.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chstab.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/chterm.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/chterm.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/clint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/clint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cloud.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cloud.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cloud0.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cloud0.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmbody.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmbody.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmcorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmcorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmfirr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmfirr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cmfreg.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cmfreg.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/coal.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/coal.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/comenv.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/comenv.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/common6.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/common6.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/const.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/const.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/core.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/core.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/corerd.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/corerd.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cputim.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cputim.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cstab5.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cstab5.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cuda_pointer.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cuda_pointer.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/cutil.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/cutil.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/data.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/data.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/decide.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/decide.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/define.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/define.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/deform.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/deform.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/degen.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/degen.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/delay.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/delay.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/derqp4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/derqp4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/dgcore.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/dgcore.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy1.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy1.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/difsy4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/difsy4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/eccmod.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/eccmod.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ecirc.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ecirc.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/edot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/edot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/efac2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/efac2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/efac3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/efac3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/eigenvalue.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/eigenvalue.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ellan.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ellan.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/endreg.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/endreg.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy_mpi.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy_mpi.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/energy_scale.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/energy_scale.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/erel4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/erel4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/escape.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/escape.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/events.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/events.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/evolve.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/evolve.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expand.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expand.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expel.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expel.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/expel2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/expel2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/extend.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/extend.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fchain.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fchain.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fclose.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fclose.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fcloud.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fcloud.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fcorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fcorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fdisk.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fdisk.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fhalo.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fhalo.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ficorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ficorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/file_init.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/file_init.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/findj.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/findj.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/findm.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/findm.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/flyby.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/flyby.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fnuc.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fnuc.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpcorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpcorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly1.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly1.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly1_mpi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly1_mpi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/fpoly2_mpi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/fpoly2_mpi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/freeze.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/freeze.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gcinit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gcinit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gcint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gcint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ghost.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ghost.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/giant3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/giant3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gntage.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gntage.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gpunb.gpu.cu` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gpunb.gpu.cu`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/gpupot.gpu.cu` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/gpupot.gpu.cu`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/grrad.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/grrad.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hcorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hcorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/helper_cuda.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/helper_cuda.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/helper_string.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/helper_string.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hiarch.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hiarch.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hicirc.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hicirc.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hidat.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hidat.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/higrow.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/higrow.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himax.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himax.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himax2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himax2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/himod.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/himod.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hipop.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hipop.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hirect.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hirect.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/histab.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/histab.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hivel.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hivel.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hmdot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hmdot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hmdot2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hmdot2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hotsys.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hotsys.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hpsort.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hpsort.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag.sverre.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag.sverre.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrdiag_fromJarrodnew.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrdiag_fromJarrodnew.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hrplot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hrplot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hut.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hut.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/hut2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/hut2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ichain.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ichain.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imf.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imf.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imf2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imf2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/imfbd.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/imfbd.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/impact.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/impact.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/inclin.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/inclin.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/indexx.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/indexx.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/induce.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/induce.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/input.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/input.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/insert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/insert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/instar.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/instar.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/int.amuse.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/int.amuse.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/intgrt.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/intgrt.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/invert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/invert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/jacobi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/jacobi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kcpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kcpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kepler.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kepler.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick.sverre.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick.sverre.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kick2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kick2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksapo.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksapo.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kscorr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kscorr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksin2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksin2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksinit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksinit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kslist.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kslist.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksmod.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksmod.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksperi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksperi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksphys.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksphys.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspoly.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspoly.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kspred.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kspred.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksrect.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksrect.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksreg.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksreg.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksres.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksres.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksres2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksres2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ksterm.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ksterm.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/kstide.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/kstide.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/lagr.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/lagr.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/lagr2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/lagr2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/levels.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/levels.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mdot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mdot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/merge.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/merge.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/merge2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/merge2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mix.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mix.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mloss.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mloss.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mlwind.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mlwind.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/modify.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/modify.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mpif.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mpif.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mpif.null.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mpif.null.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mrenv.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mrenv.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mtrace.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mtrace.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/mydump.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/mydump.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nblist.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nblist.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbody6.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbody6.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbody6.amuse.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbody6.amuse.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbpot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbpot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbrem.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbrem.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbrest.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbrest.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbsort.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbsort.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nbtide.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nbtide.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newreg.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newreg.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newsys.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newsys.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/newtev.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/newtev.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/nstab.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/nstab.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/offset.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/offset.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/orbit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/orbit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/output.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/output.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/params.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/params.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/peri.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/peri.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/permit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/permit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/pfac.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/pfac.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/phicor.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/phicor.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/physks.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/physks.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/poti.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/poti.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/proto_star.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/proto_star.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qpmod4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qpmod4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/qtides.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/qtides.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/quad.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/quad.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/r2sort.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/r2sort.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ran2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ran2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rchain.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rchain.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/recoil.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/recoil.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/redraw.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/redraw.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reduce.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reduce.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reflct.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reflct.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/regint.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/regint.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reinit.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reinit.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/remove.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/remove.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rename.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rename.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/renew.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/renew.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reset.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reset.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/reset2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/reset2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/resolv.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/resolv.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/resort.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/resort.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rkint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rkint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/roche.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/roche.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmax.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmax.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmax2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmax2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rpmin.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rpmin.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/rsort.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/rsort.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/scale.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/scale.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/search.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/search.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/select.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/select.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setsys.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setsys.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setup.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setup.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/setup2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/setup2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/short.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/short.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/shrink.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/shrink.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/slow.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/slow.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sort1.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sort1.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sort3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sort3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/spiral.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/spiral.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stability.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stability.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stabl3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stabl3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stabl4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stabl4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stablc.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stablc.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stablz.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stablz.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/star.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/star.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/start4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/start4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/status.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/status.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stepi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stepi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stepk.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stepk.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/steps.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/steps.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/stumpf.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/stumpf.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/subint.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/subint.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/subsys.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/subsys.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/swcond.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/swcond.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/sweep.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/sweep.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/switch.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/switch.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/synch.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/synch.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tchain.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tchain.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tcirc.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tcirc.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tides3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tides3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/touch.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/touch.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tperi.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tperi.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trans3.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trans3.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trans4.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trans4.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transk.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transk.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transq.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transq.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/transx.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/transx.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trdot.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trdot.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trdot2.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trdot2.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/trflow.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/trflow.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/triple.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/triple.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tstab.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tstab.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/tstep.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/tstep.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/units.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/units.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/unpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/unpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/update.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/update.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/util_gpu.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/util_gpu.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/verify.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/verify.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xcpred.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xcpred.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtf.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtf.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtpert.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtpert.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnl0.F` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnl0.F`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnld.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnld.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlf.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlf.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlt.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlt.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xtrnlv.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xtrnlv.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/xvpred.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/xvpred.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ycopy.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ycopy.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/ysave.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/ysave.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zare.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zare.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zcnsts.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zcnsts.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zdata.h` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zdata.h`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zero.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zero.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/src/amuse/community/nbody6xx/src/zfuncs.f` & `amuse-nbody6xx-2024.4.0/src/amuse/community/nbody6xx/src/zfuncs.f`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/__init__.py` & `amuse-nbody6xx-2024.4.0/support/__init__.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/classifiers.py` & `amuse-nbody6xx-2024.4.0/support/classifiers.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/config.py` & `amuse-nbody6xx-2024.4.0/support/config.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/generate_main.py` & `amuse-nbody6xx-2024.4.0/support/generate_main.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/getsp.class` & `amuse-nbody6xx-2024.4.0/support/getsp.class`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/getsp.java` & `amuse-nbody6xx-2024.4.0/support/getsp.java`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/misc.py` & `amuse-nbody6xx-2024.4.0/support/misc.py`

 * *Files identical despite different names*

### Comparing `amuse-nbody6xx-2023.11.0/support/setup_codes.py` & `amuse-nbody6xx-2024.4.0/support/setup_codes.py`

 * *Files identical despite different names*

